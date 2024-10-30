测试文件v0.1
git init //初始化仓库
git config --global user.name "woaimao" //设置用户名
git config --global user.email "woaimao@qq.com" //设置邮箱
git add README.md //添加文件到暂存区
git commit -m "first commit" //提交暂存区文件到本地仓库，-m参数后面跟注释(备注)
git branch -M main //创建分支并切换到main分支，-M参数强制重命名分支
git remote add origin https://github.com/woaimao/test.git //关联远程仓库地址
git push -u origin main //推送到远程仓库,-u参数关联远程仓库和本地分支,main为远程分支名,origin为远程仓库名,第一次推送需要加上-u参数,之后推送直接git push,不用再加-u参数


git push //推送到远程仓库
git fetch origin //拉取远程仓库代码，不合并，只下载，不更新本地仓库，只更新远程仓库
git pull origin main //拉取远程仓库代码，并合并到本地仓库，更新本地仓库，不更新远程仓库
git pull //拉取远程仓库代码
git clone https://github.com/woaimao/test.git //克隆远程仓库，下载到本地

git diff //查看文件差异
git diff --cached //查看暂存区文件差异
git log //查看提交历史（日志）
git branch //查看当前分支
git branch -a //查看所有分支,-a参数显示远程分支,本地分支,以及已经合并或丢弃的分支
git branch -d 分支名 //删除分支
git branch dev //创建dev分支
git checkout -b dev //创建并切换到dev分支
git checkout main //切换到main分支
git merge dev //合并dev分支到当前分支
git branch -d dev //删除dev分支
git push origin --delete dev //删除远程dev分支
git push origin --delete main //删除远程main分支

git remote -v //查看远程仓库地址
git status //查看仓库状态
git stash list //查看暂存区列表
git stash pop //恢复暂存区文件
git stash drop //删除暂存区文件
git stash clear //清空暂存区

git rm 文件名 //删除文件
git mv 文件名 文件名2 //重命名文件
git commit --amend //修改最后一次提交
git reset HEAD^ //回退到上一次提交
git reset HEAD^^ //回退到上上一次提交
git reset --hard HEAD^ //回退到上一个版本，hard参数表示强制回退
git reset --hard HEAD^^ //回退到上上个版本
git reset --hard 版本号 //回退到指定版本,版本号可通过git log查看

1
