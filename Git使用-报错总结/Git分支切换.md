### Git分支切换 



新建分支前，先看一下目前是在哪个分支。可以看到下图我是在master分支上。

![img](https://img-blog.csdnimg.cn/840e27bcd6d644beb601db4a2f7dcd22.png)

使用以下命令创建新分支，并切换到新分支。

>  git checkout -b main 创建main分支并切换到main，main可以换成别的名字

![img](https://img-blog.csdnimg.cn/5e3804bbd17241588fb9d0f2268bf86a.png)

呜呜，出现了以下报错，打了好几遍命令都不行~~

![img](https://img-blog.csdnimg.cn/684e1b6c8fa746d8a92543c782e4d5d1.png)![点击并拖拽以移

 切换完分支后，发现报错（注意：切换到的分支上有文件，我没有pull下拉到本地仓库）：

> error :failed to push some refs to 'git.....'

经查找， 一定要注意切换分支，一定要先拉取在上传，即：

> git pull origin main
>
> git init .
>
> git add .
>
> git commit -m ""
>
> 然后 git push origin main 
>
> 完成！！！

![img](https://img-blog.csdnimg.cn/f58cc6187b704a7381b2e8e156013658.png)

又不符合写作规范，不知道是不是字数不够呢，多打一点点字，硬凑字数，哈哈哈！ 