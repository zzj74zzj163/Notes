# git 快速上手指南#

![git work flow ](/image/git%20work%20flow.png "workflow")

## git 配置 用户名和邮箱可以不真实
>git config --global user.name "xxxx"
>git config --global user.email "xxx@163.com"


## 把当前文件位置作为git工作区
>git init 
完成后本地会多一个.get的隐藏文件夹

## 查看状态
>git status

## 把对应工作区文件添加到缓存区
>git add xx.txt
>git add . //添加全部文件

## 把文件改动上传到本地仓库
>git commit -m"把文件改动上传到本地仓库"

>git commit -am"把所有文件添加到缓存区然后上传到本地仓库"

## 版本修改信息查看

>git log

按q退出信息界面

## 非工作区文件管理

>.gitignore 
创建该文件 并把对应文件名写在这个文件里，git就会忽略管理这些文件了

## 创建分支xxx
>git branch xxx

## 查看分支信息
>git branch

## 切换到xxx分支
>git checkout xxx

## 删除xxx分支，merge后才可运行
>git branch -d xxx
## 不管是否merge，直接删除xxx分支
>git branch -D xxx 

## 当前分支与目标分支xxx合并
>git merge xxx

## 复制远程仓库到本地
>git clone 仓库地址

## 添加远程仓库
>git remote 仓库名称（自己定） 仓库地址

## 查看远程仓库对应地址
>git remote -v

## 把远程仓库拉到本地仓库，可以指定远程仓库和分支名称
>git fetch

## 对比远程仓库和分支的区别
>git fetch 远程仓库/分支

## 对比后没问题可以直接pull到工作台上
>git pull

## 把本地仓库push到远程仓库进行合并
>git push 