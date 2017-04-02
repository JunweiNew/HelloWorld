github 使用新手入门使用笔记

1.ssh服务安装
	sudo apt-get install openssh-server

2.启动ssh
	sudo /etc/init.d/ssh start

3.关闭防火墙
	sudo ufw disable

检查安装成功与否
	ssh localhost
进程查看
	ps -e | grep ssh

生成ssh-key
	ssh-keygen -t rsa -C "niujunwei2012@126.com"

cat /home/linux/.ssh/id_rsa.pub 
	
申请github账号，点击账号下的Settings,点击SSH and GPG keys，点击New SSH
key,将id_rsa.pub下的key添加进去

git 安装
	sudo apt-get install git 

配置用户名和邮箱
	git config --global user.name "niujunwei"
	git config --global user.email "niujunwei2012@126.com"

复制一个git项目
	git clone git@github.com:workalone/HelloWorld.git 

编辑项目
	..........

添加代码
git add --all

git commit -m "注释"

git push origin master




============================================================================================
git 恢复commit
	git reset --hard <commit_id>


