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
    