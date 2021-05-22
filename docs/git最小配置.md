### 最小配置

安装git后进行初始化配置

* git config --global usr.name 'usr_name'
* git config --global usr.email 'usr_email'

通过loacl、global、system控制配置的作用域

* git config --local   针对当前仓库的配置
* git config --global  针对当前用户的配置
* git config --system  针对所有登陆系统用户的配置

通过添加--list选项查看当前配置 exp:

* git config --local --list
