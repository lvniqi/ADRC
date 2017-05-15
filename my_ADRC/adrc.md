小白理解ADRC控制器
==========

## 简介
### 传统PID
传统上，对于模型不确定的系统我们(或者仅仅是我？)都喜欢用PID控制。
即使在模型清楚的情况下，有时我们也很难获得模型的部分参数，所以依然沿用PID控制器。

一般我们看到的的pid控制器是长这样的：

<div align=center>
<img src="https://imgsa.baidu.com/baike/c0%3Dbaike180%2C5%2C5%2C180%2C60/sign=0c235bc3740e0cf3b4fa46a96b2f997a/5243fbf2b21193132c0f096163380cd790238d97.jpg" width="400"  />
</div>

如果把这样的pid控制器写成传递函数，就是

![](http://latex.codecogs.com/gif.latex?G(s)=P+I\\frac{1}{s}+Ds)

Z变换的话是变成

![](http://latex.codecogs.com/gif.latex?G(z)=P+I\cdot{T_s}\\frac{1}{z-1}+D\\frac{z-1}{z\cdot{T_s}})

嗯~看起来挺不错的，那么问题在哪儿呢？

#### 超调的产生
这段我要抄书啦，都别拦我:stuck_out_tongue_winking_eye:

