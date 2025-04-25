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

# [\#](https://iot.mi.com/vela/quickapp/zh/components/general/color.html\#%E9%A2%9C%E8%89%B2%E9%85%8D%E7%BD%AE) 颜色配置

Vela JS 应用支持 `rgb()` and `rgba()` 颜色值设置，

开发者可参考 [MDN 文档(opens new window)](https://developer.mozilla.org/zh-CN/docs/Web/CSS/color_value) 了解更多颜色值的信息。

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/color.html\#%E9%A2%9C%E8%89%B2%E5%80%BC%E6%A0%BC%E5%BC%8F%E7%A4%BA%E4%BE%8B) 颜色值格式示例

- `'#f0f'` (#rgb)
- `'#ff00ff'` (#rrggbb)
- `'rgb(255, 0, 255)'`
- `'rgba(255, 255, 255, 1.0)'`
- `'#f0ff'` (#rgba)
- `'#ff00ff00'` (#rrggbbaa)

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/color.html\#%E9%80%8F%E6%98%8E) 透明

`rgba(0,0,0,0)` 还有另外一个简写版本：

- `'transparent'`

## [\#](https://iot.mi.com/vela/quickapp/zh/components/general/color.html\#%E9%A2%9C%E8%89%B2%E5%90%8D%E5%AD%97) 颜色名字

你也可以用下面的颜色配置：

- aliceblue (#f0f8ff)
- antiquewhite (#faebd7)
- aqua (#00ffff)
- aquamarine (#7fffd4)
- azure (#f0ffff)
- beige (#f5f5dc)
- bisque (#ffe4c4)
- black (#000000)
- blanchedalmond (#ffebcd)
- blue (#0000ff)
- blueviolet (#8a2be2)
- brown (#a52a2a)
- burlywood (#deb887)
- cadetblue (#5f9ea0)
- chartreuse (#7fff00)
- chocolate (#d2691e)
- coral (#ff7f50)
- cornflowerblue (#6495ed)
- cornsilk (#fff8dc)
- crimson (#dc143c)
- cyan (#00ffff)
- darkblue (#00008b)
- darkcyan (#008b8b)
- darkgoldenrod (#b8860b)
- darkgray (#a9a9a9)
- darkgreen (#006400)
- darkgrey (#a9a9a9)
- darkkhaki (#bdb76b)
- darkmagenta (#8b008b)
- darkolivegreen (#556b2f)
- darkorange (#ff8c00)
- darkorchid (#9932cc)
- darkred (#8b0000)
- darksalmon (#e9967a)
- darkseagreen (#8fbc8f)
- darkslateblue (#483d8b)
- darkslategrey (#2f4f4f)
- darkturquoise (#00ced1)
- darkviolet (#9400d3)
- deeppink (#ff1493)
- deepskyblue (#00bfff)
- dimgray (#696969)
- dimgrey (#696969)
- dodgerblue (#1e90ff)
- firebrick (#b22222)
- floralwhite (#fffaf0)
- forestgreen (#228b22)
- fuchsia (#ff00ff)
- gainsboro (#dcdcdc)
- ghostwhite (#f8f8ff)
- gold (#ffd700)
- goldenrod (#daa520)
- gray (#808080)
- green (#008000)
- greenyellow (#adff2f)
- grey (#808080)
- honeydew (#f0fff0)
- hotpink (#ff69b4)
- indianred (#cd5c5c)
- indigo (#4b0082)
- ivory (#fffff0)
- khaki (#f0e68c)
- lavender (#e6e6fa)
- lavenderblush (#fff0f5)
- lawngreen (#7cfc00)
- lemonchiffon (#fffacd)
- lightblue (#add8e6)
- lightcoral (#f08080)
- lightcyan (#e0ffff)
- lightgoldenrodyellow (#fafad2)
- lightgray (#d3d3d3)
- lightgreen (#90ee90)
- lightgrey (#d3d3d3)
- lightpink (#ffb6c1)
- lightsalmon (#ffa07a)
- lightseagreen (#20b2aa)
- lightskyblue (#87cefa)
- lightslategrey (#778899)
- lightsteelblue (#b0c4de)
- lightyellow (#ffffe0)
- lime (#00ff00)
- limegreen (#32cd32)
- linen (#faf0e6)
- magenta (#ff00ff)
- maroon (#800000)
- mediumaquamarine (#66cdaa)
- mediumblue (#0000cd)
- mediumorchid (#ba55d3)
- mediumpurple (#9370db)
- mediumseagreen (#3cb371)
- mediumslateblue (#7b68ee)
- mediumspringgreen (#00fa9a)
- mediumturquoise (#48d1cc)
- mediumvioletred (#c71585)
- midnightblue (#191970)
- mintcream (#f5fffa)
- mistyrose (#ffe4e1)
- moccasin (#ffe4b5)
- navajowhite (#ffdead)
- navy (#000080)
- oldlace (#fdf5e6)
- olive (#808000)
- olivedrab (#6b8e23)
- orange (#ffa500)
- orangered (#ff4500)
- orchid (#da70d6)
- palegoldenrod (#eee8aa)
- palegreen (#98fb98)
- paleturquoise (#afeeee)
- palevioletred (#db7093)
- papayawhip (#ffefd5)
- peachpuff (#ffdab9)
- peru (#cd853f)
- pink (#ffc0cb)
- plum (#dda0dd)
- powderblue (#b0e0e6)
- purple (#800080)
- rebeccapurple (#663399)
- red (#ff0000)
- rosybrown (#bc8f8f)
- royalblue (#4169e1)
- saddlebrown (#8b4513)
- salmon (#fa8072)
- sandybrown (#f4a460)
- seagreen (#2e8b57)
- seashell (#fff5ee)
- sienna (#a0522d)
- silver (#c0c0c0)
- skyblue (#87ceeb)
- slateblue (#6a5acd)
- slategray (#708090)
- snow (#fffafa)
- springgreen (#00ff7f)
- steelblue (#4682b4)
- tan (#d2b48c)
- teal (#008080)
- thistle (#d8bfd8)
- tomato (#ff6347)
- turquoise (#40e0d0)
- violet (#ee82ee)
- wheat (#f5deb3)
- white (#ffffff)
- whitesmoke (#f5f5f5)
- yellow (#ffff00)
- yellowgreen (#9acd32)

←
[通用样式](https://iot.mi.com/vela/quickapp/zh/components/general/style.html)[动画样式](https://iot.mi.com/vela/quickapp/zh/components/general/animation-style.html)
→


快速导航

[颜色值格式示例](https://iot.mi.com/vela/quickapp/zh/components/general/color.html#%E9%A2%9C%E8%89%B2%E5%80%BC%E6%A0%BC%E5%BC%8F%E7%A4%BA%E4%BE%8B "颜色值格式示例")

[透明](https://iot.mi.com/vela/quickapp/zh/components/general/color.html#%E9%80%8F%E6%98%8E "透明")

[颜色名字](https://iot.mi.com/vela/quickapp/zh/components/general/color.html#%E9%A2%9C%E8%89%B2%E5%90%8D%E5%AD%97 "颜色名字")