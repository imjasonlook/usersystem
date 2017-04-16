﻿## 用户管理系统

根据提供文档做了用户管理系统功能如下：

*  注册
*  登陆(记住密码 设置为记录七天)
*  聊天支持群聊,单聊

## 相关技术:

*  php框架-thinkPHP3.2.3
*  前端模板-layui
*  数据库-mysql
*  前端H5的websocket通信
*  后端php-workerman socket模块

## 流程
*  注册-用户填入手机号,姓名,密码等相关信息注册
*  登陆-用户根据手机号登陆,可选择记住密码,将用户信息加密存入cookie,密码可维持七天
*  首页-首页用户列表,可对用户进行修改,删除,操作
*  用户修改-可修改姓名,手机号
*  用户删除-利用ajax无刷新删除
*  im聊天-右下角展开聊天面板,显示所有用户,默认存在一个群组,均可聊天

## 安装与使用
*  现在nginx/apache搭建网站
*  将sql文件导入mysql 数据库为usersystem选择utf8编码
*  安装php event模块
*  运行workerman(此版本需要在linux/macos系统下运行)
*  php start.php start -d 以守护方法形式运行wokerman
*  测试聊天需要两个不同浏览器进行对话