##Github提交工程
1.首先在GitHub上创建一个仓库，把地址复制下来，如：https://github.com/my/test.git

2.右键桌面打开GitBash，cd到要提交的项目根目录下，输入git init命令初始化仓库，在项目文件夹下出现.git文件夹

3.关联远程仓库：git remote add origin https://github.com/my/test.git（后面是你的仓库地址）

4.git pull origin master --allow-unrelated-histories
将工程项目文件同步到本地（--allow-unrelated-histories为防止提交错误，第二次提交可不用加）

5.使用命令git add . 添加所有文件到暂存区---在修改代码之后，可以使用git add MainActivity.java（后面是你修改过的文件） 添加修改的文件到暂存区

6.git commit -m "first commit"，提交代码

7.我们可以通过命令git status来查看是否还有文件未提交，如果有红色文字出现，说明还有文件未提交

8.git push -u origin master （推送到远程仓库），由于远程库是空的，我们第一次推送master分支时，加上了 –u参数，Git不但会把本地的master分支内容推送到远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时，只要做了提交就可以使用命令git push origin master进行推送。