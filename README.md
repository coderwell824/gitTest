

# gitTest

git pull=git fetch + git  merge

git branch --track origin/main

从远程仓库fetch代码: 从远程仓库获取最新的代码
默认情况下是从origin中获取代码
git fetch   git fetch origin master



![image-20221226114627540](/Users/coderwell/Library/Application Support/typora-user-images/image-20221226114627540.png)

![image-20221226163628871](/Users/coderwell/Library/Application Support/typora-user-images/image-20221226163628871.png)



git push origin main:远程分支   //推到远程分支

git config push.default upstream  修改git push的默认行为为上游分支
git config push.default current  修改git push的默认行为为远程分支, 找不到就创建远程分支 simple是找不到报错


git checkout -b test   //创建本地分支

![image-20221227143336595](/Users/coderwell/Library/Application Support/typora-user-images/image-20221227143336595.png)

git tag 查看标签列表(标签不受分支管理)
git show v1.0.0 查看指定标签的详细信息

git tag v1.0.0   创建本地标签   在push之前执行
git tag -d v1.0.0 删除本地标签
git push origin -d v1.0.0 删除远程指定分支

git push origin v1.0.0  推送单个标签到远程
git push origin --tags   推送所有的标签到远程

git checkout v1.2.0  检出指定tag, 还会创建对应的本地分支

![image-20221227160437300](/Users/coderwell/Library/Application Support/typora-user-images/image-20221227160437300.png)

---
git log 提交日志  --pretty=oneline  一行



![image-20221227171718792](/Users/coderwell/Library/Application Support/typora-user-images/image-20221227171718792.png)


git branch testing  创建本地分支
git branch  查看本地分支列表

git checkout -b testing 创建并切换本地分支

![image-20221227173304017](/Users/coderwell/Library/Application Support/typora-user-images/image-20221227173304017.png)

修复指定tag的bug
先checkout tag, 创建新的分支修复bug, 然后切换到main本地分支进行合并, git merge合并到的是本地分支

git merge test //先将切换到main本地分支, 将test本地分支合并到main本地分支

git branch -v 同时查看最后一次提交
git branch --merged 查看所有合并到当前分支的本地分支
git branch --no-merged  查看所有没有合并到当前分支的本地分支

git branch -d test  删除当前本地分支
git branch -D test  强制删除某个本地分支

 ![image-20221227191245261](/Users/coderwell/Library/Application Support/typora-user-images/image-20221227191245261.png)
 
git remote add origin 远程仓库地址    本地仓库连接到远程仓库
