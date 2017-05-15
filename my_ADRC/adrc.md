小白理解ADRC控制器
==========

## 简介
传统上，对于模型不确定的系统我们(或者仅仅是我？)都喜欢用PID控制。
即使在模型清楚的情况下，我们也很难获得模型的部分参数。

一般的pid控制器是这样的：

<div align=center>
<img src="https://imgsa.baidu.com/baike/c0%3Dbaike180%2C5%2C5%2C180%2C60/sign=0c235bc3740e0cf3b4fa46a96b2f997a/5243fbf2b21193132c0f096163380cd790238d97.jpg" width="400"  />
</div>

这样的pid控制器传递函数为

![](http://latex.codecogs.com/gif.latex?G(s)=P+I\\frac{1}{s}+Ds)

Z变换后变成

![](http://latex.codecogs.com/gif.latex?G(z)=k_P+k_I\cdot{T_s}\\frac{1}{z-1}+Dz)