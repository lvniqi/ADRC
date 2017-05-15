小白理解ADRC控制器
==========

## 简介
传统上，对于模型不确定的系统我们(或者仅仅是我？)都喜欢用PID控制。
即使在模型清楚的情况下，我们也很难获得模型的部分参数。

一般的pid控制器是这样的：

<div align=center>
<img src="https://imgsa.baidu.com/baike/c0%3Dbaike180%2C5%2C5%2C180%2C60/sign=0c235bc3740e0cf3b4fa46a96b2f997a/5243fbf2b21193132c0f096163380cd790238d97.jpg" width="400"  />
</div>

![](http://latex.codecogs.com/gif.latex?\\frac{\\partial J}{\\partial \\theta_k^{(j)}}=\\sum_{i:r(i,j)=1}{\\big((\\theta^{(j)})^Tx^{(i)}-y^{(i,j)}\\big)x_k^{(i)}}+\\lambda \\xtheta_k^{(j)})

作者：Deep Reader
链接：https://www.zhihu.com/question/26887527/answer/43166739
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
<div align=center>
<img src="http://latex.codecogs.com/gif.latex?\frac{\partial J}{\partial \theta_k^{(j)}}=\sum_{i:r(i,j)=1}{\big((\theta^{(j)})^Tx^{(i)}-y^{(i,j)}\big)x_k^{(i)}}+\lambda \theta_k^{(j)}" />
</div>