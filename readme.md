# 打开vscode命令行工具

```
ctrl + `（ESC下面的符号）
```

## 本地源代码管理

1、生成一个git仓库

```shell
git init
```
命令执行后，会在当前的工作目录里生成一个.git文件夹，这个目录是当前项目的仓库文件夹，
以后不能删除这个目录，删除后，代码的记录就没了！

2、添加代码的变更文件到暂存更改里
```shell
git add <文件路径|文件夹路径>
```

3、提交暂存（确认存储）
```shell
git commit -m "描述"
```

4、查看分支
```shell
git branch
```

5、创建分支
```shell
git branch <分支名称>
```
6、删除分支
```shell
git branch -D <name>
```
7、合并分支

```
git merge <otherBranch>
```
8、在本地添加一个远程仓库的地址

```shell
git remote add <仓库名称> <仓库地址>

git remote add github https://xxx.git
```

9、删除远程仓库
```shell
git remote remove <仓库名称>
```

10、上传代码到远程仓库

```shell
git push <仓库名称> <分支名称>
```

11、绑定默认分支
```shell
第一次：
git push -u <仓库名称> <分支名称>
第二次以后
git push 
```

12、克隆项目

git clone <项目地址>

```
git clone https://github.com/xuzhciheng/webxxx.git
```
克隆的项目默认的远程仓库名称叫origin（原始仓库）
远程仓库地址：默认是当前克隆的地址

使用命令查看当前的仓库

```shell
#查看当前的仓库列表
git remote

#获取当前仓库的地址
git remote get-url remote
```

7、同步远程仓库

#拉取同步

```shell
git pull
```

8、下载分支

主分支已经克隆好了，现在要下载非主分支

```shell
git fetch <仓库名称> <远程分支名称>:<本地分支名称>
```
