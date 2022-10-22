- [一、标题](#一标题)
  - [1.1 常用语法](#11-常用语法)
  - [1.2 可选语法](#12-可选语法)
  - [1.3 自定义标题id](#13-自定义标题id)
- [二、段落、换行](#二段落换行)
  - [2.1 段落](#21-段落)
  - [2.2 换行](#22-换行)
- [三、各类样式](#三各类样式)
  - [3.1 斜体](#31-斜体)
  - [3.2 粗体](#32-粗体)
  - [3.3 粗斜体](#33-粗斜体)
  - [3.4 下划线](#34-下划线)
  - [3.5 删除线](#35-删除线)
  - [3.6 字体](#36-字体)
  - [3.7 字体大小](#37-字体大小)
  - [3.8 字体颜色](#38-字体颜色)
  - [3.9 上下标](#39-上下标)
  - [3.10 高亮](#310-高亮)
  - [3.11 居中](#311-居中)
- [四、列表](#四列表)
  - [4.1 有序列表](#41-有序列表)
  - [4.2 无序列表](#42-无序列表)
    - [4.2.1 ToDo](#421-todo)
  - [4.3 列表嵌套](#43-列表嵌套)
- [五、引用](#五引用)
  - [5.1 语法](#51-语法)
  - [5.2 多段引用](#52-多段引用)
  - [5.3 引用嵌套](#53-引用嵌套)
- [六、分割线](#六分割线)
- [七、代码块](#七代码块)
  - [7.1 行内代码](#71-行内代码)
  - [7.2 代码块](#72-代码块)
  - [7.3 围栏式代码块](#73-围栏式代码块)
- [八、表格](#八表格)
  - [8.1 表格使用](#81-表格使用)
  - [8.2 表格对齐方式](#82-表格对齐方式)
- [九、超链接](#九超链接)
  - [9.1 使用超链接](#91-使用超链接)
    - [9.1.1 链接到网站](#911-链接到网站)
    - [9.1.2 链接到其他 Markdown 页面](#912-链接到其他-markdown-页面)
    - [9.1.3 无标签链接](#913-无标签链接)
    - [9.1.4 有 title 的链接](#914-有-title-的链接)
  - [9.2 和其他元素配合](#92-和其他元素配合)
  - [9.3 自动超链接](#93-自动超链接)
- [十、添加目录](#十添加目录)
  - [10.1 TOC](#101-toc)
  - [10.2 自动添加目录](#102-自动添加目录)
  - [10.3 手动添加目录](#103-手动添加目录)
- [十一、图片](#十一图片)
  - [11.1 添加图片](#111-添加图片)
  - [11.2 带title的图片](#112-带title的图片)
  - [11.3 带链接的图片](#113-带链接的图片)
- [十二、注释、脚注](#十二注释脚注)
  - [12.1 注释](#121-注释)
  - [12.2 脚注](#122-脚注)
  - [12.3 行内脚注](#123-行内脚注)
- [十三、公式](#十三公式)
  - [13.1 行内公式](#131-行内公式)
  - [13.2 块公式](#132-块公式)
- [十四、图表](#十四图表)
  - [14.1 流程图](#141-流程图)
    - [14.1.1 线形](#1411-线形)
  - [14.2 饼图](#142-饼图)
  - [14.3 甘特图](#143-甘特图)
- [十五、Emoji表情](#十五emoji表情)
# 一、标题
## 1.1 常用语法
Markdown 的标题和 HTML 的标题一致，分为 6 级。分别在开头放 1 到 6 个 `#` 加空格再加标题内容。`<h1>标题 1</h1>`
## 1.2 可选语法
题内容的后面如果也存在空格和 `#`，也可以构成标题，且标题的级别以前面 `#` 的数量为准。  
标题 1 和标题 2 也可以用下面加横线的形式。标题下面加等号 `=` 会生成标题 1，加减号 `-` 会生成标题 2。等号和减号的数量一般不限制，可以有一个或多个。
## 1.3 自定义标题id
再标题后加花括号`# 标题 {#head}`。`<h1 id="head1">标题 1</h1>`
| Markdown        | 可选语法1             | 可选语法2           | 自定义标题id             | 预览                       |
| --------------- | --------------------- | ------------------- | ------------------------ | -------------------------- |
| `# 标题 1`      | `# 标题 1 ###`        | `标题 1`<br/> `===` | `# 标题 1 {#head1}`      | <h1>标题 1</h1>            |
| `## 标题 2`     | `## 标题 2 ####`      | `标题 2`<br/>`---`  | `## 标题 2 {#head2}`     | <h2>标题 2</h2>            |
|                 |                       |                     | `#### 标题内容 {#head?}` | <h4 id="head4">标题 4</h4> |
| `###### 标题 6` | `####### 标题6 #####` | 只能生成两个        | `###### 标题 6 {#head6}` | <h6 id="head6">标题 6</h6> |

# 二、段落、换行
## 2.1 段落
在 Markdown 里面直接顶行写一些文本就会生成段落，各个段落之间以空行分割。`<p>...</p>`
## 2.2 换行
在一行文本后面添加两个以上空格 *(通常还会加上回车来方便观看)*，引擎会生成换行符 `<br/>`，同样的也可以手写 `<br/>` 实现换行，段落文本区域1后面有两个空格。`<p>这是一段文本 1<br/>这是一段文本 2</p>`
| Markdown                                 | 预览                              |
| ---------------------------------------- | --------------------------------- |
| `段落文本区域`                           | 段落文本区域                      |
| `段落文本区域1  ` `回车` `段落文本区域2` | 段落文本区域1 <br/> 段落文本区域2 |


# 三、各类样式
## 3.1 斜体
在需要加粗的文本前后添加两个星号 `*` 或下划线 `_` 可以倾斜文本。`<em>这是斜体</em>`
## 3.2 粗体
在需要加粗的文本前后添加两个星号 `*` 或下划线 `_` 可以对文本加粗。`<strong>这是粗体</strong>`
## 3.3 粗斜体
在需要加粗斜体的文本前后添加三个星号 `*` 或下划线 `*` 可以倾斜并加粗文本,或者两者混合使用。`<strong><em>这是粗斜体</em></strong>`
## 3.4 下划线
由于 Markdown 无下划线语法，但支持 HTML 语言，可以向文本添加下划线。`<u>这是下划线</u>`
## 3.5 删除线
在需要删除线的文本前后添加两个波浪 `~`。`<s>带删除线的字</s>`  
| Markdown            | 预览                                 |
| ------------------- | ------------------------------------ |
| `_这是斜体_`        | <em>这是斜体</em>                    |
| `*这是斜体*`        |                                      |
| `**这是粗体**`      | <strong>这是粗体</strong>            |
| `__这是粗体__`      |                                      |
| `**_这是粗斜体_**`  | <strong><em>这是粗斜体</em></strong> |
| `__*这是粗体*__`    |                                      |
| `___这是粗斜体___`  |                                      |
| `***这是粗斜体***`  |                                      |
| `<u>这是下划线</u>` | <u>这是下划线</u>                    |
| `~~带删除线的字~~`  | <s>带删除线的字</s>                  |
> 以下都不怎么支持简单编写
## 3.6 字体
字体类型的设置只能在电脑上才能显示字体效果，在手机上无法显示字体类型。  
```
<font face="黑体">黑体</font>  
<font face="宋体">宋体</font>  
<font face="仿宋">仿宋</font>  
<font face="楷书">楷书</font>  
```
<font face="黑体">黑体</font>  
<font face="宋体">宋体</font>  
<font face="仿宋">仿宋</font>  
<font face="楷书">楷书</font>  

## 3.7 字体大小
`size`：规定文本的尺寸大小，取值范围为 `1~7` ，浏览器默认值是 `3` 。注意，`size=50` 也是可以显示的，但与`7`的字体大小一样。  
```
<font size=1>字体大小size=1</font>  
<font size=4>字体大小size=4</font>  
<font size=7>字体大小size=7</font>  
<font size=50>字体大小size=50</font>  
```
<font size=1>字体大小size=1</font>  
<font size=4>字体大小size=4</font>  
<font size=7>字体大小size=7</font>  
<font size=50>字体大小size=50</font>  

## 3.8 字体颜色
要写带颜色的字需要这样一句 `$\color{颜色对应的英文}{想要变色的内容}$` 或者是 `$\color{颜色对应的十六进制值}{想要变色的内容}$`  
> 同样的如果用 HTML 编写也是可以的。`<font color=red>红色</font>` 或是 `<font color=#ff0000>红色</font>`
```
$\color{red}{红色字}$  
$\color{green}{绿色字}$  
$\color{#00dd00}{浅绿色字}$  
$\color{#660066}{深紫色字}$  
<font color=YellowGreen>黄绿色字</font>  
<font color=#0000ff>蓝色字</font>
```
$\color{red}{红色字}$  
$\color{green}{绿色字}$  
$\color{#00dd00}{浅绿色字}$  
$\color{#660066}{深紫色字}$  
<font color=YellowGreen>黄绿色字</font>  
<font color=#0000ff>蓝色字</font>

## 3.9 上下标
在需要上下标的字符，上标用 `^` 包围，下表用 `~` 包围。
```
a^2^x+bx+c=0
H~2~O
```
a^2^x+bx+c=0  
H~2~O  
> 上下标并非所有 Markdown 解析器都支持。
## 3.10 高亮
在需要高亮的字符以 `==` 包围。
```
==高亮字==
```
==高亮字==
> 高亮并非所有 Markdown 解析器都支持。
## 3.11 居中
在需要居中的字符以 `<center>` 包围。`<center>...</center>`  
```
<center>居中的字样</center>
```
<center>居中的字样</center>


# 四、列表
## 4.1 有序列表
在文本前面添加数字加点加空格可以构成有序列表。如下表，最终生成的列表前面的编号和前面的数字没有绝对关系，总是从第一个数字开始依次增加。  
## 4.2 无序列表
无序列表可以在文本前面加减号 `-` 、星号 `*` 、加号 `+` 实现。  
### 4.2.1 ToDo
在无序列表 `-,+,*`  后面使用 `「中括号 []」 `声明复选框。在中括号中写入 `x` ，便可实现选中效果。
- [ ] 未选中  
- [x] 以选中  
```javascript
<ul>
<li class="task-list-item"><input type="checkbox" disabled=""> 未选中</li>
<li class="task-list-item"><input type="checkbox" disabled="" checked=""> 以选中</li>
</ul>
```
| Markdown                                  | 预览                                                          |
| ----------------------------------------- | ------------------------------------------------------------- |
| `1. 有序列表项 1` <br/> `2. 有序列表项 2` | <ol><li>有序列表项 1</li><li>有序列表项 2</li></ol>           |
| `1. 有序列表项 1` <br/> `1. 有序列表项 2` | <ol><li>有序列表项 1</li><li>有序列表项 2</li></ol>           |
| `3. 有序列表项 1` <br/> `6. 有序列表项 2` | <ol start="5"><li>有序列表项 1</li><li>有序列表项 2</li></ol> |
| `- 无序列表项 1` <br/> `- 无序列表项 2`   | <ul><li>无序列表项 1</li><li>无序列表项 2</li></ul>           |
| `* 无序列表项 1` <br/> `* 无序列表项 2`   | <ul><li>无序列表项 1</li><li>无序列表项 2</li></ul>           |
| `+ 无序列表项 1` <br/> `+ 无序列表项 2`   | <ul><li>无序列表项 1</li><li>无序列表项 2</li></ul>           |
## 4.3 列表嵌套
有序列表、无序列表是可以嵌套的，单一嵌套和混合嵌套都可以。在列表项前面添加两个以上空格或制表符可以把该行变成子列表 **(实际使用时最好用制表符)**。  
1. 有序列表 1
   1. 有序列表 2 
      - 无序列表 1 
        - 无序列表 2
   1. 有序列表 3
2. 有序列表 4


# 五、引用
## 5.1 语法
在需要引用的语句前，可以使用大于号 `>` 和`空格`生成引用。`<blockquote>...</blockquote>`  
`> 这里是个引用` 效果如下：
> 这里是个引用
## 5.2 多段引用
在需要引用的段落前全部加上大于号 `>` 和`空格`。
```
> 这是一个引用段落
>
> 这是另一个引用段落
```
> 这是一个引用段落
>
> 这是另一个引用段落
## 5.3 引用嵌套
只需要在引用里面加引用即可实现。
```
> 这是一个引用
> > 这是一个嵌套引用
```
> 这是一个引用
> > 这是一个嵌套引用


# 六、分割线
一行只存在连续三个或以上星号 `*` 、减号 `-` 或下划线 `_` 会被生成分隔线。 `<hr/>`  
分割线上下都会形成一行空白行。
```
---
***
___
```


# 七、代码块
## 7.1 行内代码
使用一对反引号 `` ` `` 来创建行内代码。如果在行内代码中需要包含反引号本身，可以使用两个反引号对加前后空格来创建。`<code>...</code>`  
| Markdown             | 预览           |
| -------------------- | -------------- |
| `` 这是行内`代码` `` | 这是行内`代码` |
| ``` `` ` `` ```      | `` ` ``        |
## 7.2 代码块
将文本的每一行缩进至少四个空格或一个制表符。这样这些文本会变成代码块。
```
    <html>
        <head></head>
    </html>
```
    <html>
        <head></head>
    </html>
## 7.3 围栏式代码块
使用三个反引号`` ` ``或三个波浪号`~`来定义围栏式代码块。  
> 如果在代码块中也存在三个反引号或波浪号，可以在外层使用 4 个。  
> 在第一个标识处后添加所属代码语言，后面的代码会高亮。
````
```C++
#include <iostream>
using namespace std;

int main()
{
	cout << "Hello World" << endl;
	return 0;
}
```
````
```C++
#include <iostream>
using namespace std;

int main()
{
	cout << "Hello World" << endl;
	return 0;
}
```


# 八、表格
## 8.1 表格使用
表格使用竖线 `|` 区分每一列，在表格头和表格体之间第列使用至少三个减号 `-` 来做为分隔。
```
| 第一列       | 第二列       | 第三列       |
| ------------ | ------------ | ------------ |
| 第一行第一列 | 第一行第二列 | 第一行第三列 |
| 第二行第一列 | 第二行第二列 | 第二行第三列 |
```
| 第一列       | 第二列       | 第三列       |
| ------------ | ------------ | ------------ |
| 第一行第一列 | 第一行第二列 | 第一行第三列 |
| 第二行第一列 | 第二行第二列 | 第二行第三列 |
## 8.2 表格对齐方式
在第二行的每一列都添加了冒号 `:` ，左侧添加一个冒号表示该列左对齐，右侧添加一个冒号表示该列右对齐，左右各添加一个冒号表示该列居中对齐。
```
| 这是第一列 | 这是第二列 | 这是第三列 |
| :--------- | :--------: | ---------: |
| 左对齐     |    居中    |     右对齐 |
```
| 这是第一列 | 这是第二列 | 这是第三列 |
| :--------- | :--------: | ---------: |
| 左对齐     |    居中    |     右对齐 |


# 九、超链接
## 9.1 使用超链接
在 Markdown 里可以创建超链接，以链接到其他 Markdown 页面或网站。
### 9.1.1 链接到网站
```
[Spray-echo/Markdown](https://github.com/Spray-echo/Markdown)
```
[Spray-echo/Markdown](https://github.com/Spray-echo/Markdown)
### 9.1.2 链接到其他 Markdown 页面
```
[Marakdown 标题](#一标题)
```
[Marakdown 标题](#一标题)  
### 9.1.3 无标签链接
```
<https://github.com/Spray-echo/Markdown>
```
<https://github.com/Spray-echo/Markdown>
### 9.1.4 有 title 的链接
```
[Spray-echo/Markdown](https://github.com/Spray-echo/Markdown "跳转Markdown")
[Marakdown 标题](#一标题 "跳转到标题")  
```
[Spray-echo/Markdown](https://github.com/Spray-echo/Markdown "跳转Markdown")  
[Marakdown 标题](#一标题 "跳转到标题")  
## 9.2 和其他元素配合
```
这是一个[**粗体链接**](#32-粗体)
这是一个[_斜体链接_](#31-斜体)
这是一个[**_粗斜体链接_**](#33-粗斜体)
这是一个[`在代码里面的链接`](#七代码块)
```
这是一个[**粗体链接**](#32-粗体)  
这是一个[*斜体链接*](#31-斜体)  
这是一个[***粗斜体链接***](#33-粗斜体)  
这是一个[`在代码里面的链接`](#七代码块)
## 9.3 自动超链接
有些 Markdown 解析器还可以自动解析代码中的链接，并生成无标签链接。  
若不想链接则可以放入代码块中`https://github.com/Spray-echo/Markdown`


# 十、添加目录
## 10.1 TOC
在 Markdown 中，自动生成目录非常简单，只需要在恰当的位置添加 `[toc]` 符号，凡是以 `#` 定义的标题都会被编排到目录中。  
> 如果想要在 TOC 中排除一个标题，在标题后面添加 {ignore=true} 即可。  
> 部分地方不支持
## 10.2 自动添加目录
> `vscode-Markdown All in One` 插件， 可以直接生成目录， 内容和手写目录基本一样, 插件生成目录：   
> `Ctrl + Shift + P` -> `markdown all in one create table of contents`（该方案会生成所有的标题目录，并按标题等级生成无序列表目录）
## 10.3 手动添加目录
手动添加目录的方法就是将「列表」和「页内超链接」相结合，通常与无序列表结合使用。`- [目录名](#标题链接)`  
标题链接中不能出现大写字母，大写字母用小写字母代替  
标题链接中不能出现空格 ` ` ，空格用 `-` 代替。  
标题链接中若出现符号，则省略不写，如本标题：`## 10.3 手动添加目录` 写成 `- [10.3 手动添加目录](#103-手动添加目录)`。  
> 以本文档的部分标题举例
```Markdown
- [九、超链接](#九超链接)
  - [9.1 使用超链接](#91-使用超链接)
    - [9.1.1 链接到网站](#911-链接到网站)
    - [9.1.2 链接到其他 Markdown 页面](#912-链接到其他-markdown-页面)
    - [9.1.3 无标签链接](#913-无标签链接)
    - [9.1.4 有 title 的链接](#914-有-title-的链接)
  - [9.2 和其他元素配合](#92-和其他元素配合)
  - [9.3 自动超链接](#93-自动超链接)
```


# 十一、图片
## 11.1 添加图片
下面的代码，在生成超链接的代码前面添加一个感叹号 `!` ，同时把链接换成图片地址。`![图片名字](图片地址)`  
```
![这是一个图片](/resource/test.jpg)
```
![这是一个图片](http://png.eot.ooo/i/2022/10/22/63535ec8d3442.jpeg)
## 11.2 带title的图片
```
![这是一个图片](/resource/test.jpg "这是一个好看的图片")
```
![这是一个图片](http://png.eot.ooo/i/2022/10/22/63535ec8d3442.jpeg "这是一个好看的图片")
## 11.3 带链接的图片
把生成图片的代码放到了超链接的名称里面。
```
[![这是一个图片](http://png.eot.ooo/i/2022/10/22/63535ec8d3442.jpeg)](http://png.eot.ooo/i/2022/10/22/63535ec8d3442.jpeg "图片所在位置")
```
[![这是一个图片](http://png.eot.ooo/i/2022/10/22/63535ec8d3442.jpeg)](http://png.eot.ooo/i/2022/10/22/63535ec8d3442.jpeg "图片所在位置")
> **注意**：填写本地图片地址时要用相对地址，绝对地址测试不行。  
> > Markdown所在位置 `/test/test1/README.md`   
> > 图片所在位置 `/test/test1/resource/test.jpg` 和 `/test/test2/resource/test.jpg`  
> > > 访问下级目录可以直接输入本级目录以后的地址 `/resource/test.jpg`  
> > > 访问上级目录可以在前方加两个 `.` ，`../test2/resource/test.jpg`  


# 十二、注释、脚注
## 12.1 注释
Markdown 本身是不支持注释的，但大部分的 Markdown 编辑器或解析器是支持 HTML 的，可以使用 HTML 的注释来做到 Markdown 注释的效果。
```
注释内容将会被隐藏，<!-- 注释内容 -->体现在文字中像这样。

或者是一种可以被展开的注释
<details>
<summary>点击查看</summary>
  这里是隐藏的内容
</details>

```
注释内容将会被隐藏：<!-- 注释内容 -->体现在文字中像这样。
<details>
<summary>点击查看</summary>
  这里是隐藏的内容
</details>

## 12.2 脚注
脚注类似于参考文献或补充说明，统一出现的文档的最后，可在文中任意位置引用。  
脚注的定义语法为： `[^名称]: 内容` : `[^1]: 引用的脚注的具体内容.`   
脚注的引用语法为：`[^名称]` : `[^1]`[^1]比如上面的`1`就是引用的脚注，点击可以跳转到下面的脚注内容。  
## 12.3 行内脚注
行内脚注 `^[行内脚注]` ^[这是一个行内脚注]不需要显式声明，只要在需要脚注的地方直接使用就可以，解析器会把内容提取出来放到文末。
> 脚注并非所有 Markdown 解析器都支持。  


# 十三、公式
## 13.1 行内公式
行内公式前后各使用一个 `$` 包裹，渲染结果和行内代码类似，在行内显示，不换行。
```
这是一个行内公式: $a^2 = b^2 + c^2$
```
这是一个行内公式: $a^2 = b^2 + c^2$  
## 13.2 块公式
块公式前后各使用两个 `$` 包裹，渲染结果和代码块一样，独占一行。
```
$$
f(x) = \int_{-\infty}^\infty
    \hat{f}(\xi)\,e^{2 \pi i \xi x}\,d\xi
$$
```
$$
f(x) = \int_{-\infty}^\infty
    \hat{f}(\xi)\,e^{2 \pi i \xi x}\,d\xi
$$
> 公式的语法可以参考[LaTex语法](https://webdemo.myscript.com/views/math/index.html "这是个直接转换的网站")。


# 十四、图表
## 14.1 流程图
````
```flow
st=>start: 开始
op=>operation: 操作
cond=>condition: 判断
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
```
````
```flow
st=>start: 开始
op=>operation: 操作
cond=>condition: 判断
e=>end: 结束

st->op->cond
cond(yes)->e
cond(no)->op
```

````
```mermaid
flowchart LR
    A[直角矩形] -->|链接文本| B(圆角矩形)
    B --> C{选择}
    C -->|一| D[结果一]
    C -->|二| E[结果二]
```
````
```mermaid
flowchart LR
    A[直角矩形] -->|链接文本| B(圆角矩形)
    B --> C{选择}
    C -->|一| D[结果一]
    C -->|二| E[结果二]
```
> 其中 `flowchart LR` 为横从左到右向放置，`flowchart TB` 为纵向从上到下放置 `RL` 、 `BT` 实现反向。  
> 其中 `flowchart` 也可以用 `graph` 替代。

### 14.1.1 线形
````
```mermaid
graph TB
  A1 --> B1
  A2 --- B2
  A3 -- 描述 --- B3
  A4 -- 描述 --> B4
  A5 -.- B5
  A6 -.-> B6
  A7 -. 描述 .- B7
  A8 -. 描述 .-> B8
  A9 === B9
  A10 ==> B10
  A11 == 描述 === B11
  A12 == 描述 ==> B12
​```
````

```mermaid
graph TB
  A1 --> B1
  A2 --- B2
  A3 -- 描述 --- B3
  A4 -- 描述 --> B4
  A5 -.- B5
  A6 -.-> B6
  A7 -. 描述 .- B7
  A8 -. 描述 .-> B8
  A9 === B9
  A10 ==> B10
  A11 == 描述 === B11
  A12 == 描述 ==> B12
```

## 14.2 饼图
````
```mermaid
pie
    title 饼图名称
    "类别A" : 386
    "类别B" : 85
    "类别C" : 150 
```
````
```mermaid
pie
    title 饼图名称
    "类别A" : 386
    "类别B" : 85
    "类别C" : 150 
```
## 14.3 甘特图
````
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       甘特图名称
    
    section 类别A
    已经完成的任务    :         done,     des1,   2014-01-06,  2014-01-08
    进行中的任务      :         active,   des2,   2014-01-09,  3d
    未来的任务        :                   des3,   after des2,  5d

    section 类别B
    完成的关键任务    :crit,    done,             2014-01-06,  24h
    进行中的关键任务  :crit,    active,                        3d
    将来的关键任务    :crit,                                   5d
```
````
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       甘特图名称
    
    section 类别A
    已经完成的任务    :         done,     des1,   2014-01-06,  2014-01-08
    进行中的任务      :         active,   des2,   2014-01-09,  3d
    未来的任务        :                   des3,   after des2,  5d

    section 类别B
    完成的关键任务    :crit,    done,             2014-01-06,  24h
    进行中的关键任务  :crit,    active,                        3d
    将来的关键任务    :crit,                                   5d
```
> 需要更详细的图表画法可以参考[这篇文章](https://blog.csdn.net/qq_32708605/article/details/123801702 "CSDN的文章")。


# 十五、Emoji表情
在 Markdown 里使用 Emoji 表情有两种方法，一种是直接输入 Emoji 表情，另一种是使用 [Emoji 表情短码](https://www.emojiall.com/zh-hans/help-shortcode "点击查看") `emoji shartcodes`。  
Emoji 表情短码放到两个冒号 `:` 之间，比如： `:joy:` :joy: `:smile:` :smile:  


[^1]: 引用的脚注的具体内容.
