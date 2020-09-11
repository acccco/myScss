# scss 常用清单

## 使用

## mixin

### clearfix

清浮动

- clearfix

### color

生成颜色类

| 方法 | 作用 |
| --- | --- |
| make-background-color($colorMap) | 生成背景色的类 `.x-bg-c-${name}` |
| make-font-color($colorMap) | 生成字体颜色类 `.x-font-c-${name}` |
| make-button-color($colorMap) | 生成按钮颜色类 `.x-btn-c-${name}` |
| make-tr-color($colorMap) | 生成表格行颜色类 `.x-btn-c-${name}` |

### ellipsis

设置文字截断方式

| 方法 | 作用 |
| --- | --- |
| ellipsis($lines, $substract) | 截断的行数，以及最后缩进距离 |

### position

设置元素定位

| 方法 | 作用 |
| --- | --- |
| position($type, $top, $left, $bottom, $right) | 设置元素定位以及各个方向上的偏移量

### size

设置元素大小

| 方法 | 作用 |
| --- | --- |
| size($width, $height: $width) | 矩形元素 |
| circle($width, $height: $width) | [椭]圆形元素 |

## class

### button

定义 `button` 需要手动引入 `_buttonGroup.scss` 与 `_button.scss` 文件

- btn
- btn-group
- btn-group-vertical
- btn-group-justified

#### simple-class

一些常用的类名

| 类名 | 作用 |
| --- | --- |
| x-b-c | 块居中 |
| x-t-c | 文字居中 |
| x-t-r | 文字右排 |
| x-t-l | 文字左排 |
| x-f-l | 块左浮动 |
| x-f-r | 块右浮动 |
| x-p-r | 相对定位元素 |
| x-[pm]-[tblr]-[5-30] | 提供 `5 - 30` 的 `padding/margin` 各个方向上的简写 |
| x-font-s-[12-30] | 提供 `12 - 30` 双字号的简写 |
| x-ellipsis | 单行文字溢出 `...` |


