# 适配规范
Vela OS 支持一系列适配多种屏幕的技术能力。

## 自适应布局
系统提供的容器组件均默认遵循 Flex 弹性布局规则，使用弹性布局可以实现屏幕自适应布局。
比如以下代码可以实现行内多个 item 平均分布。
```
<div>
 <text style="flex-grow: 1; background-color:aqua;">1</text>
 <text style="flex-grow: 1; background-color:yellow;">2</text>
 <text style="flex-grow: 1; background-color:red;">3</text>
</div>
```

更多说明请参考[Flex 布局示例](https://iot.mi.com/vela/quickapp/zh/guide/framework/style/page-style-and-layout.html#flex-布局示例)

## 自适应单位
在编写 UI 样式时，可以采用系统提供的自适应长度单位，包括：
  * px
  * %

### px
px 在 Vela 应用中不表示屏幕的物理像素，而是相对于项目配置基准宽度的单位，其原理类似于rem。
开发者在 manifest 文件中将 designWidth 字段配置为设计基准宽度（设计稿宽度），然后在样式描述中使用该长度单位，数值直接使用设计稿中的像素值，系统将自动计算使 Vela 应用 UI 在不同屏幕上进行等比例缩放。
```
{
 "config": {
  "designWidth": 336
 }
}
```

### 百分比%
% 表示百分比，许多样式属性可以取百分比值，经常用以根据父对象来确定大小。
比如以下代码可以实现行内多个 item 按百分比占据父容器宽度，
```
<div>
 <text style="width: 20%; background-color:aqua;">1</text>
 <text style="width: 40%; background-color:yellow;">2</text>
 <text style="width: 40%; background-color:red;">3</text>
</div>
```

## 固定长度单位[3+]
在有的布局场景下，需要使用固定长度单位，系统支持的 dp 长度单位可满足这个需求。
DP 长度单位表示设备独立像素（device-independent pixel），也叫密度无关像素，可以认为是计算机坐标系中的一个点，这个点代表一个可以由程序使用的逻辑像素，是一个近似物理尺寸的单位，其计算公式为：
```
屏幕宽度的 DP 值 = 屏幕分辨率的宽度 / DPR
元素宽/高度的 DP 值 = 元素宽/高度的物理像素数 / DPR
```

## 媒体查询
媒体查询是 CSS3 引入的一个功能，用于根据不同的屏幕尺寸和设备类型，为网页应用不同的样式。
在 Vela JS 应用中，也可以使用类似的媒体查询规范来针对不同屏幕和设备编写样式，详细介绍请参考[媒体查询](https://iot.mi.com/vela/quickapp/zh/guide/framework/style/media-query.html)。

## 获取屏幕信息
在 Vela JS 应用中，可以通过 device feature 接口获取屏幕信息，包括屏幕形状、屏幕分辨率等。根据获取到的结果可以进行相应的样式适配。
详细介绍请参考 [设备信息 device](https://iot.mi.com/vela/quickapp/zh/features/basic/device.html)
