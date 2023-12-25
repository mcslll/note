从TFTP服务器下载文件：  
tftp -g -l localfile -r remotefile HOST [PORT]  
将文件上传到TFTP服务器：  
tftp -p -l localfile -r remotefile HOST [PORT]  
自定义块大小进行文件传输：  
tftp -g -l localfile -r remotefile -b 512 HOST [PORT]  
其中，localfile 是本地文件名，remotefile 是远程文件名  
