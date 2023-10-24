更新镜像源：sudo apt update  
安装openssh-service：sudo apt install openssh-service  
安装文本编辑器vim：sudo apt install vim  
修改ssh配置文件：sudo vim /etc/ssh/sshd_config  
![network error](https://github.com/mcslll/note/blob/main/image/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-24%20103632.png?raw=true)  
查看ssh状态：service sshd status  
![network error](https://github.com/mcslll/note/blob/main/image/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-24%20105159.png?raw=true)  
设置liunx网络地址，达到双方能互相ping通就行  
打开vscode，安装Remote-SSH 安装完成后  
1、点击左下角打开远程窗口  
2、连接到主机-添加新的ssh主机（输入格式（liunx用户名@ip地址）（查看liunx用户名命令：whoami））  
3、选择输入主机信息的保存路径（默认第一个）  
4、再次点击左下角打开远程窗口  
5、连接到主机-选择刚才输入的ip地址-在新窗口中输入用户的密码-连接成功
