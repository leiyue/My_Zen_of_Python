# 我的Python之禅
感谢茜茜的邀请，很高兴跟大家分享我自己学习Python的心得。

## Python 之禅
学习过Python的同学，基本上都知道在 `python` 交互解析器中输入 `import this` 就会出现 **Tim Peters** 的 ***The Zen of Python*** ，我就从这段偈语开始我的感悟吧。

```
$ python
Python 2.7.11 (default, Jan 22 2016, 08:29:18)
[GCC 4.2.1 Compatible Apple LLVM 7.0.2 (clang-700.1.81)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
>>>
```

翻译和解释：

```
优美胜于丑陋（Python以编写优美的代码为目标）
明了胜于晦涩（优美的代码应当是明了的，命名规范，风格相似）
简洁胜于复杂（优美的代码应当是简洁的，不要有复杂的内部实现）
复杂胜于凌乱（如果复杂不可避免，那代码间也不能有难懂的关系，要保持接口简洁）
扁平胜于嵌套（优美的代码应当是扁平的，不能有太多的嵌套）
间隔胜于紧凑（优美的代码有适当的间隔，不要奢望一行代码解决问题）
可读性很重要（优美的代码是可读的）

即便假借特例的实用性之名，也不可违背这些规则（这些规则至高无上）

不要包容所有错误，除非你确定需要这样做
（精准地捕获异常，不写 except:pass 风格的代码）

当存在多种可能，不要尝试去猜测

而是尽量找一种，最好是唯一一种明显的解决方案（如果不确定，就用穷举法）

虽然这并不容易，因为你不是 Python 之父（这里的 Dutch 是指 Guido ）

做也许好过不做，但不假思索就动手还不如不做（动手之前要细思量）

如果你无法向人描述你的方案，那肯定不是一个好方案；反之亦然（方案测评标准）

命名空间是一种绝妙的理念，我们应当多加利用（倡导与号召）
```

## 关于我
简单说完了本文的中心思想，下面就开始论述。

在论述之前，唠叨一下本人的实际条件，让大家对后面将的学习方式有个条件认知。

本人非计算机专业，非软件开发出身，长期从事技术管理工作，绝大多数时间和各种工程师打交道。

大学语言课学过 C 语言，补考；后来自学到写拿 C 写 TSR（内存驻留程序） 的地步。

后来因为工作需要，前后学过 PHP，Android，Objective-C，node.js，AngularJS……

项目赶进度的时候不管后台或前端也需要上手帮忙……

Windows / Linux / Mac OS 混合使用。

## 学习目标
我先列以下学习目标供大家参考：

1. 单个Python脚本（200行以内）
2. 简单的Python项目（5个轮子以下的项目）
3. 复杂的Python项目（有足够的轮子可以用，只需要负责业务逻辑）
4. 足够复杂的Python项目（搞不好得自己攒轮子）
5. 成熟的Python项目（贡献轮子给大家用）

您的学习目标是哪一个呢？

不同的目标对应着不同的要求，对于要求不高的同学没有必要花费过多的精力在工具上。

## 版本选择
**Python 2 or Python 3**

学习目标为 `1`，`2`，`3` 的同学直接学 Python 3 吧。

学习目标为 `4`, `5` 的同学欢迎你们来到混乱的世界，因为大多数项目只能用 `2.7` ；甚至还要保证程序在 Python 2 和 Python 3 兼容。 

> **Tips:**
> 
> python 2 + `__futur__`
> 
> `from __future__ import (absolute_import, division, print_function, unicode_literals)`

## 学习环境
最好的学习环境我认为还是 OS X ，遇到蛋疼的问题少一些。

不过我写代码用的最多是还是 Windows ，双屏效率高一些。

部署的服务器当然都是 Linux 环境，有很多部署工具可以帮助你。

简单粗暴的问答一些典型问题：

1. 不是程序员就犯不着为学 Python 买 **MBP** 。（壕除外）
2. 用虚拟机部署 Linux 环境学 Python 挺好的。
3. 只能用 Windows 的同学听我的，我的作业全部是在 Windows 上完成的。

