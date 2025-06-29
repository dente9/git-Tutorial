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
