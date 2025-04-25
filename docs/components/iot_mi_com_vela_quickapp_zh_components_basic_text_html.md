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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#text) text

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#%E6%A6%82%E8%BF%B0) 概述

文本内容写在标签内容区，支持转义字符 `"\"`。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

仅支持 `<span>`

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| lines | `<number>` | -1 | 否 | 文本行数，-1 代表不限定行数 |
| color | `<color>` | rgba(0, 0, 0, 0.54) | 否 | 文本颜色 |
| font-size | `<length>` | 30px | 否 | 文本尺寸 |
| font-style | normal \| italic | normal | 否 |  |
| font-weight | normal \| bold \| `<number>` | normal | 否 | 当前平台仅支持 `normal` 与 `bold` 两种效果，当值为数字时，低于 `550` 为前者，否则为后者 |
| text-decoration | underline \| line-through \| none | none | 否 |  |
| text-align | left \| center \| right | left | 否 |  |
| text-indent | `<length>` \| `<percentage>` | - | 否 | 规定文本块首行的缩进 |
| line-height | `<length>` | - | 否 | 文本行高 |
| text-overflow | clip \| ellipsis | clip | 否 | 在设置了行数的情况下生效 |

**示例**

- 单行省略



```
text {
    width: 150px;
    lines: 1;
    text-overflow: ellipsis;
}

```



![](<Base64-Image-Removed>)

- 多行省略，以两行为例



```
text {
    width: 100px;
    lines: 2;
    text-overflow: ellipsis;
}

```



![](<Base64-Image-Removed>)


## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div>
    <text>这是一段文本</text>
  </div>
</template>

```

![](<Base64-Image-Removed>)

←
[swiper](https://iot.mi.com/vela/quickapp/zh/components/container/swiper.html)[span](https://iot.mi.com/vela/quickapp/zh/components/basic/span.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html#%E4%BA%8B%E4%BB%B6 "事件")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/basic/text.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")