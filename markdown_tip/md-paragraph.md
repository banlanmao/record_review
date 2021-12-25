# Markdown 段落

Markdown 段落没有特殊的格式，直接编写文字就好，**段落的换行是使用两个以上空格加上回车**。

![img](md-paragraph.assets/36A89BDA-A062-4D66-A41B-0EBEE7891AB9.jpg)

当然也可以在段落后面使用一个空行来表示重新开始一个段落。

![img](md-paragraph.assets/3F254936-778E-417A-BEF2-467116A55D00.jpg)

------

## 字体

Markdown 可以使用以下几种字体：

```
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```

显示效果如下所示：

![img](md-paragraph.assets/md3.gif)

------

## 分隔线

你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：

```
***

* * *

*****

- - -

----------
```

显示效果如下所示：

![img](md-paragraph.assets/3F46EAA9-DADE-48FD-99AA-DF7BEBFAA4FA.jpg)

------

## 删除线

如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 **~~** 即可，实例如下：

```
RUNOOB.COM
GOOGLE.COM
~~BAIDU.COM~~
```

显示效果如下所示：

![img](md-paragraph.assets/B5270A31-15D0-410B-AE1D-B9655B8F331C.jpg)

------

## 下划线

下划线可以通过 HTML 的 **<u>** 标签来实现：

```
<u>带下划线文本</u>
```

显示效果如下所示：

![img](md-paragraph.assets/05A27273-B66D-43DE-A3DB-0D32FF024093.jpg)

------

## 脚注

脚注是对文本的补充说明。

Markdown 脚注的格式如下:

```
[^要注明的文本]
```

以下实例演示了脚注的用法：

```
创建脚注格式类似这样 [^RUNOOB]。

[^RUNOOB]: 菜鸟教程 -- 学的不仅是技术，更是梦想！！！
```

演示效果如下：

![img](md-paragraph.assets/md5.gif)