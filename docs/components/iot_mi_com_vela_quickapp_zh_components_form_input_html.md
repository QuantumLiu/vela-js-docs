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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#input) input

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E6%A6%82%E8%BF%B0) 概述

提供可交互的界面，接收用户的输入。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| type | button \| checkbox \| radio \| | button | 否 | 支持动态修改 |
| checked | `<boolean>` | false | 否 | 当前组件的 checked 状态，type 为 checkbox 时生效，可触发 checked 伪类（checked 伪类样式还未支持） |
| name | `<string>` | - | 否 | input 组件名称 |
| value | `<string>` | - | 否 | input 组件的值 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| color | `<color>` | rgba(0, 0, 0, 0.87) | 否 | 文本颜色 |
| font-size | `<length>` | 37.5px | 否 | 文本尺寸 |
| width | `<length>` \| `<percentage>` | - | 否 | type 为 button 时，默认值为 128px |
| height | `<length>` \| `<percentage>` | - | 否 | type 为 button 时，默认值为 70px |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E4%BA%8B%E4%BB%B6) 事件

支持 [通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| change | 不同 type 参数不同，具体见下方 change 事件参数 | input 组件的值、状态发生改变时触发，type 为 button 时无 change 事件 |

### [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#change-%E4%BA%8B%E4%BB%B6%E5%8F%82%E6%95%B0) change 事件参数

| 参数 | checkbox | radio | 备注 |
| --- | --- | --- | --- |
| name | √ | √ | - |
| value | √ | √ | - |
| checked | √ | - | - |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E6%96%B9%E6%B3%95) 方法

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| focus | {focus:true\|false}，focus 不传默认为 true | 使组件获得或者失去焦点，可触发 focus 伪类（focus 伪类样式还未支持） |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/form/input.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div class="page">
    <div class="section">
      <text class="title">input-button 组件</text>
      <input class="button" type="button" value="按钮" @click="onButtonClick" />
      <text>{{ buttonText }}</text>
    </div>
    <div class="section">
      <text class="title">input-checkbox 组件</text>
      <input class="checkbox" type="checkbox" checked="{{ checkboxChecked }}" @change="onCheckboxChange" />
      <text>我的勾选状态: {{ checkboxChecked }}</text>
    </div>
    <div class="section">
      <text class="title">input-radio 组件</text>
      <div>
        <input class="radio" type="radio" name="radio" value="1" checked="{{radioValue === '1'}}" @change="onRadioChange" />
        <input class="radio" type="radio" name="radio" value="2" checked="{{radioValue === '2'}}" @change="onRadioChange" />
        <input class="radio" type="radio" name="radio" value="3" checked="{{radioValue === '3'}}" @change="onRadioChange" />
      </div>
      <text>当前选中第{{ radioValue }}个</text>
    </div>
  </div>
</template>

<script>
  export default {
    private: {
      buttonText: '',
      checkboxChecked: true,
      radioValue: '1'
    },
    onTextChange(e) {
      this.textValue = e.value
    },
    onButtonClick() {
      this.buttonText = '按钮被点击了'
    },
    onCheckboxChange(e) {
      this.checkboxChecked = e.checked
    },
    onRadioChange(e) {
      this.radioValue = e.value
    }
  }
</script>

<style>
  .page {
    flex-direction: column;
    padding: 30px;
    background-color: #ffffff;
  }

  .section {
    flex-direction: column;
    margin-bottom: 30px;
  }

  .title {
    font-weight: bold;
  }

  .button {
    width: 140px;
    height: 50px;
    font-size: 25px;
    color: white;
  }

  .checkbox, .radio {
    width: 40px;
    height: 40px;
    margin-right: 10px;
  }
</style>

```

![](https://iot.mi.com/vela/quickapp/assets/img/input.ad1a9272.gif)

←
[barcode](https://iot.mi.com/vela/quickapp/zh/components/basic/barcode.html)[picker](https://iot.mi.com/vela/quickapp/zh/components/form/picker.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E6%A0%B7%E5%BC%8F "样式")

[事件](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E4%BA%8B%E4%BB%B6 "事件")

[change 事件参数](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#change-%E4%BA%8B%E4%BB%B6%E5%8F%82%E6%95%B0 "change 事件参数")

[方法](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E6%96%B9%E6%B3%95 "方法")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/form/input.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")