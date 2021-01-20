
---
title: Girls_In_AI
date: 2019-01-13 19:19:18
tags:
- machine_learning
- learning note
---
首先表达一下对这个项目发起者的感谢！ [项目链接](https://github.com/YZHANG1270/Girls-In-AI/tree/master/machine_learning_diary/day-2)

我的个人网站[janeqinblog.com](http://janeqinblog.com/)的搭建是参考了ZHANGYI的博客[YZHANG](http://codewithzhangyi.com/2018/04/19/%E5%A6%82%E4%BD%95%E6%90%AD%E5%BB%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E4%B8%AA%E4%BA%BA%E7%BD%91%E7%AB%99%EF%BC%88%E4%B8%8A%EF%BC%89/) 她同时也是项目的发起者

这篇文章将用来记录我在学习过程中遇到的问题及解决方案，希望能够帮助到和我遇到相同问题的人

###  machine_learning_diary/day-2
**issuses:**
- python3.5下载完成、 配置环境变量之后，进行到 *下载python3.5版本的 Jupyter Notebook* 这一步 出现了错误，如下图：
![error](https://img-blog.csdnimg.cn/20190114230700536.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
socket.timeout: The read operation timed out
初步感觉是网络方面的问题， Google之后在Stack Overflow上找到了答案.
[参考链接](https://stackoverflow.com/questions/43298872/how-to-solve-readtimeouterror-httpsconnectionpoolhost-pypi-python-org-port)

![](https://img-blog.csdnimg.cn/20190114230931722.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
**解决方案：**
依照上方提示， 打开Anaconda Prompt， 在命令行中输入：
```
pip install --default-timeout=100 jupyter notebook
```
成功解决问题

另： 可以把环境变量看成是笔记本， python3.5看做是写笔记， 买好笔记本（搭建好环境）才可以写东西。
![](https://img-blog.csdnimg.cn/20190114231609638.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
这就是我在jupyter“笔记本”上写的笔记啦！ 哈，学习使我快落，Learning makes me happy(熬夜伤肝).

Feeling: 做的过程中会遇到非常非常多的、一个接一个的问题， 这时候要调整心态， 发现一个说明有一个提高的点， 首先接受它， 无法处理的话先记录下来， 之后通过搜索或者提问， 一步一步解决， 最后！ 就可以写成笔记和经验， 内化成你自己的小宝藏！ （仓鼠屯瓜子）我要当最胖胖的仓鼠！

###  machine_learning_diary/day-3
今天也是学习的一天， 之前学的python知识， 由于不常运用， 渐渐就会遗忘， 结合工程是最好掌握一门语言的方法（奈何现在只做了java的工程）

这次课程带我回顾了变量的知识

**conception**
- 变量：
*variables are reserved memory locations to store values*

预留的内存地址用来存值（可以看成是个杯子， 可以放许多不同数据类型的东西  比如：Numbers数字（1）、String字符串 （"girls in AI"）

**Python Numbers**

Number data types store numeric values. **Number objects are created when you assign a value to them.** For example −
```
var1 = 1
var2 = 10 #var1是一个Number类型的对象
```
You can also delete the reference to a number object by using the del statement. The syntax of the del statement is −
```
del var1[,var2[,var3[....,varN]]]]
```
You can delete a single object or multiple objects by using the del statement.

For example −
```
del var
del var_a, var_b
```
### 参考链接
[Variable Types](https://www.tutorialspoint.com/python3/python_variable_types.htm)

[数据模型](https://docspy3zh.readthedocs.io/en/latest/reference/datamodel.html)

一贯的遇到了很多问题（就是不断会遇到问题的， 大家放宽心）

**issues:**
由于我之前下载了python2.7、3.7、3.6，现在又下了3.5 。。。。 所以环境变量一大堆， 很容易出现版本冲突， 在这里告诉大家一个可以切换python版本的方法。
1. 首先大家可以找到自己下载python的文件所在地（路径），以我的为例：

![](https://img-blog.csdnimg.cn/20190115180152701.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
大家注意到， 这里python的exe文件名字被我改成了python3, 所以 如果我想用3.6版本的python， 我就会在命令行中输入python3, 这时它的版本就是3.6的， 可以使用python --version来查看。![](https://img-blog.csdnimg.cn/20190115180434327.png)
我这里还有一个2.7版本的python, 大家可以猜到， 如果我输入python2的话， 版本会是？
![](https://img-blog.csdnimg.cn/20190115180500703.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
![](https://img-blog.csdnimg.cn/20190115180633866.png)
2. 但是如果你要使用pip命令下载其他人的模块， 就要注意环境变量的配置了。
**设置环境变量**（Windows10）
右键我的电脑->属性->高级系统设置->环境变量
在下方的**系统变量**中，找到Path, 双击
![](https://img-blog.csdnimg.cn/20190115181332588.png)

这里我想要用python3.5版本的pip， 所以要把它的路径上移到最上面
![](https://img-blog.csdnimg.cn/20190115181428658.png)

![](https://img-blog.csdnimg.cn/20190115181515974.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1FpbnFpblRheWxvcg==,size_16,color_FFFFFF,t_70)
其实我们要做的就是， 让计算机能够找到你的pip所在的地方， 也就是设置环境变量。

推荐一个代码可视化的网站， 可以将你建立变量、赋值通过图像描绘。 [点击这个链接](http://pythontutor.com/)

### machine_learning_diary/day-4~7
这几节内容是python语法介绍， 和java很类似, 所以合并在一起写一篇

python中的
1. 逻辑运算符
- **与（&&）**为**and**
- **或(||)**为**or**
- **非(!)**为**not**
感觉更好记忆， 贴近英语单词意思

2. 比较操作符
- x == y #x等于y
- x != y #x不等于y
- x < y  #x小于y
- x > y  #x大于y
- x <= y #x小于等于y
- x >= y #x大于等于y
- x **is** y #x是y  （python中特有)
- x **is not** y #x不是y

*布尔表达式返回的True和False, 是布尔类型的两个取值， 它们不是字符串string*
**可以用type()来查询变量的类型**
```python
In: type(True)
Out: bool

In: type('True')
Out: str
```

