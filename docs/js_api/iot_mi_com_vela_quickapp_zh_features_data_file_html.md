# 文件存储 file

## 接口声明
```
{ "name": "system.file" }
```

## 导入模块
```
import file from '@system.file' 
// 或 
const file = require('@system.file')
```

## 接口定义
### file.move(OBJECT)
将源文件移动到指定位置
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
srcUri | String | 是 | 源文件的 uri  
dstUri | String | 是 | 目标文件的 uri  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.move({
 srcUri: 'internal://cache/path/to/file',
 dstUri: 'internal://files/path/to/file',
 success: function(uri) {
  console.log(`move success: ${uri}`)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.copy(OBJECT)
将源文件复制一份并存储到指定位置
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
srcUri | String | 是 | 源文件的 uri  
dstUri | String | 是 | 目标文件的 uri  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.copy({
 srcUri: 'internal://cache/path/to/file',
 dstUri: 'internal://files/path/to/file',
 success: function(uri) {
  console.log(`copy success: ${uri}`)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.list(OBJECT)
获取指定目录下的文件列表
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 目录 uri  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.list({
 uri: 'internal://files/movies/',
 success: function(data) {
  console.log(data.fileList)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.get(OBJECT)
获取本地文件的文件信息
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 文件的 uri  
recursive | Boolean | 否 | 是否递归获取子目录文件列表  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.get({
 uri: 'internal://files/path/to/file',
 success: function(data) {
  console.log(data.uri)
  console.log(data.length)
  console.log(data.lastModifiedTime)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.delete(OBJECT)
删除本地存储的文件
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 需要删除的文件 uri  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.delete({
 uri: 'internal://files/path/to/file',
 success: function(data) {
  console.log('handling success')
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.writeText(OBJECT)
写文本到文件
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 本地文件路径  
text | String | 是 | 需要写入的字符串  
encoding | String | 否 | 编码格式  
append | Boolean | 否 | 是否追加模式  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.writeText({
 uri: 'internal://files/work/demo.txt',
 text: 'test',
 success: function() {
  console.log('handling success')
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.writeArrayBuffer(OBJECT)
写 Buffer 到文件
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 本地文件路径  
buffer | Uint8Array | 是 | 需要写入的 Buffer  
position | Number | 否 | 写入位置偏移量  
append | Boolean | 否 | 是否追加模式  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.writeArrayBuffer({
 uri: 'internal://files/work/demo',
 buffer: buffer,
 success: function() {
  console.log('handling success')
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.readText(OBJECT)
从文件中读取文本
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 本地文件路径  
encoding | String | 否 | 编码格式  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.readText({
 uri: 'internal://files/work/demo.txt',
 success: function(data) {
  console.log('text: ' + data.text)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.readArrayBuffer(OBJECT)
从文件中读取 Buffer
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 本地文件路径  
position | Number | 否 | 读取起始位置  
length | Number | 否 | 读取长度  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.readArrayBuffer({
 uri: 'internal://files/work/demo',
 position: 100,
 length: 100,
 success: function(data) {
  console.log('buffer.length: ' + data.buffer.length)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.access(OBJECT)
判断文件或目录是否存在
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 目录或文件 uri  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.access({
 uri: 'internal://files/test',
 success: function(data) {
  console.log(`handling success`)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.mkdir(OBJECT)
创建目录
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 目录的 uri  
recursive | Boolean | 否 | 是否递归创建上级目录  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.mkdir({
 uri: 'internal://files/dir/',
 success: function(data) {
  console.log(`handling success`)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
```

### file.rmdir(OBJECT)
删除目录
#### 参数：
参数名 | 类型 | 必填 | 说明  
---|---|---|---  
uri | String | 是 | 目录的 uri  
recursive | Boolean | 否 | 是否递归删除子文件和子目录  
success | Function | 否 | 成功回调  
fail | Function | 否 | 失败回调  
complete | Function | 否 | 执行结束后的回调  

#### 示例：
```
file.rmdir({
 uri: 'internal://files/dir/',
 success: function(data) {
  console.log(`handling success`)
 },
 fail: function(data, code) {
  console.log(`handling fail, code = ${code}`)
 }
})
