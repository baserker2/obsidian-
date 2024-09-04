find -name 以name查找文件
nautilus ./.cache/vmware/drag_and_drop/St9PSE 图形界面打开文件夹
file 查看文件属性
mv 移动文件夹
./文件名   执行程序

chmod 777 文件读写权限（RWX）
[Linux常用命令：chmod修改文件权限 777和754-CSDN博客](https://blog.csdn.net/pythonw/article/details/80263428)


重置网络
sudo service NetworkManager stop
sudo rm /var/lib/NetworkManager/NetworkManager.state
sudo service NetworkManager start
