## 一、基本命令　

### 1.安装服务

```shell
mysqld --install
```	

### 2.初始化

```
mysqld --initialize --console	
```

### 3.开启服务
```
net start mysql
```

### 4.关闭服务
```
net stop mysql
```

### 5.登录mysql：
 ```
 隐藏密码：mysql -u root -p
 显示密码：mysql -uroot -proot
 ```

### 5.1退出MySQL
```
exit;
```
	
### 6.修改密码
```
alter user 'root'@'localhost' identified by 'root';(by 接着的是密码)
```

### 7.标记删除mysql服务：
```
sc delete mysql;
```

### 8.查看有哪些数据库：
```
show databases;
```

- mysql自带了4个数据库		

|     Database       |
| -----------------  |
| information_schema | 
| mysql              |  
| performance_schema | 
| sys                | 
  
  
## 9.使用某个数据库 
```
use student;
会显示：Database changed;
```
	
### 10.创建数据库
```
create database student;
```

### 11.选中后数据库后查看表
```
show tables;
```

### 12.导入表
```
source D:\ProgramData\SQLProject\bjpowernode.sql;
1.需要先选中数据库
2.路径不能有中文
```

### 13. 不看数据，只看表的结构
```
desc 表名; 等价于 descript student;
```

### 14.查看当前MySQL版本号
```
select version();
```
查看当前所使用的数据库
```
select database();
```

### 15.终止输入：  
```
mysql> show  
->  
->  
->  
->  
->  
-> \c  
mysql>  
```
