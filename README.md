# work
收集作业，小任务
学习git，提高工作效率

1. git checkout -- .\LICENSE.txt  
    场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。
    场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD <file>，就回到了场景1，第二步按场景1操作。
2. 查看工作区和版本库里面最新版本的区别：git diff HEAD -- readme.txt 
3. 删除文件（从版本库）：git rm <file>