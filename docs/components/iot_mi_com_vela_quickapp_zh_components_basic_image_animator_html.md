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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#image-animator) image-animator [2+](https://iot.mi.com/vela/quickapp/zh/guide/version/APILevel2)

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#%E6%A6%82%E8%BF%B0) 概述

图片帧动画播放器。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#%E5%AD%90%E7%BB%84%E4%BB%B6) 子组件

不支持

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#%E5%B1%9E%E6%80%A7) 属性

支持 [通用属性](https://iot.mi.com/vela/quickapp/zh/components/general/properties.html)

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| images | `Array<ImageFrame>` | - | 是 | 设置图片帧信息集合。每一帧的帧信息包含图片路径、图片大小和图片位置信息 |
| iteration | `<number>` \| `<string>` | `infinite` | 否 | 设置帧动画播放次数。number表示固定次数，infinite枚举表示无限次数播放 |
| reverse | `<boolean>` | `false` | 否 | 设置播放顺序。false表示从第1张图片播放到最后1张图片； true表示从最后1张图片播放到第1张图片 |
| fixedsize | `<boolean>` | `true` | 否 | 设置图片大小是否固定为组件大小。 true表示图片大小与组件大小一致，此时设置图片的width 、height 、top 和left属性是无效的。false表示每一张图片的 width 、height 、top和left属性都要单独设置 |
| duration | `<string>` | - | 否 | 设置单次播放时长。单位支持\[s(秒)\|ms(毫秒)\]，默认单位为ms |
| fillmode | `<string>` | `forwards` | 否 | 指定帧动画执行结束后的状态。可选项有：none：恢复初始状态。forwards：保持帧动画结束时的状态（在最后一个关键帧中定义） |

ImageFrame说明

| 名称 | 类型 | 默认值 | 必填 | 描述 |
| --- | --- | --- | --- | --- |
| src | `<uri>` | - | 是 | 图片路径 |
| width | `<length>` | 0 | 否 | 图片宽度 |
| height | `<length>` | 0 | 否 | 图片高度 |
| top | `<length>` | 0 | 否 | 图片相对于组件左上角的纵向坐标 |
| left | `<length>` | 0 | 否 | 图片相对于组件左上角的横向坐标 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#%E6%A0%B7%E5%BC%8F) 样式

支持 [通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#%E6%96%B9%E6%B3%95) 方法

支持 [通用方法](https://iot.mi.com/vela/quickapp/zh/components/general/methods.html)

| 名称 | 参数 | 描述 |
| --- | --- | --- |
| start | - | 开始播放图片帧动画。再次调用，重新从第1帧开始播放 |
| pause | - | 暂停播放图片帧动画 |
| stop | - | 停止播放图片帧动画 |
| resume | - | 继续播放图片帧 |
| getState | - | 获取播放状态。\- playing：播放中 - paused：已暂停 - stopped：已停止 |

## [\#](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html\#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81) 示例代码

```
<template>
  <div class="container">
  <image-animator class="animator" id="animator" images="{{frames}}" duration="1s" />
  <div class="btn-box">
    <input class="btn" type="button" value="start" @click="handleStart" />
    <input class="btn" type="button" value="stop" @click="handleStop" />
    <input class="btn" type="button" value="pause" @click="handlePause" />
    <input class="btn" type="button" value="resume" @click="handleResume" />
  </div>
</div>
</template>

```

```
.container {
  flex-direction: column;
  justify-content: center;
  align-items: center;
  left: 0px;
  top: 0px;
  width: 454px;
  height: 454px;
  background-color: black;
}
.animator {
  width: 70px;
  height: 70px;
}
.btn-box {
  width: 264px;
  height: 120px;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
}
.btn {
  border-radius: 8px;
  width: 120px;
  margin-top: 8px;
}

```

```
export default {
  data: {
    frames: [\
      {\
        src: "/common/asserts/001.png",\
      },\
      {\
        src: "/common/asserts/002.png",\
      },\
      {\
        src: "/common/asserts/003.png",\
      },\
      {\
        src: "/common/asserts/004.png",\
      },\
      {\
        src: "/common/asserts/005.png",\
      }\
    ],
  },
  handleStart() {
    this.$element('animator').start();
  },
  handlePause() {
    this.$element('animator').pause();
  },
  handleResume() {
    this.$element('animator').resume();
  },
  handleStop() {
    this.$element('animator').stop();
  },
};

```

←
[image](https://iot.mi.com/vela/quickapp/zh/components/basic/image.html)[progress](https://iot.mi.com/vela/quickapp/zh/components/basic/progress.html)
→


快速导航

[概述](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html#%E6%A6%82%E8%BF%B0 "概述")

[子组件](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html#%E5%AD%90%E7%BB%84%E4%BB%B6 "子组件")

[属性](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html#%E5%B1%9E%E6%80%A7 "属性")

[样式](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html#%E6%A0%B7%E5%BC%8F "样式")

[方法](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html#%E6%96%B9%E6%B3%95 "方法")

[示例代码](https://iot.mi.com/vela/quickapp/zh/components/basic/image-animator.html#%E7%A4%BA%E4%BE%8B%E4%BB%A3%E7%A0%81 "示例代码")