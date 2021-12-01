# Markdown的转换与学习

本文主要分成四部分，第一部分Markdown与Latex文件的转换，第二部分关于Markdown与知乎文章的转换，第三部分讨论其它涉及转换的情形，第四部分提供一些学习Markdown的材料。

## Markdown与Latex文件的转换

Markdown语法相对简单，可以随时编辑，随时渲染；而Latex必须先设定好引用的packages和板式，相对复杂。因此Markdown适用于方便及时的记录，而Latex适用于较为正式的材料的编辑，如论文，教材等。有时我们需要把一段Markdown内容插入Latex中，或将Latex中的一段导出为Markdown，这类问题比较好解决。

这里，我为大家推荐一款Markdown编辑器：Typora（[链接](https://typora.io/)），为了使用转换功能，我们需要安装Pandoc，这是一款Github上的开源软件，我们可以通过搜索获得它，也可以在Typora的帮助菜单中选择Install and Use Pandoc获取它的下载网址（[链接](https://github.com/jgm/pandoc/releases/tag/2.10.1)）。安装完成后， 我们就可以使用文件菜单中的导入和导出功能读取和保存为Latex文件了。

## Markdown与知乎的转换

很多人更习惯在Markdown编译器中进行编辑，不习惯在知乎窗口进行编辑，并且知乎编辑在内容较多时可能出现卡的问题，因此借助Markdown编辑知乎文章与回答就成为了问题。这个问题相对有写棘手，下面给出我的方案给大家参考：

当我们上传知乎文章时，知乎并非使用Markdown语法，这需要转换，我使用的是在线Markdown编辑工具mdnice（[链接](https://www.mdnice.com/)），我们需要把编辑好的文档复制到这里，检查后点击右上角的按钮，即可复制到知乎或微信公众号了，图片问题仍需单独处理。如果您对此方案不满意，我可以为您提供一些其它思路：

[思路一](https://zhuanlan.zhihu.com/p/91887957)、[思路二](https://zhuanlan.zhihu.com/p/97455277)、[思路三](https://zhuanlan.zhihu.com/p/99057715)、[思路四](https://zhuanlan.zhihu.com/p/141590985)。

我们可能写了一些知乎，希望下载保存下来，我的做法如下：

首先，在文章底部点击设置，修改文章，进入编辑模式，然后粘贴到空白的Typora中，保存。使用如下python代码处理保存的md文件：

```
import re
raw_file="name1.md"  #输入需转换的文件名
made_file="name2.md"     #给转换后的文件命名
with open(raw_file,"r",encoding="utf8") as f:
    s = f.read()
t = re.sub(r"\!\[(.*)\]\(.*?\)\1",r"$\1$",s)
with open(made_file,"w") as f:
    f.write(t)
```

这样，转换后的文件就是正确的Markdown了。

注：以上做法来自于知乎问题：[链接](https://www.zhihu.com/question/309343971/answer/959074405?utm_source=wechat_session&utm_medium=social&utm_oi=925517376135499776&utm_content=group3_Answer&utm_campaign=shareopn)。感谢知乎用户： [@柴士童](https://zhuanlan.zhihu.com/people/1756465d35cf4b6ec1c6df040d98d214) 。

以上做法要求我们可以编辑文章，即文章是我们自己创作的，而保存别人的文章，我并没有找到较好的办法处理其中的公式，因公式是用图片呈现的，我们不进入编辑模式直接复制得到的公式本质是一个到网址的链接，得不到公式内容，下面给出可能可行的思路：

[思路一](https://zhuanlan.zhihu.com/p/56694990)、[思路二](https://zhuanlan.zhihu.com/p/110250329)、[思路三](https://zhuanlan.zhihu.com/p/29778024)。

## 其它转换的情形

我们打开Typora的导入与导出菜单，可以发现，它不仅仅支持与Latex文件的转换，还支持其它的一些格式。我们比较关注Word、Epub、Pdf。这意味着，Markdown文件可以与Word无缝切换。

然而，我们只可以输出Pdf，不可以导入Pdf，但是，当我们拿到一篇论文的Pdf时，我们可以先将Pdf转换为Epub，再导入Epub，得到Markdown代码。因此，Markdown是可以与Pdf文档互转的，前提是Pdf真的由Markdown代码（影印版的书的Pdf不建议进行转换）。

此外，还有Pdf直接转Markdown的工具，网址：https://pdf2md.morethan.io/

这个网址来自问题：

[有没有什么办法把pdf转成markdown？](https://www.zhihu.com/question/300833276/answer/1230291158?utm_source=wechat_session&utm_medium=social&utm_oi=925517376135499776&utm_content=group3_Answer&utm_campaign=shareopn)

## Markdown学习材料

1、https://blog.csdn.net/qq_30241709/article/details/88654050 

2、https://www.jianshu.com/p/5a27d195678f 

3、[blog.csdn.net/apr15/article/details/105597907?utm_medium=distribute.pc_relevant.none-task-blog-title-2&spm=1001.2101.3001.4242](https://blog.csdn.net/apr15/article/details/105597907?utm_medium=distribute.pc_relevant.none-task-blog-title-2&spm=1001.2101.3001.4242) 

4、https://blog.csdn.net/young951023/article/details/79601664?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-1.nonecase&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-1.nonecase 

5、https://www.jianshu.com/p/7c34f5099b7e

我根据以上几份资料整理了一份我自己的数学公式列表，发表在本专栏的Github项目上。

[DSroad](https://github.com/ButterYan/DSroad)

版权说明：部分方法在知乎上已被多人提及，故无法保证收录完全，因而不提供来源，敬请理解。