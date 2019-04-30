#### html简介
* 页面结构
* 标签
html中的标记就是标签
html 使用标记标签来描述网页
结构
<标签名>内容</标签名>
*属性
html标签设置属性
属性可以为htnl元素提供附加信息
属性需要设置在开始标签或自结束标签中
属性总是以名称/值对的形式出现
比如:name="value"
有些属性可以是任意值,有些则必须是指定值
* 常见属性
id 作为唯一标示,网页中不能重复出现拥有相同的class属性可以认为是一组
class属性用来为标签分组,
title属性用来指定标签的标题,指定title以后,鼠标移入元素上方时,会出现提示文字.
*注释方面的问题
格式:<!--注释内容-->
合理的使用注释可以帮助开发人员理解网页的代码
####常用标签
* <meta>
设置页面的字符集
*设置网页的描述
*设置网页的关键字
*<html>标签用于告诉浏览器这个文档中包含的信息是用html编写的
*所有的网页的内容都需要编写到html标签中,一个页面中html标签只能有一个html
*<head>标签表示网页的元数据
*<litle>标签表示网页的标题,一般会在网页的标题栏上显示
*body标签用来设置网页的主体,所有在页面中能看到的内容都应该编写到body样本
####<h1>~<h6>
一个页面只会使用一个h1标签
####<p>标签表示网页中的一个段落
*一个浏览器会在段落的前和后个加上一个换行,也就是段落会在页面中自成一行
*br换行符
*hr直线分割线
*<img>标签是图片标签,可以在页面中直接引入另一张图片,当然也可以在盒子背景下添加图片,效果一样,属性描述,src为图片存储路径,Alt为图片的描述
*标签为超链接,通过a标签可以外部跳转到其他页面
*herf指向一个了链接地址,从而跳转到其他页面
*target设置打开目标页面位置
-self
-blank
-top
-parent
#### 字体标签
*<em>和<strong>加粗
<sub>下标H2氢气 <sup>上标5<sup>3<sup> 5的3次方
<ins>下划线 <del>删除线
#### 列表
*无序 ul li
*有序 ol li
*自定义列表 dl  dt dd
#### table
使用table标签创建一个表格
*tr表示表格中的一行
*tr中可以编写一个或多个th或td
*th表示表头
*td表示表格中的一个单元格
*colspan / rowspan 合并单元格
*<caption>表头文字</caption>
##### table属性
*border
*width/height
*cellspacing单元格间距 / 
*cellpadding单元格边距
*align: left | center ｜right
*bgcolor
*border-collapse:collapse 合并边框
#### 表单
表单是用来提交信息的标签<form>表示
*属性-action 提交的地址 -method get/post 表单提交的类型
#### 表单控件
input有type属性
-text: 文本框
-password: 密码框
-submit: 提交按钮
-radio: 单选按钮 cehcked 为默认选中
-checkbox: 多选框 cehcked 为默认
-rest: 重置按钮
#### 转义字符&nbsp空格
#### 选择器{样式名: 样式值; 样式名:样式值;}
标签{color:yellow;font-size:12px;}
####书写位置
*行内样式 <p style="color;yellow;font-size:12px;"></p>不常用
*内容样式可以直接写到样式<style>标签中
<style>
p{color:yellow; font-size:12px;}
</style>
*外部样式:可以将所有的样式保存到一个外部的CSS文件中,然后通过link引入<link rel="stylesheet" type="text/css"href="style.css">
#### css选择器
选择器（selector）用于告诉浏览器：网页上的哪些元素需要设置什么样的样式
*选择器分类
*元素选择器（标签选择器），可以根据标签的名字来从页面中选取指定的元素
*语法：  标签名 {}
* 类选择器，可以根据元素的class属性值选取元素
*语法： .classname {}
ID选择器
*ID选择器，可以根据元素的id属性值选取元素。注： id是唯一的
*语法   # id { }
		交集选择器
