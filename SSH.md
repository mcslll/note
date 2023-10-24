一、更新镜像源：sudo apt update  
二、安装openssh-server：sudo apt install openssh-server  
三、安装文本编辑器vim：sudo apt install vim  
四、修改ssh配置文件：sudo vim /etc/ssh/sshd_config  
![network error](https://github.com/mcslll/note/blob/main/image/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-24%20103632.png?raw=true)  
五、查看ssh状态：service ssh status（绿灯-Active: active (running)表示正在运行）  
<开启SSH服务命令：sudo service ssh start>  
<关闭SSH服务命令：sudo service ssh stop>  
六、设置liunx网络地址，达到双方能互相ping通就行  
七、打开vscode，安装Remote-SSH 安装完成后  
_1、点击左下角打开远程窗口  
_2、连接到主机-添加新的ssh主机（输入格式（liunx用户名@ip地址）（查看liunx用户名命令：whoami））  
_3、选择输入主机信息的保存路径（默认第一个）  
_4、再次点击左下角打开远程窗口  
_5、连接到主机-选择刚才输入的ip地址-在新窗口中输入用户的密码-连接成功  
八、配置密钥实现免密登陆  
_1、windows>ssh-keygen -t rsa -C "xxx@xxx.com"（生成公钥文件-id_rsa.pub，私钥文件-id_rsa)  
_2、将公钥文件复制到liunx中（可以直接复制，可以使用scp命令-格式：scp id_rsa.pub的绝对路径 username@ip地址：路径）  
_3、liunx>ssh-keygen -t rsa -C "xxx@xxx.com" (xxx@xxx.com要和windows上的一致)   
_4、liunx>cat id_rsa.pub >> ~/.ssh/authorized_keys
