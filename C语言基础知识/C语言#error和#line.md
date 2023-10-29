### C语言#error和#line

##### #error

#error用于生成一个编译错误消息，并停止编译

![image-20231025203158356](文档中本地图片/image-20231025203158356.png)

示例：

随便找了一个工程测试下#error

看图中我圈起来的部分，编译器提示warning和error。看我的程序如果没有定义TEST_#ERROR这个宏，编译器会报错You did not define the relevant macro

![image-20231029092956728](文档中本地图片/image-20231029092956728.png)



#line

#line用于强制指定新的行号和编译文件名，并对源程序代码重新编号

![image-20231028191930853](文档中本地图片/image-20231028191930853.png)