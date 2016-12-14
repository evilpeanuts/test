# test
# 修改
var a;
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/evilpeanuts/test.git
git push -u origin master
可以通过如下命令进行代码合并【注：pull=fetch+merge]
git pull --rebase origin master
git merge master，它会自动把master主分支之后的最新提交merge到你当前的develop分支上，如果不需要全部的提交，只需要个别的提交，可以执行 git cherry-pick  commitid(SHA值)git
