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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#marquee) marquee

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E6%A6%82%E8%BF%B0) 概述

跑马灯，用来插入一段滚动的文字，默认为单行。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| scrollamount | `<number>` | 6 | 否 | 设置每次滚动时移动的长度，单位：px |
| loop | `<number>` | -1 | 否 | 设置 marquee 滚动的次数。如果未指定值，默认值为 −1，表示 marquee 将连续滚动 |
| direction | `<string>` | left | 否 | 文字滚动方向，支持 left，right |
| text-offset | `<number>` | - | 否 | 设置跑马灯首尾相接时，上一段的尾和下一段的头之间的距离，属性值为大于 0 的整数，单位：px |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| color | `<color>` | rgba(0, 0, 0, 0.54) | 否 | 文本颜色 |
| font-size | `<length>` | 30px | 否 | 文本尺寸 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| bounce | - | 当 marquee 滚动到结尾时触发 |
| finish | - | 当 marquee 完成设置的 loop 次数时触发，loop > 0 时有效 |
| start | - | 当 marquee 开始滚动时触发 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E6%96%B9%E6%B3%95) 方法

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| start | - | 开始滚动 marquee |
| stop | - | 停止滚动 marquee |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div>
    <marquee id="marquee" scrollamount={{6}} loop={{-1}}>
      scrollamount控制滚动速度，默认值为6（6像素/秒）
    </marquee>
  </div>
</template>

<script>
  export default {
    onReady() {
      this.$element('marquee').start()
    }
  }
</script>

```

![](https://iot.mi.com/vela/quickapp/assets/img/marquee.2b33a67c.gif)

←
[progress](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html)[chart](https://iot.mi.com/vela/quickapp/zh/components/basic/chart.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E4%BA%8B%E4%BB%B6 "事件")

[方法](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E6%96%B9%E6%B3%95 "方法")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/basic/marquee.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")