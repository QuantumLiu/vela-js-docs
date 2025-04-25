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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#progress) progress

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#%E6%A6%82%E8%BF%B0) 概述

进度条

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| percent | `<number>` | 0 | 否 | - |
| type | horizontal \| arc | horizontal | 否 | 进度条类型，不支持动态修改 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

注：horizontal progress 底色为#f0f0f0；height 属性失效

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| color | `<color>` | #33b4ff 或者 rgb(51, 180, 255) | 否 | 进度条的颜色 |
| stroke-width | `<length>` | 32px | 否 | 进度条的宽度 |
| layer-color | `<color>` | #f0f0f0 或者 rgb(240, 240, 240) | 否 | 进度条的背景颜色 |

type=arc时生效：

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| start-angle | `<deg>` | 240 | 否 | 弧形进度条起始角度，以时钟0点为基线。范围为0到360（顺时针） |
| total-angle | `<deg>` | 240 | 否 | 弧形进度条总长度，范围为-360到360，负数表示起点到终点为逆时针 |
| center-x | `<length>` | 组件宽度的一半 | 否 | 弧形进度条中心位置，（坐标原点为组件左上角顶点）。该样式需要和 center-y \ radius 一起使用 |
| center-y | `<length>` | 组件高度的一半 | 否 | 弧形进度条中心位置，（坐标原点为组件左上角顶点）。该样式需要和 center-x \ radius 一起使用 |
| radius | `<length>` | 组件宽高较小值的一半 | 否 | 弧形进度条半径，该样式需要和 center-x \ center-y 一起使用 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div style="flex-direction: column">
    <progress class="p1" percent="40"></progress>
    <progress class="p2" percent="80" type="arc"></progress>
  </div>
</template>
<style>
  .p1 {
    margin-bottom: 10px;
    stroke-width: 12px;
  }

  .p2 {
    margin-bottom: 10px;
    stroke-width: 12px;
    start-angle: 0;
    total-angle: 360deg;
  }
</style>

```

![](<Base64-Image-Removed>)

←
[image-animator](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html)[marquee](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html#%E4%BA%8B%E4%BB%B6 "事件")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")