# flask-ansible

#### 介绍
Flask实现Ansible和Ansible-Playbook的配置+部署系统。同时带有简单的服务器管理系统和认证系统。

#### 软件架构
本项目使用的Python为Python3.6版本，数据库使用Mysql，后端使用Flask，前端框架使用Bootstrap实现。依赖的库较少，数据库未使用框架。


#### 安装教程

1. 创建数据库

```
  create database devops;  
  grant all privileges on *.* to 'shijiange'@'127.0.0.1' identified by 'shijiangepwd';  
  flush privileges;
```

2. 导入数据

```
  set names utf8;  
  source Flask-Ansible.sql;
```

3. Python3依赖安装
```  
  pip3 install -r requirements.txt
```
4. 运行Flask项目
```  
  python3 app.py
```

#### 使用说明

1. 认证系统
![需要登录](https://images.gitee.com/uploads/images/2019/0710/111040_c8e2f6e3_129867.png "认证.png")
登录界面没优化，比较丑，默认用户名密码shijiange/shijiangepwd，可自行添加用户
```
insert into user (username,password) values ('xxx', md5('xxxx'));
```
2. 服务器管理系统
![服务器管理系统](https://images.gitee.com/uploads/images/2019/0710/111256_364aa699_129867.png "服务器管理.png")

3. Ansible和Playbook配置+部署系统
![Ansible配置管理](https://images.gitee.com/uploads/images/2019/0710/111415_7c10e8ad_129867.png "Ansible配置管理.png")
![Ansible执行说明](https://images.gitee.com/uploads/images/2019/0710/111449_c7e23e77_129867.png "Ansible执行说明.png")


#### 如何实现的在线教程地址
  https://item.taobao.com/item.htm?spm=a1z10.1-c.w4004-16405581643.28.6c3a3fcfbof39R&id=597766904277

#### 参与贡献

1. Fork 本仓库
2. 新建 Feat_xxx 分支
3. 提交代码
4. 新建 Pull Request


#### 码云特技

1. 使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2. 码云官方博客 [blog.gitee.com](https://blog.gitee.com)
3. 你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解码云上的优秀开源项目
4. [GVP](https://gitee.com/gvp) 全称是码云最有价值开源项目，是码云综合评定出的优秀开源项目
5. 码云官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6. 码云封面人物是一档用来展示码云会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)