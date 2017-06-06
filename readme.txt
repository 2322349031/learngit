git add readme.txt
git commit -m "wrote a readme file"
git status 查看仓库当前状态
git diff readme.txt 查看readme修改了哪里
git log  查看从最近到最远的日志
git log --pretty=oneline   查看从最近到最远的日志(简略版)
git reset --hard [commit id]   回到commit id对应的版本
工作区 add 暂存区 commit 版本库
git diff HEAD -- readme.txt    查看工作区和版本库的最新区别
git checkout -- readme.txt   把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
git reset HEAD readme.txt 把暂存区的修改撤销掉（unstage），重新放回工作区.
$ ssh-keygen -t rsa -C "youremail@example.com"   创建SSH key