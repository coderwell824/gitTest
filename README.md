

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
