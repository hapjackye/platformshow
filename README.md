# 平台演示
该平台目前是一个基于django框架开发的轻量级平台，现已完成模块：登陆、权限控制（包括组织架构管理、用户管理、菜单管理、角色管理、个人信息设置）、系统日志管理，其目的在于建立一套规范化、统一化和清晰化的标准业务支撑承载平台。
系统支持多数据库，能够清晰的处理、记录和追踪平台操作流程。
目前已完成平台级功能，后续将持续提供业务场景化功能。
后续的技术扩展：
1. 可使用分布式任务队列管理工具（如celery，中间人采用redis）来处理比较耗时的操作，如发送邮件，计划任务等;
2. 用mongodb来存储日志信息；

# 1 功能介绍
## 1.1 系统登陆
![image](https://github.com/hapjackye/platformshow/blob/master/Image/001.png)<br>
## 1.1 权限管理功能介绍
系统权限是采用基于角色组的权限配置，根据用户角色组权限动态生成导航菜单，基于角色组的权限管理，权限分明，各司其职<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/002.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/003.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/004.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/005.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/006.png)<br>
## 1.2 系统日志功能介绍
用于记录系统用户进入系统后的操作过程，采用服务端分页方式提高响应速度，并配有单独的数据库以便后续进行扩展<br>
图1：基于用户的操作痕迹<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/007.png)<br>
## 2.1 业务功能(待续)