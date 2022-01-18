# Ubuntu 20.04 添加sudo权限

## 添加xigua用户sudo权限

### 方法一：添加到sudo组

`user mod -a -G sudo xigua`

方法二：visudo编辑

xigua ALL=(ALL:ALL) NOPASSWD: ALL

## sudo免密

`visudo`

%sudo ALL=(ALL:ALL) NOPASSWD: ALL





visudo 详细说明

字段1: 用户名  %开头为用户组

字段2 允许登陆的主机 ALL表示所有

字段3 表示sudo可以提权到的用户和用户组 ALL表示所有，省略为root：root

字段4 可以为NOPASSWD： 表示执行sudo不需要密码



