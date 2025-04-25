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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#swiper) swiper

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E6%A6%82%E8%BF%B0) 概述

滑块视图容器。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| index | `<number>` | ０ | 否 | 当前显示的子组件索引 |
| autoplay | `<boolean>` | false | 否 | 渲染完成后，是否自动进行播放 |
| interval | `<number>` | 3000ms | 否 | 自动播放时的时间间隔，单位毫秒 |
| indicator | `<boolean>` | true | 否 | 是否启用 indicator，默认 true |
| loop | `<boolean>` | true | 否 | 是否开启循环模式 |
| duration | `<number>` | - | 否 | 滑动动画时长（duration默认根据手指的速度动态计算） |
| vertical | `<boolean>` | false | 否 | 滑动方向是否为纵向，纵向时indicator 也为纵向 |
| previousmargin | `<string>` | 0px | 否 | 前边距，可用于露出前一项的一小部分，支持单位：px和% |
| nextmargin | `<string>` | 0px | 否 | 后边距，可用于露出后一项的一小部分，支持单位：px和% |
| enableswipe | `<boolean>` | true | 否 | 是否支持手势滑动swiper |

**备注**： `previousmargin` 和 `nextmargin` 的总和不应该超过整个swiper大小的1/2，超过部分将会被截取。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| indicator-color | `<color>` | rgba(0, 0, 0, 0.5) | 否 | indicator 填充颜色 |
| indicator-selected-color | `<color>` | #33b4ff 或者 rgb(51, 180, 255) | 否 | indicator 选中时的颜色 |
| indicator-size | `<length>` | 20px | 否 | indicator 组件的直径大小 |
| indicator-\[top\|left\|right\|bottom\] | `<length>` \| `<percentage>` | - | 否 | indicator相对于swiper的位置 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| change | {index:currentIndex} | 当前显示的组件索引变化时触发 |
| swipestart [2+](https://iot.mi.com/vela/quickapp/zh/guide/version/APILevel2) | {index:currentIndex} | 子组件切换动画开始时触发（如果是手指拖动导致的切换，指的是手指按压开始拖动的时间点） |
| swipeend [2+](https://iot.mi.com/vela/quickapp/zh/guide/version/APILevel2) | {index:currentIndex} | 子组件切换动画结束时触发 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E6%96%B9%E6%B3%95) 方法

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| swipeTo | {index: number(指定位置)} | swiper 滚动到 index 位置 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div class="page">
    <swiper class="swiper">
      <text class="item item-1">A</text>
      <text class="item item-2">B</text>
      <text class="item item-3">C</text>
      <text class="item item-4">D</text>
    </swiper>

  </div>
</template>

<style>
  .page {
    padding: 30px;
    background-color: white;
  }

  .swiper {
    width: 300px;
    height: 160px;
    indicator-size: 10px;
  }

  .item {
    text-align: center;
    color: white;
    font-size: 30px;
  }

  .item-1 {
    background-color: #3f56ea;
  }

  .item-2 {
    background-color: #00bfc9;
  }

  .item-3 {
    background-color: #47cc47;
  }

  .item-4 {
    background-color: #FF6A00;
  }
</style>

```

![](https://iot.mi.com/vela/quickapp/assets/img/swiper.3d3d5407.gif)

←
[stack](https://iot.mi.com/vela/quickapp/zh/components/container/stack.html)[text](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E4%BA%8B%E4%BB%B6 "事件")

[方法](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E6%96%B9%E6%B3%95 "方法")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")