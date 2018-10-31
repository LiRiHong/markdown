## 通用markdown的基本语法

[toc]


### 标题

设置标题，在文字前面设置“#”就好了，一个“#”是一级标题，字体最大，越来越多“#”，标题就越来越大，最大是6级标题，6级标题字体最小。
**使用语法**："# xxx"
**快捷键：ctrl+h(headline)**

**样例**

``` markdown
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```


### 列表

#### 无序列表
无序列表单纯是分点列出效果，没有序号标记，一般是用 “·”小黑点显示。用法可以用"+","-","*"，可以简记为四则运算符号中少了“/”除号
**使用语法**：“+”/“-”/“*” 项目名
**快捷键：ctrl+u(unordered)**

**样例**

``` markdown
* 项目1
  * 子项目1.1
  * 子项目1.2
    * 子项目1.2.1
* 项目2
* 项目3

+ 项目1
  + 子项目1.1
  + 子项目1.2
    + 子项目1.2.1
+ 项目2
+ 项目3

- 项目1
  - 子项目1.1
  - 子项目1.2
    - 子项目1.2.1
- 项目2
- 项目3
```
**效果**

* 项目1
  * 子项目1.1
  * 子项目1.2
    * 子项目1.2.1
* 项目2
* 项目3

+ 项目1
  + 子项目1.1
  + 子项目1.2
    + 子项目1.2.1
+ 项目2
+ 项目3

- 项目1
  - 子项目1.1
  - 子项目1.2
    - 子项目1.2.1
- 项目2
- 项目3


#### 有序列表
有序列表是按照一定的数字顺序去列出你要陈述的点子，可以根据自己的需要自定义最开开始的序号，接下来的序号就在原来的基础上递增。比如说开始序列是1，接下来的就是2,3……等，如果开始的是59，接下来的就是60,61……。在接下来的样例中你会发现只要你的第一个点子是采用“数学”+“.”的形式，接下来的序号不管是怎么样都没所谓了，系统会自动按照最开始的序号进行自增1.
**使用语法**："数字"+"."  项目名
**快捷键：ctrl+o(ordered)**

**样例1**

``` markdown
1. 项目1
1. 项目2
3. 项目3
    1. 项目3.1
    2. 项目3.2

1. 项目1
1. 项目2
1. 项目3
    1. 项目3.1
    1. 项目3.2
```

**效果1**

1. 项目1
1. 项目2
3. 项目3
    1. 项目3.1
    2. 项目3.2

1. 项目1
1. 项目2
1. 项目3
    1. 项目3.1
    1. 项目3.2

**样例2**

``` markdown
58. 项目5
2. 项目6
3. 项目7
```

**效果2**

58. 项目5
2. 项目6
3. 项目7




### 文字样式

#### 加粗
加粗字体用来突出效果，让重点更加鲜明
**使用语法**：** xxxxx ** 或者 __ xxxx __
**快捷键：ctrl+b(bold)**

**样例**

``` markdown
**你好**，你好
__你好__，你好
```

**效果**

**你好**，你好
__你好__，你好

#### 斜体
**快捷键：ctrl+i(italics)**
**使用语法：** * xxx * 或者_ xxx _
**样例**

``` markdown
*斜体*，斜体
_斜体_,斜体
```
**效果**
*斜体*，斜体
_斜体_，斜体

#### 删除线
删除线是用来标记错误的信息，达到警示的作用。
**样例**

``` markdown
~~删除~~，不删除
```
**效果**
~~删除~~，不删除


### 引用
引用了别人说的话或者是别人的文章，最好就需要标记一下引用。一般一用标记后会有一个灰色的区域来显示内容，以突出是引用别人的东西。
**快捷键：ctrl+q(quote)**
**使用语法：** > 引用内容
**样例**

``` markdown
> 引用内容
> 引用内容
```
**效果**
> 引用内容
> 引用内容





### 水平线/分割线
一般用于分割内容，表示上下的两部分是不关联的，或者联系程度没有那么高的。
**快捷键：ctrl+r**
**使用语法：** ----（长度没有限制，只要-的数量超过三个就好了，因为一个是无序的意思，两个是--的意思，三个以上系统才会认为是分割线的意思）

**样例**

``` markdown
-----
```
**效果**

---




### 链接类

#### 自动转换成超链接
如果我们直接写一个url，那个url会自动转换成对应的超链接，我们点击url后会自动跳转到对应的页面去的了。这个是接下来的所有的超链接类的基础。
**样例**

``` markdown
https://www.baidu.com/
```
**效果**
https://www.baidu.com/

#### 超链接
超链接一般是用于链接到其他地方，比如链接到其他的网页，点击超链接就会跳转到其他地方。“[]”括号里面是文字解释说明，“（）”括号里是链接的url或者路径等。也可以像论文的标注一样，统一写在一起，然后不同的地方就使用下标标记就好了。下面的也类似
**使用语法**：
1. [链接名称]（链接地址）
2. [链接名称][1]
[1] : 链接地址

