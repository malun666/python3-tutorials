# Python3 Tutorials

Python2已经不再维护，所以直接进行Python3 的介绍。

## Python 介绍

Python 是著名的“龟叔” Guido van Rossum 在 1989 年圣诞节期间，为了打发无聊的圣诞节而编写的一个编程语言。牛人就是牛人，为了打发无聊时间竟然写了一个这么牛皮的编程语言。
Python 是高级编程语言，它有一个特点就是能快速的开发。Python 为我们提供了非常完善的基础代码库，覆盖了网络、文件、GUI、数据库、文本等大量内容，被形象地称作“内置电池（batteries included）”。用 Python 开发，许多功能不必从零编写，直接使用现成的即可。而且 Python 还能开发网站，多大型网站就是用 Python 开发的，例如 YouTube、Instagram，还有国内的豆瓣。很多大公司，包括 Google、Yahoo 等，甚至 NASA（美国航空航天局）都大量地使用 Python。

当然，任何编程语言有有点，也有缺点，Python 也不例外。那么 Python 有哪些缺点呢？
第一个缺点就是运行速度慢，和C程序相比非常慢，因为Python是解释型语言，你的代码在执行时会一行一行地翻译成CPU能理解的机器码，这个翻译过程非常耗时，所以很慢。而C程序是运行前直接编译成CPU能执行的机器码，所以非常快。
第二个缺点就是代码不能加密。如果要发布你的 Python 程序，实际上就是发布源代码。像 JAVA , C 这些编译型的语言，都没有这个问题，而解释型的语言，则必须把源码发布出去。

## Python3 安装

直接参考[官方文档](https://docs.python.org/zh-cn/3.7/using/index.html)

## Python3 HelloWorld

国际惯例，学习一门新语言，第一个程序当然是`Helloworld`

步骤：

1. 第一步： 新建一个文件，命名为 HelloPython.py , 注意，这里是以 .py 为后缀的文件。

1. 然后打开文件，输入如下代码：

  ```py
  print('Hello Python, aicoder.com')
  ```

> print是python内置的函数，用于向控制台打印内容。

3. 打开命令行窗口，把当前目录切换到 HelloPython.py 所在目录，就可以运行这个程序了，下面就是运行的结果。

```sh
Hello World, aicoder.com
```

## Python的语法入门基础

### 文件编码注释

- 如无特殊情况, 文件一律使用 UTF-8 编码
- 如无特殊情况, 文件头部必须加入#-*-coding:utf-8-*-标识

### 代码注释

#### 块注释

“#”号后空一格，段落件用空行分开（同样需要“#”号）

```py
# 块注释
# 块注释
#
# 块注释
# 块注释
```

#### 行注释

至少使用两个空格和语句分开

```py
# 正确的写法
x = x + 1  # 边框加粗一个像素
```

### 文档注释

作为文档的Docstring一般出现在模块头部、函数和类的头部，这样在python中可以通过对象的__doc__对象获取文档. 编辑器和IDE也可以根据Docstring给出自动提示.

文档注释以 """ 开头和结尾, 首行不换行, 如有多行, 末行必需换行。

比如:

```py
# -*- coding: utf-8 -*-
"""Example docstrings.
  this function is ....
"""

...

"""Oneline docstring"""

```

> 所有的公共模块、函数、类、方法，都应该写 docstring 。私有方法不一定需要，但应该在 def 后提供一个块注释来说明。
> docstring 的结束"""应该独占一行，除非此 docstring 只有一行。
