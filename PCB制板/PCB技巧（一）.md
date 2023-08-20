##  一、AD基本使用技巧

1、mm和mil切换

![img](https://img-blog.csdnimg.cn/812eebf37fd84bdcb68668ed79abbe58.png)

 2、AD导入结构工程师的dwg结构文件

![img](https://img-blog.csdnimg.cn/d9fe300d108644c28591a9ae188bebfe.png)

 导入时选择mm，一定要注意！

3、机械层和kepp-out层注意检查！

![img](https://img-blog.csdnimg.cn/c7986b0de1564efb863ca80c1e883e6b.png)



 ![img](https://img-blog.csdnimg.cn/6d0bff0f060947eba68c03a77c1c16e3.png)

有次打板只在机械层画了孔，没在keep-out层画，结果板子打回来立创没有给打孔。第一：没有仔细确认生产文稿；第二：制板工程师有的看机械层，有的看keep-out层。

解决办法：1、把两层都画上。

​         2、打孔的部分切掉，

![img](https://img-blog.csdnimg.cn/ee973972cbac416381d91ab0e21ddca8.png)



举例：先在机械层选中这个孔， 然后把这一部分区域切掉。

![img](https://img-blog.csdnimg.cn/0d19dce0e7a94fa0a900620c63228861.png)

 4、单层显示的设置

找到AD右下角Panels，点它。

![img](https://img-blog.csdnimg.cn/809440997bc946d0badc9c83f19e8a09.png)

 ![img](https://img-blog.csdnimg.cn/cd235a8b2c7d4a4691788504796fe79b.png)

 选择最后一个View Configuration，然后出来以下。通过它来设置单层，方便调整布线。

![img](https://img-blog.csdnimg.cn/8a726220c41647f29b2d7a0daa301934.png)

 5、寻找相似的，同步设置。Find Similar Objects ，多个一起设置，不需要单个逐步设置，提高效率。

![img](https://img-blog.csdnimg.cn/91d08a0d95a84c2b9a2ec4d92e8f1128.png)

 6、PCB库文件一键更新。

有时需要修改PCB文件库，又不想手动逐个去原理图更新，有个小方法，在画完PCB库的时候，一键自动更新。操作如下：

![img](https://img-blog.csdnimg.cn/1cf0f6e8919348799fbbaf5081527b54.png)

7、PCB查看3D效果时，可以按快捷键3，按V+B翻转。