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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#picker) picker

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#%E6%A6%82%E8%BF%B0) 概述

滚动选择器，目前支持两种选择器，普通选择器，时间选择器。默认为普通选择器。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

**普通选择器**

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| type | text | - | 是 | 不支持动态修改 |
| range | `<array>` | - | 否 | 选择器的取值范围 |
| selected | `<number>` | 0 | 否 | 选择器的默认取值，取值为 range 的索引 |

**时间选择器**

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| type | time | - | 是 | 不支持动态修改 |
| selected | `<string>` | 当前时间 | 否 | 选择器的默认取值，格式为 hh:mm |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| color | `<color>` | 主题色 | 否 | 候选项字体颜色 |
| font-size | `<length>` | 30px | 否 | 候选项字体尺寸，单位px |
| selected-color | `<length>` | #ffffff | 否 | 选中项字体颜色 |
| selected-font-size | `<length>` | 20px | 否 | 选中项字体尺寸，单位px |
| selected-background-color | `<color>` | - | 否 | 选中项背景颜色 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#%E4%BA%8B%E4%BB%B6) 事件

**普通选择器**

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| change | {newValue:newValue, newSelected:newSelected} | 滚动选择器选择值后确定时触发（newSelected 为索引） |

**时间选择器**

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| change | {hour:hour, minute:minute} | 滚动选择器选择值后确定时触发 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div class="page">
    <text class="title">普通picker</text>
    <picker
      class="picker"
      type="text"
      range="{{pickerList}}"
      selected="1"
      onchange="onPickerChange">
    </picker>
    <text class="value">选择的值：{{v1}}</text>

    <text class="title">时间picker</text>
    <picker
      class="picker"
      type="time"
      selected="12:00"
      onchange="onTimePickerChange">
    </picker>
    <text class="value">选择的值：{{v2}}</text>
  </div>
</template>

<script>
  export default {
    private: {
      pickerList: ['apple', 'peach', 'pear', 'banana'],
      v1: 'peach',
      v2: '12:00'
    },
    onPickerChange(e) {
      this.v1 = e.newValue;
    },
    onTimePickerChange(e) {
      this.v2 = e.hour + ':' + e.minute;
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
    color: #000;
  }

  .value {
    margin-top: 5px;
    margin-bottom: 30px;
    color: #090;
  }

  .picker {
    font-size: 25px;
    color: #000;
    selected-font-size: 30px;
    selected-color: #09f;
    selected-background-color: #ccc;
  }
</style>

```

![](https://iot.mi.com/vela/quickapp/assets/img/picker.5b1be30e.gif)

←
[input](https://iot.mi.com/vela/quickapp/zh/components/form/input.html)[switch](https://iot.mi.com/vela/quickapp/zh/components/form/switch.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html#%E4%BA%8B%E4%BB%B6 "事件")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")