### 查询是否存在ssh
`cat ~/.ssh/id_rsa.pub`

### 生成ssh
```markdown
1. ssh-keygen -t rsa -b 4096 -C "邮箱"
2. 三次回车
```

### 获取本地ssh并绑定至git
`cat ~/.ssh/id_rsa.pub`

### 配置全局变量

```markdown
1. git config --global user.name "变量名"
2. git config --global user.email "邮箱"
3. 如果不配置后面会无法操作
```

### 从git上面下载数据

```markdown
1. git clone 仓库地址
2. git@github.com:xxxxxx
```

***`git支持Linux命令`***

### 提交至git

```markdown
1. git add -A  
		# 提交的内容，-A：all，也可以用.表示
2. git commit -m "本次提交的修改的备注"
3. git push origin 分支名(默认为master/main)
		# 第一次才需要输入分支名，后续可直接git push
		# 需要提交到其他的分支则填写分支名即可
4. git pull
		# 相当于并集，将远程仓库的内容同步至本地但并不覆盖
		# 如果有的内容本地没有则会下载至本地
		# 多人开发时提交之前最好使用一次
5. git commit -am "本次提交的修改的备注"
		# 1/2步骤合并
```

### 绑定远程仓库

```markdown
1. git init
		# 初始化项目目录，创建一个.git文件夹，没有这个无法提交
2. git remote -v
		# 查看当前项目是否绑定过远程仓库，如果绑定过则无法继续绑定
3. git remote add origin 仓库地址
		# 绑定远程仓库
4. git remote remove origin
		# 解除绑定
```

