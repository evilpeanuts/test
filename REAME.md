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
