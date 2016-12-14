# git 笔记

## 所有命令前 先配置好秘钥

```
ssh-keygen -t rsa -C "email"

```
## window下需要先配置用户

```
git config --global user.name "evilpeanuts"
git config --global user.email "**@qq.com"
git config --global push.default simple


```

## copy 一个项目到本地

```
git clone https://github.com/evilpeanuts/test.git

```
## git 基础命令

```

git init                    // 把文件变成可执行的git文件
git add x                   // 检测文件夹下面文件 x     git add . 检测所有
git commit -m "first commit"//  提交已修改的并注释
git remote add origin https://github.com/evilpeanuts/test.git // 与远程分支建立联系
git push -u origin master   // 提交 -u 默认主机   以后直接 git push

git branch                  // 查看分支
git branch gh-pages         // 创建分支
git checkout gh-pages       // 进入gh-pages 分支
git fetch origin master     // 相当于是从远程获取最新版本到本地，不会自动merge
git pull origin master      // 相当于是从远程获取最新版本并merge到本地
git merge master            // 它会自动把master主分支之后的最新提交merge到你当前的develop分支上


```
