# Newton Iteration

1.程序里给出的算例是求解方程的根，因此f(x)的形式是已知的，因此可以求微分。但是实际情况往往是无法得到f(x)的解析式，只能求取f(x)的值，所以这里用求差分代替求微分，牛顿迭代式则可以写为：

![](https://ws3.sinaimg.cn/large/006tKfTcly1g1knmkvbtdg308v01cdfl.gif)
 
 其中![](https://ws3.sinaimg.cn/large/006tKfTcly1g1knqiajajg300f00c03y.gif)为一小量。
 
2.最初是想写一个通用的牛顿迭代函数，希望将要迭代求解的方程作为函数的输入，不过将函数作为参数传递不像我想的那么简单。。。
一开始写了一种以普通函数作为参数传递的牛顿迭代函数，但是真正用的时候带求解的方程是另一个类里的成员函数，这就需要写一种以成员函数作为参数传递的牛顿迭代函数。必须说明的是，目前我写的这个通用性受限，需要在我写好的方程类里写方程，将来可以将该牛顿迭代函数声明为模板函数。

>一个插曲：之前用Macdown输入公式的时候也知道可以以LaTeX形式输入，但就是搞不出来，看自带的帮助例子也没搞懂，今天偶然发现就是没有进行设置！！！

* 设置方法：

`Preferences→Rendering→勾选"TeX-like math syntax"以及"Use dollar sign($) as inline delimiter"`
![](https://ws3.sinaimg.cn/large/006tKfTcly1g1jzt3a9tzj30sq0uy12p.jpg)

## 曾经沧海难为水，除却巫山不是云。
