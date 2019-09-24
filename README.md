## scss 常用清单

### mixin

#### border

补充不能设置单边的圆角

- border-top-radius($radius)
- border-bottom-radius($radius)
- border-right-radius($radius)
- border-left-radius($radius)

#### clearfix

清浮动

- clearfix

#### color

生成颜色类

- make-background-color($colorMap) 生成背景色的类     `.x-bg-c-${name}`
- make-font-color($colorMap)       生成字体颜色类     `.x-font-c-${name}`
- make-button-color($colorMap)     生成按钮颜色类     `.x-btn-c-${name}`
- make-tr-color($colorMap)         生成表格行颜色类   `.x-btn-c-${name}`

#### ellipsis

设置文字截断方式

- ellipsis($lines, $substract)   截断的行数，以及最后缩进距离

#### position

设置元素定位

- position($type, $top, $left, $bottom, $right)          设置元素定位以及各个方向上的偏移量

#### size

设置元素大小

- size($width, $height: $width)     矩形元素
- circle($size)                     [椭]圆形元素

### class

#### button

定义 `button` 需要手动引入 `_buttonGroup.scss` 与 `_button.scss` 文件

- btn
- btn-group
- btn-group-vertical
- btn-group-justified

#### flex

- x-flex                  生成 `flex` 容器
- 定义主轴方向
  - x-m-l2r               主轴从左到右
  - x-m-r2l               主轴从右到左
  - x-m-t2b               主轴从上到下
  - x-m-b2t               主轴从下到上
- 定义内容在主轴上的呈现效果
  - x-m-start
  - x-m-end
  - x-m-center
  - x-m-around
  - x-m-between
  - x-m-evenly            以上为 `justify-content` 的缩写
  - x-m-avg               内容完全平分空间
- 定义内容在交叉轴上的呈现效果
  - x-a-start
  - x-a-end
  - x-a-baseline
  - x-a-stretch           以上为 `align-items` 的缩写
- 定义多行容器，已经换行规则（定义交叉轴方向）
  - x-a-t2b               交叉轴由上到下（从上到下换行）
  - x-a-b2t               交叉轴由下到上（从下到上换行）
- 容器行在交叉轴上的空间分配
  - x-r-start
  - x-r-end
  - x-r-center
  - x-r-around
  - x-r-between
  - x-r-evenly
  - x-r-stretch           以上为 `align-content` 的缩写

#### simple-class

一些常用的类名

- x-b-c                   块居中
- x-t-c                   文字居中
- x-t-r                   文字右排
- x-t-l                   文字左排
- x-f-l                   块左浮动
- x-f-r                   块右浮动
- x-p-r                   相对定位元素
- x-[pm]-[tblr]-[5-30]    提供 `5 - 30` 的 `padding/margin` 各个方向上的简写
- x-font-s-[12-30]           提供 `12 - 30` 双字号的简写
- x-ellipsis              单行文字溢出 `...`


