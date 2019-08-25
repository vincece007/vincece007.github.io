 ### 1.Pipenv 介绍
 pipenv解决了旧的pip+virtualenv+requirements.txt 的工作方式的弊端（因为requirements.txt 需要手动维护，使用上不够灵活）

 具体来说，它是pip、Pipfile、Virtualenv的结合体，它让安装包、包依赖管理和虚拟环境管理更加方便。
 ### 2.基本命令
 ###### 安装：
 pip install pipenv
 ###### 查看是否安装成功：
 pipenv --version
 ###### 启动虚拟化环境：
 pipenv shell （命令行前有虚拟环境名说明添加成功）
 ###### 退出：
 exit
 ###### 查看当前项目依赖包：
 pip list
 ### 3. 管理依赖包
 一个程序通常会使用很多的Python包，即依赖（dependency）。而程序不仅仅会在一台电脑上运行，程序部署上线时，需要安装到远程服务器上。

 如果你打算开源的话，就可能会有更多的人需要在他们的电脑上运行。为此，他们不得不记录下所有的依赖包，然后使用pip或Pipenv安装，这些重复无用的当然应该避免。

 而且requirements.txt 需要手动维护，使用上不够灵活。Pipfile的出现就是为了替代难于管理的requirements.txt。

 在创建虚拟环境时，如果项目根目录下没有Pipfile文件，pipenv还会在项目的根文件夹目录下创建Pipfile和Pipfile.lock文件。

 前者用来记录项目依赖包列表，后者记录了固定版本的详细依赖包列表。当我们使用Pipenv 安装/删除/更新 依赖包时，二者会自动更新。


 
