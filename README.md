# 1引言

## 1.1编写目的

为了便于项目开发人员能够清楚了解项目整体框架，指导后续项目开发，特编写此开发指导。

## 1.2背景

v  系统名称：图书馆管理系统

v  任务提出者：凤姐

v  项目开发者：凤姐

v  用户：图书馆管理人员

 

## 1.3开发环境和工具

v     操作系统: win8/win10 

v     内存: 4G 以上

v     JDK: 8.0

v     开发工具: Intellij IDEA2020.1 旗舰版

v     服务器:  Tomcat8.0

v     数据库工具:mysql5.5 +Navicat Premium 12  

## 1.4 项目技术

基于B/S结构  

前端: HTML+CSS+JS +JQuery  

后端: Servlet+JSP+MySql   

![web服务器2](D:\桌面2\README (2).assets/clip_image002.jpg)      

## 1.5定义

JSP: JavaServer Pages是由Sun Microsystems公司倡导、许多公司参与一起建立的一种动态网页技术标准。

Apache: Apache是世界使用排名第一的Web服务器软件。

Ajax：Asynchronous Javascript And XML（异步JavaScript和XML），是指一种创建交互式网页应用的网页开发技术。通过在后台与服务器进行少量数据交换，AJAX 可以使网页实现异步更新。

C3P0:数据库连接池

OSI：Open System Interconnect 开放系统互连参考模型。

MVC：Model View Controller ，是模型(model)－视图(view)－控制器(controller)的缩写，一种软件设计典范，用一种业务逻辑、数据、界面显示分离的方法组织代码。

DBUtils：Commons DbUtils是[Apache](https://baike.baidu.com/item/Apache/8512995)组织提供的一个对[JDBC](https://baike.baidu.com/item/JDBC)进行简单封装的开源工具类库，使用它能够简化[JDBC](https://baike.baidu.com/item/JDBC)应用程序的开发，同时也不会影响程序的性能。

# 2  开发过程

### 2.1 功能模块 

​    

| 功能模块    | 功能点       | 优先级 |
| ----------- | ------------ | ------ |
| 1：用户管理 | 1-1 用户登录 | *****  |
|             | 1-2 安全退出 | ****   |
|             | 1-3 修改密码 | ****   |
| 2:会员管理  | 2-1 会员开卡 | *****  |
|             | 2-2 注销会员 | ****   |
|             | 2-3 查看会员 | *****  |
|             | 2-4 修改会员 | ****   |

 

| 3: 图书管理 | 3-1 添加图书 | ***** |
| ----------- | ------------ | ----- |
|             | 3-2 查看图书 | ***** |
|             | 3-3 修改图书 | ****  |
|             | 3-4 删除图书 | ****  |

 

| 4: 常用功能 | 4-1 图书借阅         | ***** |
| ----------- | -------------------- | ----- |
|             | 4-2 归还图书         | ***** |
|             | 4-3 历史借阅信息查询 | ****  |

 

## 2.2 重要功能点流程图

**用户登录流程图**

![img](D:\桌面2\README (2).assets/clip_image004.jpg)

**借阅图书流程图**

![img](D:\桌面2\README (2).assets/clip_image006.jpg)

**归还图书流程图**

![img](D:\桌面2\README (2).assets/clip_image008.jpg)

 

## 2.3 E-R图

![img](D:\桌面2\README (2).assets/clip_image010.jpg)

## 2.4 开发流程

### 2.4.1 准备环境

v  安装jdk8.0 和 idea：安装文件和安装配置方式请参考前面视频

v  安装mysql 和navicat: 安装文件和安装配置方式请参考前面视频

v  安装tomcat 和 配置: 安装文件和安装配置方式请参考前面视频

v  创建web项目配置tomcat: 从这里开始

v  创建数据库bookdb

v  添加配置文件

v  添加包

v  测试数据库连接类

v  在webContent中添加前端资源

v  启动项目，访问前端资源