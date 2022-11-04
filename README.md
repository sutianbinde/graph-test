
```
# 将本地静态网页项目的文件夹变成用git管理的本地仓库
git init
# 查看所有文件，多出 .git 文件
ls -al

# 新建后对项目进行介绍
touch README.md
# 新建后可以写入后续不想提交到GitHub上的文件
touch .gitignore

# 列出所有本地分支和远程分支，仓库默认在 master 分支
git branch -a

# 新建并切换到 gh-pages 分支
git checkout -b gh-pages

# 显示有变更的文件
git status

# 删除 master 分支
git branch -d master

# 添加当前目录的所有文件到暂存区
git add .

# 提交暂存区到仓库区，并添加代码提交信息
git commit -m 'first commit'

# 添加远程仓库
git remote add origin git@github.com:DesertsX/yulequan-relations-graph.git

# 把本地的 gh-pages 分支推送到 origin 服务器上
git push origin gh-pages
```