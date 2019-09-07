# 平台演示
该平台目前是一个基于django框架开发的轻量级平台，现已完成模块：登陆、权限控制（包括组织架构管理、用户管理、菜单管理、角色管理、个人信息设置）、系统日志管理，主页，其目的在于建立一套规范化、统一化和清晰化的标准业务支撑承载平台。
系统支持多数据库，能够清晰的处理、记录和追踪平台操作流程。
目前已完成平台级功能，后续将持续提供业务场景化功能。
由于云主机到期，暂不能提供公网访问地址。
后续的技术扩展：
1. 前端界面后续可React方式展示；
2. 可使用分布式任务队列管理工具（如celery，中间人采用redis）来处理比较耗时的操作，如发送邮件，计划任务等;
3. 用mongodb来存储日志信息；

# 功能介绍
## 1. 平台支撑功能
### 1.1 系统登陆
![image](https://github.com/hapjackye/platformshow/blob/master/Image/001.png)<br>
### 1.2 权限管理功能介绍
系统权限是采用基于角色组的权限配置，根据用户角色组权限动态生成导航菜单，基于角色组的权限管理，权限分明，各司其职<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/002.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/003.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/004.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/005.png)<br>~~~~
![image](https://github.com/hapjackye/platformshow/blob/master/Image/006.png)<br>
### 1.3 系统日志功能介绍
用于记录系统用户进入系统后的操作过程，采用服务端分页方式提高响应速度，并配有单独的数据库以便后续进行扩展<br>
图1：基于用户的操作痕迹<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/007.png)<br>
## 2. 业务功能(持续更新中)
### 2.1 主页
本来想弄个框架就好，但实在看不下去，简单的修饰了一番（鄙人前端不强，又非美工出身，觉得丑的请勿喷^_^），做了些简单的数据图形呈现，算是抛砖引玉吧，后续可以根据实际业务场景使用现代金属风格来美化，图形插件用的是echarts，尚有些bug,后续再寻觅更好的插件，地图可以换成第三方的，比如百度。
![image](https://github.com/hapjackye/platformshow/blob/master/Image/008.png)<br>
### 2.2 资源管理
资源管理的概念相当大，主要负责所有资源的管理，这里简单的列举一些对象来做演示，内含资源的录入、跟踪、管理以及CMDB的使用。
#### 2.2.1 销售管理
管理资产设备购进过程中涉及的分销商信息<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/010.png)<br>
#### 2.2.2 客户管理
目标用户信息管理
![image](https://github.com/hapjackye/platformshow/blob/master/Image/011.png)<br>
#### 2.2.3 资产类型管理
基于CMDB方式的CI项管理，根据项目需要自定义资产类型
![image](https://github.com/hapjackye/platformshow/blob/master/Image/012.png)<br>
#### 2.2.4 设备类型管理
基于CMDB方式的CI项管理，根据项目需要自定义设备类型
![image](https://github.com/hapjackye/platformshow/blob/master/Image/013.png)<br>
#### 2.2.5 资产管理
对于项目所需的资产进行录入，资产录入后自动与相关CI项信息进行绑定，绑定后能自动生成资产变更记录可作为台账信息进行处理
![image](https://github.com/hapjackye/platformshow/blob/master/Image/014.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/015.png)<br>
#### 2.2.6 设备管理
对于企业所使用的各种设备进行登记和管理，包括了设备购进信息及使用负责单位，并对于设备的维护进行实时记录，可作为台账信息进行处理
![image](https://github.com/hapjackye/platformshow/blob/master/Image/016.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/017.png)<br>
![image](https://github.com/hapjackye/platformshow/blob/master/Image/018.png)<br>

### 2.3 工单管理（待续）
