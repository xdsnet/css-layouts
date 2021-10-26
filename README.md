# css-layouts

css经典布局的实现记录
参考：
[只要一行代码，实现五种 CSS 经典布局](https://www.ruanyifeng.com/blog/2020/08/five-css-layouts-in-one-line.html) 和
[1-Line Layouts*](https://1linelayouts.glitch.me/)


# Edge Firefox Chrome Safari 均支持的布局效果
* [居中、起始、末尾对齐布局](./SuperCentered.html)，关键是`place-items: center` 
* [多栏并列布局](./TheDeconstructedPancake.html),关键是`flex: 0 1 <baseWidth>`
* [两栏分区布局](./SidebarSays.html),关键是`grid-template-columns: minmax(<min>, <max>) ...`
* [上中下三明治布局](./PancakeStack.html),关键是`grid-template-rows: auto 1fr auto`
* [圣杯布局](./ClassicHolyGrail.html),关键是`grid-template: auto 1fr auto / auto 1fr auto`
* [12列网格布局模板](./SpanGrid12.html),关键是`grid-template-columns: repeat(12, 1fr)`
* [子元素有最小宽度的多栏并列布局](./RAM.html),关键是`grid-template-columns: repeat(auto-fit, minmax(<base>, 1fr))`
* [多并列卡片布局](./LineUp.html),关键是`justify-content: space-between`

# Edge Firefox Chrome 支持,Safari 不支持的布局效果
* [自定义紧扣风格](./Clamping.html),关键是`clamp(<min>, <actual>, <max>)`