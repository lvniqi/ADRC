小白理解ADRC控制器
==========

## 简介
传统上，对于模型不确定的系统我们(或者仅仅是我？)都喜欢用PID控制。
即使在模型清楚的情况下，我们也很难获得模型的部分参数。

一般的pid控制器是这样的：

<div align=center>
<img src="https://imgsa.baidu.com/baike/c0%3Dbaike180%2C5%2C5%2C180%2C60/sign=0c235bc3740e0cf3b4fa46a96b2f997a/5243fbf2b21193132c0f096163380cd790238d97.jpg" width="400"  />
</div>

@名称:MathJax
@触发文本:MathJax
@代码片段:请在下一行开始输入内容!
<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
It is well known that if $ax^2 + bx + c = 0$, then $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.