**快捷键：ctrl+l(link)**

**样例**

``` markdown
[百度](https://www.baidu.com/)
```
**效果**

[百度](https://www.baidu.com/)

#### 图片
显示图片和超链接类似，一般提供一个url就可以显示图片了。
**使用语法**：
1."![名称]（链接地址）"
2.“![名称][1]”
[1] : 链接地址

**快捷键：ctrl+g(graph)**

**样例**

``` markdown
![自然风景](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1540818893336&di=d9f167a4fdb0f7f82feda5cc2db43145&imgtype=0&src=http%3A%2F%2Fimg17.3lian.com%2Fd%2Ffile%2F201702%2F27%2Fecb90526f7386849a0773f69d3b71636.jpg)
```
**效果**


![自然风景](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1540818893336&di=d9f167a4fdb0f7f82feda5cc2db43145&imgtype=0&src=http%3A%2F%2Fimg17.3lian.com%2Fd%2Ffile%2F201702%2F27%2Fecb90526f7386849a0773f69d3b71636.jpg)

**说明**：这种情况的图片显示不能控制图片的大小，默认是居中，图片大小是多大就会自动显示多大，如果要做到可控的大小以及位置的调整，需要使用像前端一样的“<img”标签进行设置。建议还是使用第二种，这样方便和整体的 布局保持一致，而不会让图片显得特别大，和整体效果有点不合适。

**样例**

``` markdown
<div align="center">
	<img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1540818893336&di=d9f167a4fdb0f7f82feda5cc2db43145&imgtype=0&src=http%3A%2F%2Fimg17.3lian.com%2Fd%2Ffile%2F201702%2F27%2Fecb90526f7386849a0773f69d3b71636.jpg" width="150px">
</div>
		
```
**效果**
<div align="center">
	<img src="https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1540818893336&di=d9f167a4fdb0f7f82feda5cc2db43145&imgtype=0&src=http%3A%2F%2Fimg17.3lian.com%2Fd%2Ffile%2F201702%2F27%2Fecb90526f7386849a0773f69d3b71636.jpg" width="150px">
</div>



### 表格
用表格显示数据方便我们更加清晰的对比不同的数据部分，使整个数据都清楚明了。一般我们可以通过Excel表格弄好数据后在截图复制到这里，但是这样可能还需要打开Excel表格，但是现在我们这里直接可以编辑表格数据，所以我们可以充分的使用这个语法来方便自己工作。
**快捷键：暂无**

#### 普通表格
主要是第一行和第二行的形式要对应，第一行一般是表头的字段，第二行主要是根据第一行的不同字段分割显示表格内容，表格内容可以是空的。
**样例**

``` markdown
First Header  | Second Header | Thrid Header
------------- | ------------- | -------------
Content Cell  | Content Cell  | Content Cell 
Content Cell  | Content Cell
Content Cell  | | Content Cell 

```
**效果**
First Header  | Second Header | Thrid Header
------------- | ------------- | -------------------
Content Cell  | Content Cell  | Content Cell 
Content Cell  | Content Cell
Content Cell  |   | Content Cell 

#### 增强型表格
（目前简书和GitHub也不支持增强型表格）我们发现普通表格一般是规整的，一般都是单独一个单元格的，而且每个单元格之间是用一个竖线分割的，前后不用竖线，但是增强型的表格就不一样了，他是每一个内容前后都会有竖线进行分割，可以进行单元格合并，而且可以自己定义样式，比如说一二行是表头等内容，然后通过
|------------- | -------------|-------------|这种按照这种形式进行数据的分割和整理做出可以合并单元格的表格了。
**样例**

``` markdown
|First Header  | Second Header ||
|First Header  | Second Header | Third Header|
|------------- | -------------|-------------|
表身1Content Cell  | Merge Content Cell||
Content Cell  | Content Cell| Content Cell|

表身2Content Cell  | Merge Content Cell||
Content Cell  | Content Cell| Content Cell|
[表格标题]
```

**效果**

|First Header  | Second Header ||
|First Header  | Second Header | Third Header|
|------------- | -------------|-------------|
表身1Content Cell  | Merge Content Cell||
Content Cell  | Content Cell| Content Cell|

表身2Content Cell  | Merge Content Cell||
Content Cell  | Content Cell| Content Cell|
[表格标题]


### 支持html的写法
[支持的html标签](https://github.com/github/markup/tree/master#html-sanitization)

拓展阅读
《GitHub 简书 小书匠中markdown的特殊语法对比》


参考资料
1.文中大部分资料参考于小书匠的官网 http://markdown.xiaoshujiang.com/