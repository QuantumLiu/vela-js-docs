[![Xiaomi Vela JS 应用开发文档](https://iot.mi.com/vela/quickapp/logo.png)Xiaomi Vela JS 应用开发文档](https://iot.mi.com/vela/quickapp/)

[教程](https://iot.mi.com/vela/quickapp/zh/guide/)

[组件](https://iot.mi.com/vela/quickapp/zh/components/)

[JS接口](https://iot.mi.com/vela/quickapp/zh/features/)

[编程示例](https://iot.mi.com/vela/quickapp/zh/samples/)

[工具](https://iot.mi.com/vela/quickapp/zh/tools/)

[教程](https://iot.mi.com/vela/quickapp/zh/guide/)

[组件](https://iot.mi.com/vela/quickapp/zh/components/)

[JS接口](https://iot.mi.com/vela/quickapp/zh/features/)

[编程示例](https://iot.mi.com/vela/quickapp/zh/samples/)

[工具](https://iot.mi.com/vela/quickapp/zh/tools/)

- [通用规范](https://iot.mi.com/vela/quickapp/zh/components/general/)

- [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)
- [颜色配置](https://iot.mi.com/vela/quickapp/zh/components/general/color.html)
- [动画样式](https://iot.mi.com/vela/quickapp/zh/components/general/animation-style.html)
- [背景图样式](https://iot.mi.com/vela/quickapp/zh/components/general/background-img-styles.html)
- [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)
- [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)
- [通用方法](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html)

- [容器组件](https://iot.mi.com/vela/quickapp/zh/components/container/)

- [div](https://iot.mi.com/vela/quickapp/zh/components/container/div.html)
- [list](https://iot.mi.com/vela/quickapp/zh/components/container/list.html)
- [list-item](https://iot.mi.com/vela/quickapp/zh/components/container/list-item.html)
- [scroll](https://iot.mi.com/vela/quickapp/zh/components/container/scroll.html)
- [stack](https://iot.mi.com/vela/quickapp/zh/components/container/stack.html)
- [swiper](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html)

- [基础组件](https://iot.mi.com/vela/quickapp/zh/components/basic/)

- [text](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html)
- [span](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html)
- [a](https://iot.mi.com/vela/quickapp/zh/components/basic/a.html)
- [image](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html)
- [image-animator](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html)
- [progress](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html)
- [marquee](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html)
- [chart](https://iot.mi.com/vela/quickapp/zh/components/basic/chart.html)
- [qrcode](https://iot.mi.com/vela/quickapp/zh/components/basic/qrcode.html)
- [barcode](https://iot.mi.com/vela/quickapp/zh/components/basic/barcode.html)

- [表单组件](https://iot.mi.com/vela/quickapp/zh/components/form/)

- [input](https://iot.mi.com/vela/quickapp/zh/components/form/input.html)
- [picker](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html)
- [switch](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html)
- [slider](https://iot.mi.com/vela/quickapp/zh/components/form/slider.html)

# [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#%E9%80%9A%E7%94%A8%E6%96%B9%E6%B3%95) 通用方法

通用方法，是所有组件都可以调用的方法。在组件使用id标记 id 属性后，开发者可通过this.$element('idName')获取 dom 节点，再调用通用方法。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#this-element) this.$element

获取指定 id 的组件 dom 对象，如果没有指定 id，则返回根组件 dom 对象，假设有如下模板：

```
<template>
  <div>
    <div id='xxx'></div>
  </div>
</template>

```

this.$element('xxx') 获取 id 为 xxx 的 div 组件实例对象， this.$element() 获取模板中的根组件实例对象。

`id` 属性赋值可以查看此 [文档](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)。

通过 this.$element 获取到的 dom 对象，提供两个 api 供调用：

### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#getboundingclientrect-object-object) getBoundingClientRect(Object object) [2+](https://iot.mi.com/vela/quickapp/zh/guide/version/APILevel2)

返回元素的大小及其相对于视窗的位置，需要在页面的 onShow 生命周期之后调用。

#### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#%E5%8F%82%E6%95%B0) 参数

Object object

| 属性 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| success | function |  | 否 | 接口调用成功的回调函数 |
| fail | function |  | 否 | 接口调用失败的回调函数 |
| complete | function |  | 否 | 接口调用结束的回调函数（调用成功、失败都会执行） |

#### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#object-success-%E5%9B%9E%E8%B0%83%E5%87%BD%E6%95%B0%E5%8F%82%E6%95%B0%E8%AF%B4%E6%98%8E) object.success 回调函数参数说明

Object rect

| 属性 | 类型 | 描述 |
| --- | --- | --- |
| left | number | 元素的左边界坐标 |
| right | number | 元素的右边界坐标 |
| top | number | 元素的上边界坐标 |
| bottom | number | 元素的下边界坐标 |
| width | number | 元素的宽度 |
| height | number | 元素的高度 |

#### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#%E4%BB%A3%E7%A0%81%E7%A4%BA%E4%BE%8B) 代码示例

```
<template>
  <div>
    <div id="box1" class="box-normal"></div>
    <div id="box2" class="box-normal"></div>
  </div>
</template>
<script>
  export default {
    onShow(){
      this.$element('box1').getBoundingClientRect({
        success: function(data) {
          const { top, bottom, left, right, width, height } = data;
          console.log(data);
        },
        fail: (errorData, errorCode) => {
          console.log(`错误原因：${JSON.stringify(errorData)}, 错误代码：${errorCode}`)
        },
        complete: function() {
          console.info('complete')
        }
      })
    }
  }
</script>

```

### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#focus-object-object) focus(Object object)

使组件获得或者失去焦点的方法

#### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#%E5%8F%82%E6%95%B0-2) 参数

| 属性 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| focus | boolean | true | 否 | 使组件获得或者失去焦点，聚焦时可触发 focus 伪类效果（focus 伪类样式还未支持） |

#### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html\#%E4%BB%A3%E7%A0%81%E7%A4%BA%E4%BE%8B-2) 代码示例

```
<script>
  // 聚焦效果
  this.$element('box1').focus();
  // 聚焦效果
  this.$element('box2').focus({focus:true});
  // 失焦效果
  this.$element('box3').focus({focus:false});
</script>

```

←
[通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)[div](https://iot.mi.com/vela/quickapp/zh/components/container/div.html)
→


快速导航

[this.$element](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html#this-element "this.$element")

[getBoundingClientRect(Object object)](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html#getboundingclientrect-object-object "getBoundingClientRect(Object object)")

[focus(Object object)](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html#focus-object-object "focus(Object object)")