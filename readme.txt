
git is a version control sysytem

git is free software
Unix的哲学是“没有消息就是好消息”

配置：
git config --global user.naem "your name"
git config --global user.email "your email"

mkdir learmgit
cd learngit
pwd 用于显示当前的目录

git init 把这个目录变成可以管理的仓库

ls -ah 可以显示隐藏的文件夹和目录

git add readme.txt
git commit -m 'wrote a readme file'

git add file.txt
git add file2.txt file3.ext
git commit -m "desc "

git status 查看当前仓库状态 
git diss readme.txt 查看修改内容

新增

git log 查看历史记录

git log --pretty=oneline 格式化，单行显示

准备撤销的

git reset --hard HEAD^  指向当前版本

cat readme.txt 查看文件内容

git reset --hard HEAD^  
git reflog 记录每一次命令
git reset --hard commit_id 任意回退

git is change
