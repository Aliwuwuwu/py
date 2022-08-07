# Git
简介：git是一个分布式控制系统可以便利的管理文件，能让他人一起修改文件且别人的任何改动都有记录
指令：
1. `git config`配置git相关参数 
2. `git clone` 从远程仓库克隆一个版本到本地
3. `gti init` 初始化项目且会在目录留下叫做git.的目录
4. `git status` 查看本地仓库状态
5. `git remote` 控制远程库
6. `git branch` 操控git分支
7. `git checkout` 检出命令，用于创建、切换分支
8. `git cherr-pick` 把已经提交的记录合并到当前分支
9. `git commit` 将暂存区里的文件提交到本地仓库
10. `git push` 将本地仓库的文件提交到远程仓库
11. `git add` 将文件提交到暂存区当使用git commit时将暂存区的文件的内容上传

### git 提交常规流程
1. `git add .`
2. `git status`
3. `git commit -m "本次更改内容（英文）"`
4. `git push`