                          Web前端代码规范
1.HTML
原则
1.规范 。保证您的代码规范，保证结构表现行为相互分离。
2.简洁。保证代码的最简化，避免多余的空格、空行，保持代码的语义化，尽量使用具有语义的元素，避免使用样式属性和行为属性。任何时候都要用尽量简单、尽量少的元素解决问题。
3.实用。遵循标准，但是不能以牺牲实用性为代价。
4.忠诚。选择一套规范，然后始终遵循。不管代码由多少人参与，都应该看起来像一个人写的一样

语法
1.小写. html标签、属性全部小写。
2.嵌套. 所有元素必须正确嵌套。
3.闭合. 双标签必须闭合，单标签（自关闭标签）不闭合 如 <hr>。
4.双引号. 双引号属性值，不要使用单引号。

注释
1.详尽注释。解释代码解决问题、解决思路等。
2.模块注释。建议不使用模块结束注释。

文档
1.文档类型使用html5标准文档类型，文档类型声明之前，不允许出现任何非空字符。不允许添加<meta>强制改变文档模式。
2.html元素上指定lang属性。显示页面语言，有助于语言合成工具来确定怎样发音，以及翻译工具决定使用的规则，等等。
3.指定明确的字符编码。让浏览器轻松、快速的确定适合网页内容的渲染方式。

属性
1.双引号属性值，不要使用单引号。
2.省略type属性。使用style、link、script，不用指定type属性，因为 text/css 和 text/javascript 分别是他们的默认值。
3.省略Boolean属性值。Boolean属性不用添加取值，disabled,checked,selected等。
4.省略url类属性资源协议头。
5.属性顺序。html属性应该按照特定的顺序出现以保证易读性。class->id,name->data-*->src,for,type,href->title,alt->aria-*,role。
6.多媒体元素添加替代属性。图像增加alt属性，音视频增加替代文字。

元素
1.避免冗余标签。
2.避免JS生成标签。
3.段落文字应该用p，避免使用br。
4.列表项放ul,ol,dl,不要使用一系列的div或p。
5.input使用for属性绑定label。
6.使label标签包裹radio或checkbox和他们的文字，不用再使用for属性。
8.form button应制定type类型，使用type="submit"、type="reset"或type="button"。

参考: http://www.php100.com/html/it/qianduan/2015/0116/8389.html

CSS

全局：global.css

全局样式为全站公用，为页面样式基础，页面中必须包含。

结构：layout.css

页面结构类型复杂，并且公用类型较多时使用。多用在首页级页面和产品类页面中。

私有：style.css

独立页面所使用的样式文件，页面中必须包含。

模块 module.css

产品类页面应用，将可复用类模块进行剥离后，可与其它样式配合使用。

主题 themes.css

实现换肤功能时应用。

补丁 mend.css 基于以上样式进行的私有化修补。

CSS命名规范
头：header
内容：content/containe
尾：footer
导航：nav
侧栏：sidebar
栏目：column
页面外围控制整体布局宽度：wrapper
左右中：left right center
登录条：loginbar
标志：logo
广告：banner
页面主体：main
热点：hot
新闻：news
下载：download
子导航：subnav
菜单：menu
子菜单：submenu
搜索：search
友情链接：friendlink
页脚：footer
版权：copyright
滚动：scroll
内容：content
标签页：tab
文章列表：list
提示信息：msg
小技巧：tips
栏目标题：title
加入：joinus
指南：guild
服务：service
注册：regsiter
状态：status
投票：vote
合作伙伴：partner

1.命名统一采用小写
注意事项::
一律小写;
尽量用英文;
不加中杠和下划线;
尽量不缩写，除非一看就明白的单词.

class的命名:

(1)颜色:使用颜色的名称或者16进制代码,如
.red { color: red; }
.f60 { color: #f60; }
.ff8600 { color: #ff8600; }

（2）字体大小,直接使用”font+字体大小”作为名称,如
.font12px { font-size: 12px; }
.font9pt {font-size: 9pt; }

(3)对齐样式,使用对齐目标的英文名称,如
.left { float:left; }
.bottom { float:bottom; }

(4)标题栏样式,使用”类别+功能”的方式命名,如
.barnews { }
.barproduct { }


XHTML文件中id的命名

(1)页面结构
容器: container
页头：header
内容：content/container
页面主体：main
页尾：footer
导航：nav
侧栏：sidebar
栏目：column
页面外围控制整体布局宽度：wrapper
左右中：left right center 
(2)导航
导航：nav
主导航：mainbav
子导航：subnav
顶导航：topnav
边导航：sidebar
左导航：leftsidebar
右导航：rightsidebar
菜单：menu
子菜单：submenu
标题: title
摘要: summary 
(3)功能
标志：logo
广告：banner
登陆：login
登录条：loginbar
注册：regsiter
搜索：search
功能区：shop
标题：title
加入：joinus
状态：status
按钮：btn
滚动：scroll
标签页：tab
文章列表：list
提示信息：msg
当前的: current
小技巧：tips
图标: icon
注释：note
指南：guild
服务：service
热点：hot
新闻：news
下载：download
投票：vote
合作伙伴：partner
友情链接：link
版权：copyright

参考：http://www.qianduan.net/css-selectors-naming-2/

Javascript:
使用驼峰标记法
首字母是小写的，接下来的字母都以大写字符开头。例如：
var testValue = 0, secondValue = "hi";

不要使用 switch
switch 在所有的编程语言中都是个非常错误的难以控制的语句，建议用 if else 来替换它。

操作符（+，-，*，/，%）前后请加空格
例如
return x + y;

缩进
使用两个空格来代替tab

字符串
统一使用单引号(‘)，不使用双引号(“)。这在创建 HTML 字符串非常有好处：

三元条件判断（if 的快捷方法）
用三元操作符分配或返回语句。在比较简单的情况下使用，避免在复杂的情况下使用。没人愿意用 10 行三元操作符把自己的脑子绕晕。

不推荐
if(x === 10) {
  return 'valid';
} else {
  return 'invalid';
}
推荐
return x === 10 ? 'valid' : 'invalid';

澄清：分号与函数
分号需要用在表达式的结尾，而并非函数声明的结尾。区分它们最好的例子是：
var foo = function() {
  return true;
};  // semicolon here.
 
function foo() {
  return true;
}  // no semicolon here.


参考：http://www.css88.com/archives/5366
