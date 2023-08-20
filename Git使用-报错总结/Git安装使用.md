### windows 11 下安装git，上到资源到GitHub

 一、我们需要去官网下载git，并安装。

下载链接如下：

https://git-scm.com/

![img](https://img-blog.csdnimg.cn/3f27f75d9ee449bfb47a2d7d97cde4eb.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 点进去，选择64位

![img](https://img-blog.csdnimg.cn/b2becd8868a94ec98f666c032e076f06.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

下载完成后点击安装，直至完成。

二、绑定信息

首先，我们在桌面上新建一个文件夹，用于测试使用git上传文件，里面随便放一个文本文件

，然后点进这个文件夹

 ![img](https://img-blog.csdnimg.cn/2fad4168125740f68439a114a4723982.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 使用windows11 的同学请注意，右击鼠标，点进显示更多选项，然后再点进 Git Bash Here。![img](https://img-blog.csdnimg.cn/d658a30205244959ac208fceb99ef817.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 ![img](https://img-blog.csdnimg.cn/df282e03a51d4a5fb26e1d9d05edc3ed.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 会出现以下窗口，如图。

![img](https://img-blog.csdnimg.cn/1341f9c35f314ce79577c85cc7938646.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 接下来，我们来绑定自己的信息邮箱，我之前绑定过，这里删除一下。

> git config --global --unset-all

 然后我们开始绑定信息

> git config --global user.name "换成自己的github名字"
>
> git config --global user.email "换成自己的邮箱"

 ![img](https://img-blog.csdnimg.cn/57a0341a470f4c50bfceaa238198e16a.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 然后，命令如下：

> git init .
>
> git add .
>
>  git commit -m "feat():测试"
>  

接下来，我们打开github新建仓库，点击New。

![img](https://img-blog.csdnimg.cn/d65135f660a5439a9c0757b270f1c0ff.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 配置如下，注意public是开源，private是自己可见，然后下一步。![img](https://img-blog.csdnimg.cn/07c8abe607b24dd398538a0514bed2f1.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑



 然后我们进入这个页面，会有代码命令提示

![img](https://img-blog.csdnimg.cn/2d8b71de3b7d46ffbf7faf3572e47d5f.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 把本地项目推上去

>  git remote add origin git@github.com:qq-hh/hello_github.git 注意这里换成自己的ssh链接
>
>  git push -u origin master 推到仓库
>
> git pull origin master  仓库下拉代码
>  

![img](https://img-blog.csdnimg.cn/2871934bf278454b8f0e7ce2e5f9b298.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 然后，我们刷新GitHub仓库页面，代码已提交上去啦。

![img](https://img-blog.csdnimg.cn/a659c53667294de89f15206d8fa6b4cd.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

到此完成，给自己点个赞吧~ 

![img](https://img-blog.csdnimg.cn/5637741c768548f5b6d6d6bc50724d08.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