## 入门教程

1. 廖雪峰《Python教程》
2. 笨办法学Python
3. 与孩子一样学编程
4. 魔力教程

个人看法：

1. `1` 只用看最基础的部分，经典但无趣
2. `2` 只坚持了前几章，成就感全无，确实是笨办法
3. `3` 号称是给孩子看的，不过据说大人都吃力，`(*^__^*) `嘻嘻……
4. `4` 茜茜都说是全宇宙最好的教材~\(≧▽≦)/~啦啦啦，赶快来学习吧~~

## 学习诀窍
我总结自己的学习方法有三点：

1. 看
2. 想
3. 写

### 看
看什么？

1. 通识 [Awesome Python](https://github.com/vinta/awesome-python)
2. 文档 例如：爬虫 [Scrapy](http://scrapy.org/) 文档
3. 代码 [Github](https://github.com)

#### 通识
- 快速了解整个Python开发各个方向的整体情况。
- 要找轮子也知道该去找哪个轮子。
- 当然不止Awesome Python，实际上只要是有关Python的东西我都会读一读。

#### 文档
- 不同的学习内容都有入门教程。
- 这些入门教程一般都非常好用。
- 帮助你快速安装轮子。

#### 代码
- 搜索 [Github](https://github.com) 。
- 你遇到的问题别人也遇到过。
- 看看别人是怎么解决的。
- 代码美不美，框架帅不帅。
- 考虑一下是不是要展开追求呢？O(∩_∩)O~

### 想
想追求的时候自然过渡到想的阶段，这个阶段 **Python之禅** 就要起作用了。

Python哲学就是任何事情尽量找一种，最好是唯一一种明显的解决方案，我们叫做 **Pythonic** 。

在阅读功能相近的代码时，你自然得就会感受到大家都好像使用同一种思维或者同一种方法或者同一种形式在解决问题。(⊙v⊙)嗯，于是你也继续保持队形，在自己的代码中保持同样的特色。

你自己实现过的代码，把关键字放到 [Github](https://github.com) 上搜一搜，看看有没有别人实现的更好的代码，想一想自己在哪些地方做的不够好，尝试把别人的优点带回到自己的代码中。

不要过早的优化框架，先实现功能，在实现过程中你会总会发现有更棒的想法可以试试。

尽量使用一些人性化的轮子，反人性的轮子都会被人所唾弃的。
> Python 2 在 `urllib` 和 `urllib2` 轮子上的设计不得人心，被绝大多数人舍弃，转而使用更人性化的 `requests` 。

### 写
然后语言类的学习都离不开 **写** 代码。

学习语言只有一条路： 写，写，写

这点不管是哪个语言哪个教程都是一样的要求，一定要多写代码。

而且要反复写。

有时觉得自己的代码不够 **Pythonic** ，等到自己有时间了就删了全重写。

开始一个项目的时候，先确认最基本的功能，实现最小原型。

然后再在这个原型上逐步扩展，实现其他功能。

### 小结
遇到问题不知道方向，请返回第一步，重新按照 `看`，`想`，`写` 三个步骤进行。

## 带着问题学习
Python学习三个最常见的理由：

1. Web开发
2. 爬虫开发
3. 科学计算

始终记得自己是为什么要学习Python的：

1. Django 和 Flask 到底学哪个
2. Scrapy 和 requests + lxml 哪个更实用
3. numpy 和 cython 到底难不难

> @听雨：我看好你哟，虽然你不在上述范围，一定要记得自己的学习目标。

可能 **实战计划** 并不能解决你所有的问题，因为很多问题只有你自己才能发现真正的答案。

## 社群
学习是痛苦的，孤独也是痛苦的。

大家一起学，遇到困难相互帮助。

这就是社群的作用和力量，但请不要用简单的重复的问题浪费大家的时间，请学会科学上网和正确使用搜索引擎。

## 期许
希望 **魔力教程** 和 **实战计划** 越来越成熟，取得更多的成绩。

希望大家都能够通过自己的努力达到自己设定的学习目标。

谢谢大家！






