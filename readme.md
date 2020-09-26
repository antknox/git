1.设置用户名和密码

git config --global user.email "you@example.com"

git config --global user.name "Your Name"

2.生成密钥对

ssh-keygen -t rsa -C "your_email@youremail.com"

3.配置公钥到git

用户目录/.ssh

设置 SSH and GPG keys

4.验证密钥

ssh -T git@github.com

5.查看remote url

git remote -v

6.创建本地仓库

mkdir test

cd test

git init

7.添加远程仓库

git remote add origin git@github.com:user/test.git

8.创建文件

touch readme

git add .

git commit -m "add readme"

9.推送本地仓库到远程仓库

git push -u origin master

10.克隆远程仓库

git clone git@github.com:user/test.git

11.进入仓库

cd test

12.创建文件

touch readme

git add .

git commit -m "add readme"

13.推送本地仓库到远程仓库 新文件

git push -u origin master

14.进入本地仓库

cd test

15.添加本地仓库到远程仓库

git remote  rename origin old-origin

git remote add origin git@github.com:user/test.git

git push -u origin --all

git push -u origin --tags

16.查看状态

git status

17.创建分支

git branch branch_name

18.切换分支

git checkout branch_name

19.提交分支

git add .

git commit -m "branch_name"

git push -u origin branch_name

20.拉取远程仓库

git checkout master

git pull origin master

21.合并分支

git merge origin/branch_name

git add .

git commit -m "master+branch_name"

20.查看状态

git status

21.提交合并分支

git pull origin master