*可以同时使用多个选择器，这样可以选择同时满足多个选择器的元素
*语法： – 选择器1选择器2{}
*并集选择器
*可以同时使用多个选择器，多个选择器将被同时应用指定的样式。用逗号隔开
*语法： 选择器1,选择器2,选择器3 {}
*后代选择器
*可以根据标签的关系，为处在元素内部的代元素设置样式。用空格隔开
8语法： 祖先元素  后代元素  后代元素 { }
8通用选择器
*可以同时选中页面中的所有元素。
*语法： * { }
#### CSS特性
*层叠性,继承性,特殊性:a标签不能继承父元素中的文字颜色
#### 常见属性
*width,height,color,background-color,font-size,text-align,textindent,font-size,font-family,font-weight,font-style,font
#### 背景图片
*background-color:	背景颜色	
*background-image:	背景图片	url(‘1.png’); 
*background-repeat: 	平铺方式	repeat | no-repeat  | repeat-x | repeat-y
*background-position:	图片位置	left | right | top | bottom | center
*background-attachment: 	背景滚动	scroll|fixed 
*background	简写	background: green url(1.jpg) no-repeat center center fixed;
#### 盒子模型的四部分
*content(内容区)
*padding(内边距)
*border(边框)
*margin(外边距)
*padding: X X X X;代表上右下左的顺序,三个值代表上 左右 下的顺序,两个值代表上下  左右的顺序,一个值就是上下左右都包裹[magin的顺序一样]
*单写padding-top;padding-left;padding-right;padding-bottom 
*border: 1px red solid;设置的是宽度,颜色,样式,-none是没边框,– dotted（点线）,
– dashed（虚线）,
– solid（实线）,
– double（双线）
##### 嵌套崩塌
*当div发生嵌套 里面div的margin-top值 直接影响到了父类
*解决方法：
*overflow:hidden
*padding 
*float
#####垂直叠加（重叠）
*当两个div发生垂直局部时，margin值没有发生累加，最终谁大取谁
*对比的是margin-bottom  和margin-top的值
#####display
*我们不能为行内元素设置width、height、margin-top和margin-bottom。
*我们可以通过修改display来修改元素的性质。
*值：
*– block：设置元素为块元素
*– inline：设置元素为行内元素
*– inline-block：设置元素为行内块元素
*– none：隐藏元素(但是不占据原先位置)
#####visibility: hidden;(透明但是占据位置)
*visbility: visible;(可见)
##### overflow
*visible：默认值
 *scroll：添加滚动条
*auto：根据需要添加滚动条
*hidden：隐藏超出盒子的内容
#### 文档流
*块状元素独占一行
*行内元素在一行上显示，如果排不下换行
*自上而下
#### 浮动
*浮动的概念 可选值: none,left,right,
*块级元素和行内元素都可以浮动,行内元素浮动之后转化为块级元素
*块级元素浮动后,宽度被内容撑开,所以应当为其指定一个宽度
##### 浮动的表现形式
* 当一个元素浮动以后，其下方的元素会上移。元素中的内容将会围绕
在元素的周围
* 浮动会使元素完全脱离文本流，也就是不再在文档中在占用位置
* 元素设置浮动以后，会一直向上漂浮直到遇到父元素的边界或者其他
浮动元素
* 元素浮动以后即完全脱离文档流，这时不会再影响父元素的高度。也
就是浮动元素不会撑开父元素.
* 浮动元素默认会变为块元素，即使设置display:inline以后其依然是个
块元素.
##### 清楚浮动
* 清除元素周围的浮动影响
* clear: both;(通常用)
#### 定位
* position 属性可以把一个元素放置到网页中任何位置
* 可选值：
* static
* relative
* absolute
* fixed
##### 1.相对定位（relative）
每个元素在页面的文档流中都有一个自然位置。相对于这个位置对元素进行移动就称为相对定位。周
围的元素完全不受此影响。
 * 当开启了相对定位以后，可以使用top、right、bottom、left四个属性对元素进行定位。
* 如果不设置元素的偏移量，元素位置不会发生改变。
* 相对定位不会使元素脱离文本流。元素在文本流中的位置不会改变。
* 相对定位不会改变元素原来的特性。
*相对定位会使元素的层级提升，使元素可以覆盖文本流中的元素 .
##### 绝对定位
绝对定位指使元素相对于html元素或离他最近的祖先定位元素进行定位.
*当开启了绝对定位以后，可以使用top、right、bottom、left四个属性对元素进行定位.
*绝对定位会使元素完全脱离文本流。
*绝对定位的块元素的宽度会被其内容撑开。
*绝对定位会使行内元素变成块元素。
8一般使用绝对定位时会同时为其父元素指定一个相对定位，以确保元素可以相对于父元素进行定位。
##### 固定定位（fixed）
固定定位的元素会被锁定在屏幕的某个位置上，当访问者滚动网页时，固定元素会在屏幕上保持不.
* 固定定位不占据原来的位置，会脱标。
* 给元素设置固定定位之后，元素位置从浏览器左上角出发。
* 可以将行内元素转换为行内块元素。
##### z-index
当元素开启定位以后就可以设置z-index这个属性
* z-index可以指定一个整数作为参数，值越大元素显示的优先级越高，也就是z-index值较大的元素会显示在网页的最上层
##### 规避脱标流
* 能用标准流（没有脱标）解决就不用浮动
* 解决不了就考虑有浮动（页面布局类型，“不完全脱标”）
* 浮动解决不了用定位（小图标，完全脱标，不影响内容）