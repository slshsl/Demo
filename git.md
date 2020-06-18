# git 常用命令

<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [git 常用命令](#git-常用命令)
  - [获得配置](#获得配置)
  - [添加远程连接](#添加远程连接)

<!-- /code_chunk_output -->

## 获得配置
- git config --list/-l

```code{.line-numbers,highlight=[38,39,46]}
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
user.name=slshsl
user.email=slshsl@qq.com
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
credential.helper=store
gui.recentrepo=E:/WebLearn/Repository/Demo
core.safecrlf=false
core.repositoryformatversion=0
core.filemode=false
:...skipping...
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
user.name=slshsl
user.email=slshsl@qq.com
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
credential.helper=store
gui.recentrepo=E:/WebLearn/Repository/Demo
core.safecrlf=false
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=https://github.com/slshsl/Demo.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
gui.wmstate=normal
gui.geometry=668x483+736+324 202 185
branch.master.remote=origin
branch.master.merge=refs/heads/master
```
>上面第38、39行，添加用户名和邮箱一般在全局里配置
>上面第46行是为解决在windows系统下回车换行与linux系统下的换行不同，没有此配置在`git add .`时会有警告信息

## 添加远程连接
- git remote add [源名称：origin] [远程仓库地址：url]
- git remote -v:查看远程连接
### 添加github远程仓库方式
1. https
2. ssh
    需要执行`ssh-Keygen -t rsa -C "your email"`;然后将生成的公钥添加到github上