# 多语言覆盖
Vela 的能力会覆盖多个国家地区，框架支持多语言的能力后，可以让一个JS 应用产品（一个 RPK 文件）同时支持多个语言版本的切换，开发者无需开发多个不同语言的源代码项目，避免给项目维护带来困难。
使用系统默认的语言，开发者配置多语言的方式非常简单，只需要`定义资源`与`引用资源`两个步骤即可。

## 定义资源文件
资源文件用于存放多个语言的业务信息定义，与其它技术平台类似（它们使用`properties文件`或者`xml文件`的格式），JS 应用平台使用`JSON文件`保存资源定义；
在项目源代码`src目录`下定义`i18n文件夹`，内部放置每个语言地区下的资源定义文件即可；其中文件名定义为：`zh-CN.json`、`zh.json`；
如果开发者当前产品仅计划支持一种语言，同时还希望用到多语言能力，那么仅声明一个名称为`defaults.json`的文件即可；
每个 JSON 文件的内容格式如下：
```
{
 "message": {
  "pageA": {
   "text": "pure-text-content",
   "format": {
    "object": "type-{name}",
    "array": "type-{0}"
   },
   "array": [
    "item-type-string",
    {
     "key": "item-type-object-attribute"
    },
    ["item-type-array"]
   ],
   "plurals": {
    "double": "car | cars",
    "three": "no apples | one apple | {count} apples",
    "format": {
     "object": "type-{name}",
     "array": "type-{0}"
    }
   }
  }
 }
}
```

页面中通过`message.pageA.text`类似的`path`引用对应内容`"pure-text-content"`；

## 页面中引用资源
页面中多语言的使用语法，主要体现在 ViewModel 的几个函数上，如：`$t`，这些方法可以在`<template>`或`<script>`中使用；
如下代码所示：
```
<template>
 <div class="page">
  <text>{{ $t('message.pageA.text') }}</text>
  <text>{{ $t('message.pageA.format.object', { name: 'arg-object' }) }}</text>
  <text>{{ $t('message.pageA.format.array', ['arg-array']) }}</text>
 </div>
</template>
<script>
 export default {
  onInit () {
   // 简单格式化：
   this.$t('message.pageA.text')
   this.$t('message.pageA.format.object', { name: 'arg-object' })
   this.$t('message.pageA.format.array', ['arg-array'])
  }
 }
</script>
<style>
 .page {
  flex-direction: column;
  background-color: white;
  padding: 30px;
 }
</style>
```

### 效果展示
![](https://iot.mi.com/vela/quickapp/zh/guide/framework/other/i18n.html)

### 简单格式化方法
属性 | 类型 | 参数 | 描述  
---|---|---|---  
$t | Function | path: String 资源路径 arg0: object | array 格式化参数，非必要参数，根据系统语言完成简单的替换：`this.$t('message.pageA.text')`  
比如：
```
// 示例：无额外参数的格式化
// 输出："pure-text-content"
this.$t('message.pageA.text')
// 示例：额外参数为对象，替换引用内容中的绑定
// 输出："type-arg-object"
this.$t('message.pageA.format.object', { name: 'arg-object' })
// 示例：额外参数为数组，替换引用内容中的绑定
// 输出："type-arg-array"
this.$t('message.pageA.format.array', ['arg-array'])
```

### 单复数格式化方法
属性 | 类型 | 参数 | 描述  
---|---|---|---  
$tc | Function | path: String 资源路径 count: number 要表达的值 | 根据系统语言完成单复数替换：`this.$tc('message.plurals.double')`，注意：定义资源的内容通过 | 分隔为多个选项  
比如：
```
// 示例：message的值为两个选项时，传递数值不为单数
// 输出："cars"
this.$tc('message.pageA.plurals.double', 0)
// 示例：message的值为两个选项时，传递数值为单数
// 输出："car"
this.$tc('message.pageA.plurals.double', 1)
// 示例：message的值为两个选项时，传递数值不为单数
// 输出："cars"
this.$tc('message.pageA.plurals.double', 2)
// 示例：message的值为三个及以上的选项时，传递数值不为单数
// 输出："no apples"
this.$tc('message.pageA.plurals.three', 0)
// 示例：message的值为三个及以上的选项时，传递数值为单数
// 输出："one apple"
this.$tc('message.pageA.plurals.three', 1)
// 示例：message的值为三个及以上的选项时，传递数值不为单数
// 输出："10 apples"
this.$tc('message.pageA.plurals.three', 10)
```

## 修改地区语言后的回调
当用户在系统设置切换地区语言，会触发 onConfigurationChanged 回调，且返回来的 event.type 值为locale。
详情可参考[文档](https://iot.mi.com/vela/quickapp/zh/guide/framework/script/lifecycle.html#onconfigurationchangedevent)。
示例代码：
```
// 监听语言变化
onConfigurationChanged(event) {
 if (event && event.type && event.type === 'locale') {
  console.log('locale or language changed!')
 }
}
