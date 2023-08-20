 ![img](https://img-blog.csdnimg.cn/b32e6e29f25c4facb3f70d65148690b1.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑 git报错如下：

> Connection reset by 140.82.113.4 port 22
>  fatal: Could not read from remote repository.
>
> Please make sure you have the correct access rights
>  and the repository exists.

遇到这个报错，我按照百度方法一，重新绑定SSH。结果不行，呜呜呜~~~

> ssh-keygen -t rsa -C  "自己的邮箱"

然后打开github官网更新SSH

![img](https://img-blog.csdnimg.cn/056d28932e9344e18089b426dc113be4.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

之后找到方法二，看能不能ping通github，可能是网络连接不是git

> ping github.com 

![img](https://img-blog.csdnimg.cn/c7469b893d43455491bdefdb7c000855.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 不是这个问题，github可以ping通。

之后查找，发现可能是网络的问题，我用手机开了热点，再次使用上传命令，搞定！！！

![img](https://img-blog.csdnimg.cn/cb8b27e775e94a8d84f5b2e088426a6a.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