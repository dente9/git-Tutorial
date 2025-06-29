# 下载git

```
https://git-scm.com/downloads
```

# 配置用户名和邮箱

```
git config --global user.name your_user_name
git config --global user.email your_email_address

```

# 常用命令

```
git init
git status
git add
git commit -m "mesage"

```

## 删除暂存区的文件

```
git rm --cached file
```

## 查看日志

```
git log
git log --oneline
```

### 回退

```
git reset

```

接收三种参数,分别是

- git reset  --soft 保留工作区和暂存区的所有内容
- git reset --hard 丢弃工作区和暂存区的所有内容
- git reset --mixed 默认模式 保留工作区内容,丢弃暂存区内容

## 查看暂存区文件

```
git ls-files
```

## 查看所有操作

```
git reflog
```

## 查看差异diff

- git diff  默认是查看工作区和暂存区之间的差异
- git diff head 查看工作区和仓库之间的差异
- git diff --cached 查看暂存区和版仓库之间的差异
- git diff id_ id_1 查看两个版本之间的差异
- git diff head head~3 查看最新仓库与前3个版本之间的差异
- git diff head head~3 file.txt 查看指定文件的差异

## 配置密钥

```
ssh-kengen -t rsa
```

生成的.pub文件上传到服务器(公钥文件)

指定验证的自定义文件

```
Host github.com
HostName github.com
IdentityFile ~/.ssh/your_pub
```

## 关联本地和远程的仓库

```
git remote add origin git@github.com:dente9/remote.git  #远程仓库名,地址
git branch -M main #重命名分支名字
git push -u origin main # 远程仓库名,分支名字
git pull origin main  # 远程仓库名, 远程分支名字:本地分支名字 相同可省略冒号后面部分
```

## 分支

```
git branch #查看分支
git branch name # 创建分支
git checkout dev #切换分支
git switch dev
git merge dev #在主分支里面合并其他分支
git branch -d dev # 删除合并后分支
git branch -D dev # 强制删除分支,无论合并与否
```

## 合并分支

```
git merge --abort

```
