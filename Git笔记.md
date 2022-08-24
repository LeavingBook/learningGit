# Git笔记

## 1. Git简介

Git 是一个免费的、开源的**分布式版本控制系统**，可以快速高效地处理从小型到大型的各种项目。同时，Git也是目前世界上最先进的分布式版本控制系统。

* 版本控制：

  > 版本控制是一种记录文件内容变化，可以记录文件修改历史记录，从而让用户能够查看历史版本， 方便版本切换。

* 集中式版本控制：

  > 版本库集中存放在中央服务器,修改时必须从中央服务器取出最新文件，进行修改更新，然后再上传到中央服务器中

* 分布式版本控制：

  > 分布式版本控制系统没有中央服务器，客户端提取的不是最新版本的文件快照，而是把代码仓库完整地镜像下来（本地库），每个客户端的每一次文件提取操作，实际上都是一次 对整个文件仓库的完整备份。

* 四个区域：
  
  > 工作区(workspace)： 直接写好的代码，以文件形式存在硬盘上的，即保存在本机工作区。
  > 暂存区(index/stage)： git add之后会存入暂存区。
  > 本地仓库(repository)： git commit之后会存入本地仓库。
  > 远程仓库(remote):：git push 之后会存入远程仓库。
  
  ![fa191e879d4449fbb7fcd469953a4623](.\fa191e879d4449fbb7fcd469953a4623.png)
  
  

## 2. Git常用命令

配置个人Git信息：

```bash
git config --global user.name "xxxx用户名"
git config --global user.email "xxxx.com邮箱"
git config --global user.password "xxxxx密码"
```

查看个人Git信息：

```bash
git config user.name      #用户名
git config user.password  #密码
git config user.email     #邮箱
```

查看本地库的所有配置：

``` bash
git config --list
```

初始化本地库：

```bash
git init #该命令将所在目录初始化一个能用Git管理的仓库，若在windows下需保证绝对路径中不含中文
```

查看本地库状态：

```bash
git status
```







