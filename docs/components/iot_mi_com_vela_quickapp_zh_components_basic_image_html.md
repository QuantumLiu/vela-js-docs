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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#image) image

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#%E6%A6%82%E8%BF%B0) 概述

渲染图片

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| src | `<uri>` | - | 否 | 图片的 uri，同时支持本地和云端路径，支持的图片格式包括png，jpg |
| alt | `<uri>` \| 'blank' | - | 否 | 加载时显示的占位图；只支持本地图片资源 |

注意：alt 属性详情如下：

- 如果 Image 组件没有设置 alt 值，终端会加上默认的灰色占位图；

- src 为本地图片地址时，不会有占位图；

- src 为远程图片地址时，如果之前已经成功加载过图片，有本地缓存，则不会有占位图；

- src 为远程图片地址时，且 Image 组件 的 alt 值传入字符串 "blank" 值，不会有占位图（可避免一些远程地址的小图标第一次加载时瞬间闪烁的现象）；

- 设置 alt 为本地图片地址时，占位图缩放模式由原来的居中不缩放改为居中保持宽高比缩放，减少了占位图资源文件的分辨率与体积大小。


注：缩放模式可以通过样式值 `object-fit` 配置，默认值为 `cover`（居中保持宽高比缩放），详情查看 [样式](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E6%A0%B7%E5%BC%8F) 一节

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| object-fit | contain \| cover \| none \| scale-down | cover | 否 | 图片的缩放类型 |

注意：

1. object-fit参数列表如下：

| 类型 | 描述 |
| --- | --- |
| contain | 保持宽高比，缩小或者放大，使得图片完全显示在显示边界内，居中显示 |
| cover | 保持宽高比，缩小或者放大，使得两边都大于或等于显示边界，居中显示 |
| none | 居中，无缩放 |
| scale-down | 保持宽高比，缩小或保持不变，取 `contain` 和 `none` 中显示较小的一个，居中显示 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| complete | {width: widthValue(px), height: heightValue(px)} | 图片加载完成时触发 |
| error | - | 图片加载失败时触发 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div>
    <image src="/common/logo.png" />
  </div>
</template>

```

![](<Base64-Image-Removed>)

←
[a](https://iot.mi.com/vela/quickapp/zh/components/basic/a.html)[image-animator](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E4%BA%8B%E4%BB%B6 "事件")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")