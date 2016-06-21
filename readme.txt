
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

git diff HEAD --readme.txt 可查看工作起和版本库里面最新版本的区别
git checkout --file 丢弃工作起的修改
git checekout --file 就是让文件回到最近一次 git comimit 或者git add 状态

git reset HEAD file 可以把暂存区的修改 撤销掉

场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。

场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD file，就回到了场景1，第二步按场景1操作。

场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考版本回退一节，不过前提是没有推送到远程库。


rm test.txt
git rm test.txt
git status
-------
git checkout --test.txt 
git checkout 其实是用版本库里的版本替换工作区的版本。
无论删除还是修改。都可以一键还原。

E:\itisi\mongodb\data\db

ssh-keygen -t rsa -C "321354544@qq.com"  生成密钥

git remote add origin git@github.com:itisi00/gitdemo.git
git push -u origin master
我们第一次推送master分支时，加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。
