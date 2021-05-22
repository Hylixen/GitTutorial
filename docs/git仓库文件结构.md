# Git仓库文件结构

* config  存放local配置
* HEAD  存放当前分支head
* refs  存放heads与tags
* logs  存放log
* objects  存储对象

使用git cat-file -t 查看对象类型，git主要有commit、tree、blob三种文件类型  
<div align="center"><img src='../pics/filestructure.png' alt=''> </img></div> 
使用git cat-file -p 查看对象内容  
<div align="center"><img src='../pics/gitfiles.png' alt=''> </img></div> 

每次commit对应一个tree，tree下有子tree或blob，bolob为实际文件，相同内容文件通过hash在仓库中仅有唯一一个，提高了存储效率。git作为分布式版本管理系统，记录了每个版本重建信息，每一个仓库都可以完整恢复已获取的版本。
