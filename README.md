# POC-available
POCs can run in some Linux kernel versions  
## CVE-2019-11599  
POC运行内核版本：4.6.2  
运行方式：  
gcc -o coredump_helper coredump_helper.c  
sudo ./set_helper.sh  
gcc -o dumpme dumpme.c  
./dumpme  
运行结果：  
运行poc  
![image](https://github.com/HaleyWei/POC-available/blob/master/Image/pg1.png)  
通过dmesg查看日志  
![image](https://github.com/HaleyWei/POC-available/blob/master/Image/pg2.png)  

## CVE-2019-9213  
POC运行内核版本：4.6.2  
运行方式：  
gcc -o nullmap nullmap.c  
./nullmap  
运行结果：  
![image](https://github.com/HaleyWei/POC-available/blob/master/Image/pg3.png)  

## CVE-2019-13272  
POC运行内核版本：4.15.0-29  
运行方式：  
gcc -s poc.c -o exp  
./exp  
运行结果：  
获得root权限  
![image](https://github.com/HaleyWei/POC-available/blob/master/Image/pg4.PNG)  

## CVE-2018-18955
POC运行内核版本：4.15.x < 4.19.2  
运行方式：./exploit.polkit.sh  
运行结果：  
获取root权限  
![image](https://github.com/HaleyWei/POC-available/blob/master/Image/pg5.png)
