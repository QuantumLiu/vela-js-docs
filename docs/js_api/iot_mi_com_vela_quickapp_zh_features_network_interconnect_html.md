# 设备通信 interconnect

用于和搭配使用的手机 app 进行通信，收发手机 app 数据。通信连接会自动建立，应用内不用关心连接的创建和销毁，但是可以注册回调函数来接收连接状态改变的信息，以便进行相应处理，例如对用户进行提示。

## 接口声明
```
{ "name": "system.interconnect" }
```

## 导入模块
```
import interconnect from '@system.interconnect' 
// 或 
const interconnect = require('@system.interconnect')
```

## 接口定义
### interconnect.instance()
获取连接对象，在 app 中以单例形式存在，后续的数据收发都是基于这个连接对象
#### 参数：
无
#### 示例：
```
let conn = interconnect.instance()
```

### conn.getReadyState(OBJECT)
获取 App 连接状态
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  

#### success 返回值：
参数值 | 类型 | 说明  
---|---|---  
status | number | 1：连接成功，2：连接断开  

#### fail 返回值：
错误码 | 说明  
---|---  
1006 | 连接断开  

#### 示例：
```
conn.getReadyState({
 success: data => {
  if (data.status === 1) {
   console.log('连接成功')
  } else if (data.status === 2) {
   console.log('连接失败')
  }
 },
 fail: (data, code) => {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### conn.send(OBJECT)
发送数据到手机 App 端
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
data | Object | 否 | 发送的数据  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  

#### success 返回值：
无

#### fail 返回值：
错误码 | 说明  
---|---  
1006 | 连接断开  

#### 示例：
```
conn.send({
 data: {},
 success: ()=>{
  console.log(`handling success`)
 },
 fail: (data: {data, code})=> {
  console.log(`handling fail, errMsg = ${data.data}, errCode = ${data.code}`)
 }
})
```

## 事件
### conn.onmessage
接收手机 App 端数据
#### 回调参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
data | Object | 否 | 接收的数据  

#### 示例：
```
conn.onmessage = (data) => {
 console.log(`received message: ${data.data}`)
}
```

### conn.onopen
连接打开时的回调函数
#### 回调参数：
无

#### 示例：
```
conn.onopen = () => {
 console.log(`connection opened`)
}
```

### conn.onclose
连接关闭时的回调函数
#### 回调参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
data | Object | 否 | 连接关闭返回的数据  

#### 示例：
```
conn.onclose = (data) => {
 console.log(`connection closed, reason = ${data.data}, code = ${data.code}`)
}
```

### conn.onerror
连接出错时的回调函数
#### 回调参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
data | Object | 否 | 连接出错返回的数据  

#### 示例：
```
conn.onerror = (data)=> {
 console.log(`connection error, errMsg = ${data.data}, errCode = ${data.code}`)
}
```

## 开发注意事项
interconnect 通信前提要保证快应用和三方应用安卓端两者的包名及签名保持一致。
  * 保证快应用 manifest.json 里 package 字段与 需要接入的三方app 安卓端包名一致。
  * 快应用签名需要使用三方应用安卓端签名，可以从.jks中提取证书及私钥，方法如下：

  1. 先将 jks 转换成 p12，执行以下命令，输入相应密码后，在同级目录下生成对应的 p12 格式文件。

```
keytool -importkeystore -srckeystore keystore.jks -destkeystore keystore.p12 -srcstoretype jks -deststoretype pkcs12
```

  1. 再将 p12 转 pem，执行以下命令，输入上一步设置的 p12 文件密码后，在同级目录下生成对应的 pem 格式文件。

```
openssl pkcs12 -nodes -in keystore.p12 -out keystore.pem
```

  1. 从 pem 格式文件中复制出私钥和证书： 把-----BEGIN PRIVATE KEY-----到-----END PRIVATE KEY-----的内容复制到private.pem中。 把-----BEGIN CERTIFICATE-----到-----END CERTIFICATE-----的内容复制到certificate.pem中。

  * 如果本地没有安装Openssl或想要更简便的操作流程，我们提供了[在线签名生成工具 (opens new window)](https://cdn.hybrid.xiaomi.com/aiot-ide/signature-generate-tool/v2/index.html)。该工具是一个基于WebAssembly编写的Web应用，它可以在浏览器环境中直接生成 pem 格式的私钥和证书，无需将签名文件和密码上传到远程服务器，充分保证了用户的隐私安全。使用在线签名生成工具的步骤如下：
    1. 上传 p12 文件并输入对应的密码；
    2. 点击"生成签名"按钮，等待签名生成成功弹窗出现；
    3. 点击"下载签名"按钮，下载 pem 格式的私钥和证书；
  * 快应用需要将上述生成的私钥 private.pem 和证书 certificate.pem 放在快应用根目录 /sign/debug 和 /sign/release 下打包测试。
  * 在真机测试的时候建议先输入包名uninstall老包再安装新包，可以观察桌面图标卸载的话会删除应用图标保证彻底替换。

参考附录
  1. 小米穿戴第三方APP能力开放接口文档：[点击下载 (opens new window)](https://vela-docs.cnbj1.mi-fds.com/vela-docs/files/%E5%B0%8F%E7%B1%B3%E7%A9%BF%E6%88%B4%E7%AC%AC%E4%B8%89%E6%96%B9APP%E8%83%BD%E5%8A%9B%E5%BC%80%E6%94%BE%E6%8E%A5%E5%8F%A3%E6%96%87%E6%A1%A3_1.4.pdf "下载")
  2. interconnect开发测试demo：[点击下载 (opens new window)](https://cdn.cnbj3-fusion.fds.api.mi-img.com/quickapp-vela/interconnect_dev_test_demo.zip "下载")
