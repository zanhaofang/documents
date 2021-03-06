﻿# **iSee电影在线购票网站**
# **软件需求说明书（SRS）**



### 中山大学数据科学与计算机学院
### iSee小组
















### **1 引言**
#### **1.1 编写目的**
&#8195;&#8195;为项目开发做准备的前提条件，为明确软件基本功能和性能及概要设计说明书的编写提供依据，为系统开发后的测试和评审做参考，同时也是客户的要求。

#### **1.2 背景**
&#8195;&#8195;本项目为iSee小组自主实现的能够实现在线购票功能的网站，旨在帮助人们更便捷的从网络上购买电影票。


项目名称：iSee电影在线购票网站

项目组织者： iSee小组

项目主负责人：徐广晖

项目组成员： 徐广晖，吴其锋，方赞浩

产品用户者： 所有在线用户

产品设计者： iSee小组

产品所有权： iSee小组拥有

#### **1.3 定义**
&#8195;&#8195;该电影购票网站是基于Internet及Web技术，建立以Browser/Server 为结构模式、以数据库为后台核心应用、以服务为目的销售平台，对上映电影的信息进行总和，实现在线售票功能的网站。
开发平台：Node 7.6.0+

### **2 人物概述**
#### **2.1 目标**
&#8195;&#8195;iSee电影在线购票网站是一个集挑选电影、挑选场次、挑选座位、在线预订及支付等功能的网站，旨在为用户提供一个更加便捷的电影购票网站，让人们在忙碌之余可以抽空去电影院看电影而省去买实体电影票的麻烦。

#### **2.2 用户的特点**
&#8195;&#8195;本网站的用户面向所有人群。

#### **2.3 假定和约束**
&#8195;&#8195;针对开发者的约束有：

&#8195;&#8195;a.所需要的高级程序语言

&#8195;&#8195;b.硬件限制

&#8195;&#8195;c.开发期限

&#8195;&#8195;d.运行环境

### **3 具体要求**
#### **3.1 功能需求**
#### 3.1.1 网站各功能下的画面

&#8195;&#8195;打开网站时的画面：

![](https://github.com/iSee-SYSU/documents/blob/master/img/init1.png)

![](https://github.com/iSee-SYSU/documents/blob/master/img/init2.png)

![](https://github.com/iSee-SYSU/documents/blob/master/img/init3.png)

![](https://github.com/iSee-SYSU/documents/blob/master/img/init4.png)

&#8195;&#8195;点击购票时的画面：

![](https://github.com/iSee-SYSU/documents/blob/master/img/buy.png)

&#8195;&#8195;点击查看影院时的画面：

![](https://github.com/iSee-SYSU/documents/blob/master/img/cinema.png)

#### 3.1.1 功能模块
a、网站各个界面的加载和切换

&#8195;&#8195;网站主要分为四个界面：主界面，即进入网站看到的界面，显示的是位置以及上映电影的信息，用户可以选择切换位置来切换影院，可以选择自己喜欢的电影进入影院选择界面；影院选择界面，用户点击电影购票之后进入的界面，可以看到该区域正在上映该电影的影院列表以及影院的基本信息及电影的最低价格，用户可以点击相应的影院进入购票界面；购票界面，用户点击了影院之后进入的界面，显示的是电影的上映信息以及影院的详细位置信息及简介。

b、用户的点击选择

&#8195;&#8195;在主界面用户可以点击位置选择来选择自己的区域，选择电影之后点击购票按钮会进入相应的影院选择界面，选择完影院之后点击影院可以进入对应的购票界面。

c、用户的状态判断

&#8195;&#8195;网站没有实现登录注册功能，用户进入网站即为登录状态，退出网站即为退出状态。

#### 3.1.3 UML结构图
&#8195;&#8195;用例1：用户登录

![](https://github.com/iSee-SYSU/documents/blob/master/img/case1.png)

A.描述：用户进入网站即为登录

B.参与者：进入网站的用户

&#8195;&#8195;用例2：退出网站

![](https://github.com/iSee-SYSU/documents/blob/master/img/case2.png)

A.描述：用户退出网站

B.参与者：已经进入网站的用户

&#8195;&#8195;用例3：选择区域

![](https://github.com/iSee-SYSU/documents/blob/master/img/case3.png)

A.描述：用户进行位置区域选择

B.参与者：进入网站的用户

&#8195;&#8195;用例4：选择电影

![](https://github.com/iSee-SYSU/documents/blob/master/img/case4.png)

A.描述：用户选择喜欢的电影

B.参与者：进入网站的用户

&#8195;&#8195;用例5：影院选择

![](https://github.com/iSee-SYSU/documents/blob/master/img/case5.png)

A.描述：用户选择想看电影的影院

B.参与者：进入网站的用户

&#8195;&#8195;用例6：系统管理用例图

![](https://github.com/iSee-SYSU/documents/blob/master/img/case6.png)

#### **3.2 性能需求**
#### 3.2.1 时间特性相应
&#8195;&#8195;响应时间不大于0.05s。 

#### 3.2.2 灵活性
&#8195;&#8195;说明对该软件的灵活性的要求，即当需求发生某些变化时，该软件对这些变化的适应能力，如：

&#8195;&#8195;a．操作方式上的变化；

&#8195;&#8195;b．运行环境的变化；

&#8195;&#8195;c．同其他软件的接口的变化；

&#8195;&#8195;d．精度和有效时限的变化；

&#8195;&#8195;e．计划的变化或改进。

&#8195;&#8195;对于为了提供这些灵活性而进行的专门设计的部分应该加以标明。

#### 3.2.3 故障处理要求
&#8195;&#8195;列出可能的软件、硬件故障以及对各项性能而言所产生的后果和对故障处理的要求。

##### 3.2.4 其他专门要求
&#8195;&#8195;如用户单位对安全保密的要求，对使用方便的要求，对可维护性、可补充性、易读性、可靠性、运行环境可转换性的特殊要求等。

### **4 运行环境要求**
#### **4.1 设备**
&#8195;&#8195;所有拥有web浏览器的设备。

#### **4.2 支持软件**
&#8195;&#8195;现代浏览器和 IE9 及以上（需要 polyfills）。

