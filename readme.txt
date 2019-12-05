结构：工作区 -- 暂存区(stage) -- 分支(如master)

cd 进入需要管理的文件目录
git init #初始化

git status #查看状态
git diff <file> #查看有什么变化

git add <file> #加入暂存区
git commit -m "message" #提交

git log #查看历史版本
git reflog #查看存在过的所有的版本
git reset --hard HEAD^ #回到上一个版本
git reset --hard 版本号 #回到某个版本

git checkout --<file> #想丢弃工作区的修改时（此时没有放入暂存区），回到最近一次git commit或git add时的情况
git reset HEAD <file> #放入了暂存区，还没有commit时，可以使用此命令，再用git checkout --<file>撤销工作区的修改

git remote add origin git@github.com:user-name/repo-name.git #关联远程库
git push -u origin master #第一次推送master分支的所有内容
git push origin master #之后每次推送最新修改
git clone git@github.com:server-name/repo-name.git #从github克隆

git branch #查看分支
git branch <name> #创建分支
git checkout <name> #切换分支
git checkout -b <name> #创建+切换分支
git merge <name> #合并指定的分支到当前分支
git branch -d <name> #删除分支

