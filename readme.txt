1. mkdir learngit //新建文件夹
2. cd learngit //进入文件夹
3. pwd // 查看文件夹路径
4. git init // 把这个目录变成git可以管理的仓库
5. 然后可以新建readme.txt，编写内容
6. git add readme.txt // 把文件添加到仓库 
    git add .  // 把所有文件添加到仓库
7. git commit -m "wrote a readme file" // 把文件提交到仓库
8. git remote add origin https://github.com/chenrunmiao/learngit.git
9. git push -u origin master // 会报权限错误
	git@github.com: Permission denied (publickey).
	fatal: Could not read from remote repository.
	Please make sure you have the correct access rightsand the repository 	exists.
解决方法：删除当前key，重新生成key
1. ssh-keygen -t rsa -C "github注册邮箱"
2. 直接回车默认
3. 然后打开C:\Users\Administrator\.ssh里面的id_rsa.pub
4.打开github，登录个人账户，右上角settings —— SSH and GPG keys —— New SSH key
5. title随便写，key将id_rsa.pub复制进去
6. git push -u origin master  // 成功了

上传文件到github上
1. git add .   // 添加到本地仓库
2. git commit -m '描述'  // 添加提交描述
3. git pull origin master  // 提交前先从远处主仓库中拉取请求
4. git push -u origin master  // 把本地仓库代码提交