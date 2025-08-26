git add source/_posts/linux.md  把修改添加到本地git
# 查看本地仓库的状态
$ git status

# 把指定1个或多个文件添加到暂存区中
$ git add <文件路径>

# 将工作区所有变化提交到暂存区，包括修改、新文件和删除文件。
$ git add . 
$ git add -A <文件路径>
$ git add --all <文件路径>

# 添加所有修改、已删除的文件到暂存区中，不包含新增文件
$ git add -u [<文件路径>]

git rm --cached source/_posts/git.md 只删除git中的记录，不删除文件本身
git rm -f source/_posts/git.md 会把我的文件也删除掉

1