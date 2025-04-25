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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html\#%E9%80%9A%E7%94%A8%E5%B1%9E%E6%80%A7) 通用属性

通用属性，即所有组件都支持的属性。

开发者可以在所有的组件标签上都使用 `通用属性`。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div>
      <text id="text1" class="text-normal">line 1</text>
      <text id="text2" class="text-normal red">line 2</text>
  </div>
</template>

```

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html\#%E5%B8%B8%E8%A7%84%E5%B1%9E%E6%80%A7) 常规属性

| 名称 | 类型 | 默认值 | 描述 |
| --- | --- | --- | --- |
| id | `<string>` | - | 唯一标识 |
| style | `<string>` | - | 样式声明 |
| class | `<string>` | - | 引用样式表 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html\#%E6%B8%B2%E6%9F%93%E5%B1%9E%E6%80%A7) 渲染属性

| 名称 | 类型 | 默认值 | 描述 |
| --- | --- | --- | --- |
| for | `<array>` | - | 根据数据列表，循环展开当前标签 |
| if | `<boolean>` | - | 根据数据 boolean 值，添加或移除当前标签 |
| show | `<boolean>` | - | 根据数据 boolean 值，显示或隐藏当前标签，相当于控制{ display: flex \| none } |

渲染属性工作方式详见 [template 模板](https://iot.mi.com/vela/quickapp/zh/guide/framework/template/)。

注意

属性和样式不能混用，不能在属性字段中进行样式设置。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html\#data-%E5%B1%9E%E6%80%A7) data 属性

给组件绑定 data 属性，然后运行时通过 `dataset` 获取，方便进一步判断。

**示例：**

```
<template>
  <div>
    <div id="elNode1" data-person-name="Jack"></div>
  </div>
</template>

<script>
  export default {
    onReady () {
      const el = this.$element('elNode1')
      const elData = el.dataset.personName
      console.info(`输出data属性： ${elData}`)
    }
  }
</script>

```

←
[背景图样式](https://iot.mi.com/vela/quickapp/zh/components/general/background-img-styles.html)[通用事件](https://iot.mi.com/vela/quickapp/zh/components/general/events.html)
→


快速导航

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")

[常规属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html#%E5%B8%B8%E8%A7%84%E5%B1%9E%E6%80%A7 "常规属性")

[渲染属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html#%E6%B8%B2%E6%9F%93%E5%B1%9E%E6%80%A7 "渲染属性")

[data 属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html#data-%E5%B1%9E%E6%80%A7 "data 属性")