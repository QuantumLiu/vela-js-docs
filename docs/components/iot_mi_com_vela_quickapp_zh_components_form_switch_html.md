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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#switch) switch

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#%E6%A6%82%E8%BF%B0) 概述

开关选择

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| checked | `<boolean>` | false | 否 | 可触发 checked 伪类（checked 伪类样式还未支持） |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| thumb-color | `<color>` | #ffffff 或者 rgb(255, 255, 255) | 否 | 滑块颜色 |
| track-color | `<color>` | #0d84ff 或者 rgb(13, 132, 255) | 否 | 滑轨颜色 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| change | {checked:checkedValue} | checked 状态改变时触发 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div class="page">
    <text class="title">switch 组件</text>
    <switch checked="{{ switchValue }}" class="switch" @change="onSwitchChange"></switch>
    <text>状态：{{ switchValue }}</text>
  </div>
</template>

<script>
  export default {
    private: {
      switchValue: true
    },
    onSwitchChange(e) {
      this.switchValue = e.checked
    }
  }
</script>

<style>
  .page {
    flex-direction: column;
    padding: 30px;
    background-color: #ffffff;
  }

  .title {
    font-weight: bold;
  }

  .switch {
    width: 100px;
    margin-top: 10px;
  }
</style>

```

![](https://iot.mi.com/vela/quickapp/assets/img/switch.9fcb7b6a.gif)

←
[picker](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html)[slider](https://iot.mi.com/vela/quickapp/zh/components/form/slider.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html#%E4%BA%8B%E4%BB%B6 "事件")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")