###  git报错: Unable to create ‘D:/github开源/My_Project_stm32/.git/index.lock‘: File exists.

今天在push代码的时候，上传不了，不知道是不是里面有PDF文件的原因，删除之后也无法上传，报错如下：

![img](https://img-blog.csdnimg.cn/f9b5cdb013ed4547bfad850884763804.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 报错提示：一个git进程正在储存库中运行，比如用git commit打开编辑器。确认所有流程终止，在重试。如果仍上传失败，则git进程可能在储存库中崩溃。

点开本地仓库文件夹，进入git，将index和index.lock.文件删除。

![img](https://img-blog.csdnimg.cn/738c9fb41b6f47a9b4048b4ff23101f3.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 再次报错

![img](https://img-blog.csdnimg.cn/8ea7ea2cea804342b2408a1884d2ec71.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 删除git文件夹，重新连接远程仓库初始化

git add 报错

![img](https://img-blog.csdnimg.cn/cde9cb71c67948e9a208ee38b1037d6e.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 输入 git config --global core.autocrif false重新开始

![img](https://img-blog.csdnimg.cn/4b38775d020f4a6a9d0cde332be515b4.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 先pull下拉代码，在push 还报错

![img](https://img-blog.csdnimg.cn/462901f6b1d14d47b02df1b47ccf5775.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 解决办法  git pull origin master --allow-unrelated-histories

![img](https://img-blog.csdnimg.cn/ce96967bf5ac44908c8b2e8df244580d.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 在初始化上传，能上传到远程仓库，但是有三个warning![img](https://img-blog.csdnimg.cn/8ca976a0c2714beb8ba012ca2ace2c1a.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

 这是因为单个文件超过100M，push代码会报错。GitHub不允许直接上传大文件（超过100M）的文件到远程仓库，若要想继续提交可以尝试使用大文件支持库：[https://git-lfs.github.com](https://link.jianshu.com/?t=https%3A%2F%2Fgit-lfs.github.com)

需要安装git - ifs扩展，具体参考这里[Github超过100M的大文件上传 - 简书 (jianshu.com)](https://www.jianshu.com/p/7d8003ba2324)