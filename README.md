学习Git命令的使用

1、主要参考网站：https://www.runoob.com/git/git-basic-operations.html

2、常见命令:
    git clone   ---- 克隆远程代码库到本地
    git add  ----  添加本地文件到缓存区
        git add .  ---- 添加所有修改和新建的数据到缓存区
        git add -u ---- 提交所有被删除和修改的文件到缓存区
    git status  ----- 显示所有有变更的文件
        git status -s   -----  更加详细一些
    git diff HEAD  ----- 查看已缓存和未缓存的所有变动
    git diff --cached  -----  查看已缓存的所有变动
    git commit -m 'xxxx'   -----  将暂存区内容添加到本地仓库

3、case
    我们在本地新建了hello_cc.cpp文件，之后执行 git add hello_cc.cpp, git commit -m 'add cpp file'
    通过git log --oneline 可以查看到本次提交的日志
    此时，如果我们需要修改这个cpp文件，修改后同样可以和之前一样，add  commit，但是git log时会发现有两条日志！！
    因为我们修改的是同一个文件，不想日志过多，此时可以先git add ，然后执行
    git commit --amend --no-edit   ---- 将上一次add commit的文件进行本地修改后，可以使用这条命令
    