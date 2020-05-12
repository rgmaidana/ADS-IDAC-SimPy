﻿﻿# ADS-IDAC-SimPy

基于Python开发的Maritime ADS-IDAC系统。
Maritime ADS-IDAC system is developed by Python.


# 系统开发架构

![系统架构](https://github.com/Eternal-Br/ADS-IDAC-SimPy/blob/master/%E5%BC%80%E5%8F%91%E6%96%87%E6%A1%A3/images/Framework.png)

## 如何使用本系统
1. 您的计算机系统需要安装Python 3 (3.6或者更高的版本，默认安装带有相应版本的pip)，并配置好Python 和 pip的环境变量。
2. 在工程目录下使用 pip install -r requirements.txt 命令安装依赖，如果安装失败，或者在安装及使用过程中提示缺少某个依赖项，则需要您使用 python -m pip install [xxx] 手动安装。
3. 如果您有可以使用的远程数据库MySQL，请先登录到远程数据库，并在数据库软件内新建一个普通用户，并赋予相应的权限（如果您使用本软件默认的设置，则新建的用户名为 "user1"，密码为"hello"），之后您需要以该用户的身份创建一个名为"idac"的数据库。跳转至第6条。
4. 如果您没有可供使用的远程数据库软件，那么需要在您的计算机系统上安装MySQL数据库软件。安装指南->. 之后您需要做好相关的配置工作。
5. 请在您本机的数据库软件内新建一个普通用户，并赋予相应的权限（如果您使用本软件默认的设置，则新建的用户名为 "user1"，密码为"hello"），之后您需要以该用户的身份创建一个名为"idac"的数据库。
6. 在 src/server/opt_db.py中调用init_mysql() 函数初始化对应的数据表。
7. 设置仿真参数，运行仿真程序。
8. 启动服务器，在浏览器中查看。





