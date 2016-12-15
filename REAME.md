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

# 查看、切换、创建和删除分支

```
git br -r  // 查看远程分支

git br <new_branch> // 创建新的分支

git br -v // 查看各个分支最后提交信息

git br --merged // 查看已经被合并到当前分支的分支

git br --no-merged // 查看尚未被合并到当前分支的分支

git co <branch> // 切换到某个分支

git co -b <new_branch> // 创建新的分支，并且切换过去

git co -b <new_branch> <branch> // 基于branch创建新的new_branch

git co $id // 把某次历史提交记录checkout出来，但无分支信息，切换到其他分支会自动删除

git co $id -b <new_branch> // 把某次历史提交记录checkout出来，创建成一个分支

git br -d <branch> // 删除某个分支

git br -D <branch> // 强制删除某个分支 (未被合并的分支被删除的时候需要强制)

```


# git暂存管理


```
git stash # 暂存

git stash list # 列所有stash

git stash apply # 恢复暂存的内容

git stash drop # 删除暂存区


```


# 回退版本


```

git reflog     //查看命令历史

git log        //查看提交历史

git reset --hard  commit_id   //HEAD指向的版本就是当前版本

```
