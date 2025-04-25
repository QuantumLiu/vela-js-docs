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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#%E9%80%9A%E7%94%A8%E4%BA%8B%E4%BB%B6) 通用事件

通用事件，即所有组件都支持的 `事件回调`。

开发者可以在组件标签上使用 `on{eventName}`（如 `onclick`）或 `@{eventName}`（如 `@click`）注册回调事件。

更详细的讲解，可查阅 [事件绑定](https://iot.mi.com/vela/quickapp/zh/guide/framework/template/event.html) 文档了解。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div>
      <text onclick="clickFunction1">line 1</text>
      <text @click="clickFunction2">line 2</text>
  </div>
</template>

```

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#%E9%80%9A%E7%94%A8%E4%BA%8B%E4%BB%B6%E5%88%97%E8%A1%A8) 通用事件列表

| 名称 | 参数 | 描述 | 冒泡 |
| --- | --- | --- | --- |
| touchstart | TouchEvent | 手指刚触摸组件时触发 | 支持 |
| touchmove | TouchEvent | 手指触摸后移动时触发 | 支持 |
| touchend | TouchEvent | 手指触摸动作结束时触发 | 支持 |
| click | MouseEvent | 组件被点击时触发 | 支持 |
| longpress | MouseEvent | 组件被长按时触发 | 支持 |
| swipe | { direction: < `"left"` \| `"right"` \| `"up"` \| `"down"` \> } | 组件上快速滑动后触发（滑动方向有滚动条时不触发该事件）<br> 参数说明：<br> left：　向左滑动；<br>right： 向右滑动；<br>up：　 向上滑动；<br>down：向下滑动； | 不支持 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#%E4%BA%8B%E4%BB%B6%E5%AF%B9%E8%B1%A1) 事件对象

### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#_1%E3%80%81touchevent-%E7%B1%BB%E5%9E%8B%E8%AF%B4%E6%98%8E) 1、TouchEvent 类型说明：

| 属性 | 类型 | 说明 |
| --- | --- | --- |
| touches | TouchList | 触摸事件，当前停留在屏幕中的触摸点信息的数组 |
| changedTouches | TouchList | 触摸事件，当前变化的触摸点信息的数组。changedTouches 数据格式同 touches， 表示有变化的触摸点，如从无变有（touchstart），位置变化（touchmove），从有变无（touchend），<br>比如用户手指离开屏幕时，touches 数组中无数据，而 changedtouches 则会保存离开前的数据 |

**其中，TouchList 是 Touch 对象的集合。**

### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#_2%E3%80%81touch-%E7%B1%BB%E5%9E%8B%E8%AF%B4%E6%98%8E) 2、Touch 类型说明

| 属性 | 类型 | 说明 |
| --- | --- | --- |
| identifier | number | 触摸点的标识符。对于多点同时触摸则是 \[0,1,2,3,...\]，分别表示第一个手指、第二个手指...<br>一次触摸动作(手指按下到手指离开的过程)，在整个屏幕移动过程中，该标识符不变，可以用来判断是否是同一次触摸过程 |
| clientX | number | 距离可见区域左边沿的 X 轴坐标，不包含任何滚动偏移 |
| clientY | number | 距离可见区域上边沿的 Y 轴坐标，不包含任何滚动偏移以及状态栏和 titlebar 的高度 |
| pageX | number | 距离可见区域左边沿的 X 轴坐标，包含任何滚动偏移 |
| pageY | number | 距离可见区域上边沿的 Y 轴坐标，包含任何滚动偏移。（不包含状态栏和 titlebar 的高度） |
| offsetX | number | 距离事件触发对象左边沿 X 轴的距离 |
| offsetY | number | 距离事件触发对象上边沿 Y 轴的距离 |

### [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#_3%E3%80%81mouseevent-%E7%B1%BB%E5%9E%8B%E8%AF%B4%E6%98%8E) 3、MouseEvent 类型说明

| 属性 | 类型 | 说明 |
| --- | --- | --- |
| clientX | number | 距离可见区域左边沿的 X 轴坐标，不包含任何滚动偏移 |
| clientY | number | 距离可见区域上边沿的 Y 轴坐标，不包含任何滚动偏移以及状态栏和 titlebar 的高度 |
| pageX | number | 距离可见区域左边沿的 X 轴坐标，包含任何滚动偏移 |
| pageY | number | 距离可见区域上边沿的 Y 轴坐标，包含任何滚动偏移。（不包含状态栏和 titlebar 的高度） |
| offsetX | number | 距离事件触发对象左边沿 X 轴的距离 |
| offsetY | number | 距离事件触发对象上边沿 Y 轴的距离 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/events.html\#%E7%A4%BA%E4%BE%8B) 示例

如下，在 div 上绑定了 click 和 touchmove 事件，触发事件时将事件打印出来。

```
<template>
  <div class="root-page">
    <div class="touch-region" onclick="click" ontouchmove="move"></div>
  </div>
</template>

<style>
  .root-page {
    flex-direction: column;
    align-items: center;
  }

  .touch-region {
    width: 80%;
    height: 20%;
    background-color: #444444;
  }

</style>

<script>
  export default {
    private: {},
    click(event) {
      console.log("click event fired")
    },
    move(event) {
      console.log("move event touches:" + JSON.stringify(event.touches))
      console.log("move event changedTouches:" + JSON.stringify(event.changedTouches))
    }
  }

</script>

```

**打印结果如下，click 事件：**

```
move event touches:[\
  {\
    "offsetX": 296,\
    "identifier": 0,\
    "offsetY": 113.48148345947266,\
    "clientY": 113.48148345947266,\
    "clientX": 360,\
    "pageY": 113.48148345947266,\
    "pageX": 360\
  }\
]

```

```
move event changedTouches:[\
  {\
    "offsetX": 296,\
    "identifier": 0,\
    "offsetY": 113.48148345947266,\
    "clientY": 113.48148345947266,\
    "clientX": 360,\
    "pageY": 113.48148345947266,\
    "pageX": 360\
  }\
]

```

```
click event fired

```

←
[通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)[通用方法](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html)
→


快速导航

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")

[通用事件列表](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#%E9%80%9A%E7%94%A8%E4%BA%8B%E4%BB%B6%E5%88%97%E8%A1%A8 "通用事件列表")

[事件对象](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#%E4%BA%8B%E4%BB%B6%E5%AF%B9%E8%B1%A1 "事件对象")

[1、TouchEvent 类型说明：](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#_1%E3%80%81touchevent-%E7%B1%BB%E5%9E%8B%E8%AF%B4%E6%98%8E "1、TouchEvent 类型说明：")

[2、Touch 类型说明](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#_2%E3%80%81touch-%E7%B1%BB%E5%9E%8B%E8%AF%B4%E6%98%8E "2、Touch 类型说明")

[3、MouseEvent 类型说明](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#_3%E3%80%81mouseevent-%E7%B1%BB%E5%9E%8B%E8%AF%B4%E6%98%8E "3、MouseEvent 类型说明")

[示例](https://iot.mi.com/vela/quickapp/zh/components/general/events.html#%E7%A4%BA%E4%BE%8B "示例")