# git学习笔记

### git初始化账号和邮箱

```bash
git config --global user.name "qianfu"   (用户名)
git config --global user.email 1733034367@qq.com (邮箱)
git config --global credential.helper store (保存账号密码)
git config --global --list (查看配置信息)
```

### git创建仓库

```bash
mkdir learn-git
cd learn-git
git init
```

## 创建文件

```bash
 git status (查看当前状态)
 echo "hello world" > hello.txt (创建一个文本)
 git status (查看当前状态会发现多了一个文件)
 git add hello.txt (添加文件到暂存区)
 git commit -m "这是第一次提交" (提交文件到仓库,注意如果不加-m解释说明就会自动跳到vim编辑器界面让你填写操作信息)//(而且每一次提交只会提交暂存区的文件)
 git add *txt (添加所有txt文件到暂存区)
 git add . (添加所有文件到暂存区)
 git log (查看提交记录)
 git log --oneline (查看提交记录,一行显示)
 git reset --soft 回退到某一个版本并且保存工作区和暂存区的所有修改内容
 git reset --hard 回退到某一个版本并且不保存工作区和暂存区的所有修改内容
 git reset --mixed 回退到某一个版本并且保存工作区的所有修改内容,不保存暂存区的修改内容
 git reset --hard 版本号 (回退到某一个版本)
 git diff (查看工作区和暂存区的不同)
 git diff --cached (查看暂存区和仓库的不同)
 git diff HEAD (查看工作区和仓库的不同)
 git diff 版本号 版本号 (可以比较两个版本之间的不同)
 git diff HEAD~N HEAD 表示比较

 

```
## 删除文件

```bash
rm 文件名 (删除文件)
 git add 需要删除的文件名(这个与上一个操作配套,从暂存区删除文件)
 
 git commit -m "删除文件" (提交删除文件的操作)
```

## 远程仓库(github)

```bash
git pull (把远程仓库的代码拉取到本地)
git push (把本地仓库的代码推送到远程仓库)
```





