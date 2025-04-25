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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#span) span

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#%E6%A6%82%E8%BF%B0) 概述

格式化的文本，只能作为 [`<text>`](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html)、 [`<a>`](https://iot.mi.com/vela/quickapp/zh/components/basic/a.html) 和 `<span>` 的子组件。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

仅支持 `<span>`

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#%E5%B1%9E%E6%80%A7) 属性

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| id | `<string>` | - | 否 | 唯一标识 |
| style | `<string>` | - | 否 | 样式声明 |
| class | `<string>` | - | 否 | 引用样式表 |
| for | `<array>` | - | 否 | 根据数据列表，循环展开当前标签 |
| if | `<boolean>` | - | 否 | 根据数据 boolean 值，添加或移除当前标签 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#%E6%A0%B7%E5%BC%8F) 样式

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| color | `<color>` | rgba(0, 0, 0, 0.54) | 否 | 文本颜色 |
| font-size | `<length>` | 30px | 否 | 文本尺寸 |
| font-style | normal \| italic | normal | 否 | - |
| font-weight | normal \| bold \| `<number>` | normal | 否 | 当前平台仅支持 `normal` 与 `bold` 两种效果，当值为数字时，低于 `550` 为前者，否则为后者 |
| text-decoration | underline \| line-through \| none | none | 否 | - |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#%E4%BA%8B%E4%BB%B6) 事件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div>
    <text>
      <span>I am span,</span>
      <span style="color: #f76160">I am span,</span>
      <span style="color: #f76160;text-decoration: underline;">I am span,</span>
    </text>
  </div>
</template>

```

![](<Base64-Image-Removed>)

←
[text](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html)[a](https://iot.mi.com/vela/quickapp/zh/components/basic/a.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html#%E4%BA%8B%E4%BB%B6 "事件")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")