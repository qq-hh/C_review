

### PCB技巧（五）



####  一、问题及原因

问题：

对板子进行测试，发现引脚OPA电压不对，DAC输出电压没有问题，OPA接DAC输出应该和DAC电压大致差不多，但是电压差100mV。

原因：

经查找是下图中GND走线与旁边引脚OPO有接触。在未焊接任何元件的裸板进行测试，OPO引脚和GND的确导通。

走线在检查报错时一定要注意：线距小于8mil的一定要仔细查看，避免后续问题。

![img](https://img-blog.csdnimg.cn/bc5007413db242d8b784a7526f568ecd.png)

##  二、如何避免PCB走线出错

报错运行如下：

点击Tools -->Design Rule Check



![img](https://img-blog.csdnimg.cn/5255029b9dd94ea08d122930df2c5fcc.png)

 出现以下界面，然后点击Run Design Rule Check 进行规则检查。

![img](https://img-blog.csdnimg.cn/9c14e918f6aa44268ba1a09bfe780909.png)

查看报错信息如下：注意下以下报错信息和PCB板子上是否有为连接的线。

报错信息如图：

 ![img](https://img-blog.csdnimg.cn/772ca487a17f440fa3cd00bc668ca6e4.png)

 PCB如果有线未连接如下显示：

![img](https://img-blog.csdnimg.cn/a00c4f166336430581e44216c7ffef77.png)

 另外，这种走线在PCB连线中是允许的，如下图。注意：这种线是线和覆铜相连，由于线GND和覆铜都是GND，所以可以连接，在画的时候要注意：线必须在覆铜上，线和覆铜才会导通。如图，这种走线是正确的。

![img](https://img-blog.csdnimg.cn/78f378929afa40e788f235ffb277b627.png)

如图，这样连接是不导通的：

覆铜避开了线，虽然它们都是GND，但是没有导通，这种走线是错误的。

![img](https://img-blog.csdnimg.cn/9bc5d2d8160f4e23acaa25ee1103a067.png)