# work
收集作业，小任务
学习git，提高工作效率

1. git checkout -- .\LICENSE.txt  
    场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。
    场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD <file>，就回到了场景1，第二步按场景1操作。
2. 查看工作区和版本库里面最新版本的区别：git diff HEAD -- readme.txt 
3. 删除文件（从版本库）：git rm <file>
    一是确实要从版本库中删除该文件，那就用命令git rm删掉，并且git commit。
    另一种情况是删错了，因为版本库里还有呢，所以可以很轻松地把误删的文件恢复到最新版本：
4. 远程仓库：
    要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；
    关联后，使用命令git push -u origin master第一次推送master分支的所有内容；
    此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；
    克隆：git clone git@github.com:michaelliao/gitskills.git
5. 分支管理：
    查看分支：git branch
    创建分支：git branch <name>
    切换分支：git checkout <name>
    创建+切换分支：git checkout -b <name>
    合并某分支到当前分支：git merge <name>
    删除分支：git branch -d <name>