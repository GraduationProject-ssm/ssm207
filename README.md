# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# ssm207基于SSM的视频播放系统的设计与实现+vue

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1gn8XeNE2J?p=6)


# 第一章 绪论
## 1.1研究背景
当今时代是飞速发展的信息时代。在各行各业中离不开信息处理，这正是计算机被广泛应用于信息管理系统的环境。计算机的最大好处在于利用它能够进行信息管理。使用计算机进行信息控制，不仅提高了工作效率，而且大大的提高了其安全性。尤其对于复杂的信息管理，计算机能够充分发挥它的优越性。

随着人们物质生活的提高，人们也开始享受精神生活。人们主要通过看视频、听音乐、阅读等来减轻生活工作压力，近年来，视频占有比例越来越高。基于这个现状，我们急需一个高速、快捷、方便的视频播放系统，为用户提供充足视频和快捷的查询手段，能及时、准确地查找出自己喜欢的视频，同时系统还容纳了论坛、投稿以及商城等功能模块，满足了用户的不同功能需求，可以为用户提供更优质的服务。
## 1.2 设计原则
在开始开发项目之前，必须要先考虑项目的实用性、科学性，以及该项目是否能够真正让用户受益并尽可能的发挥项目的作用。因此，在开发前，通过以下几条原则对项目进行判断：

（1）可行性原则。项目需要保证经济可行性和技术可行性，这包括了项目在浏览端、服务端等方面上的经济和技术上是可以达成的。

（2）适应性原则。项目要保证可维护性和可扩展性，这是每个非短期项目都需要考虑的，并且不论是维护还是扩展，都必须要建立在适应用户的正常需求的基础上。

（3）安全性及保密性原则。要充分保证用户信息的安全性和保密性，不能因为开发上的疏忽，导致用户的信息泄露。

（4）系统工程原则。为了确保项目的整体性，在项目调查、项目分析、项目设计、项目开发的过程中，都需遵从项目工程的方法和步骤逐步进行。

（5）统一规划、分期实施、逐步完善原则。项目开发的过程中，要按照规划、分期实施，特别是要注意在项目开发过程中要有条理，从点到面，一步步完善，不要贪图进度，要循环渐进的对项目进行开发。
## 1.3 研究内容
根据视频播放系统编写的论文主要阐述了视频播放系统的开发过程中使用的技术，首先进行系统需求分析，进而进行系统设计，最后才是系统功能实现以及测试几个部分，在开始编写论文之前亲自到图书馆借阅Java书籍，MYSQL数据库书籍等编程书籍，然后针对开发的视频播放系统，去网上查找了很多别人做好的系统，根据他们的功能设计进行自己的系统的系统功能结构设计，出具需求报告，最后才是进行程序编码，系统完成后才能进行测试和最后的验收工作，程序开发流程大致如此。

这次编写的论文包含了6个部分的内容，具体内容如下：

第一部分绪论：文章主要从课题背景以及设计原则综合阐述了开发此系统的必要性。

第二部分相关技术：系统开发用到的各种技术都大致做出了简介

第三部分系统分析：从可行性分析和功能需求分析等角度综合研究了此次开发的系统

第四部分系统设计：功能模块设计和数据库设计这两部分内容都有专门的表格和图片表示

第五部分系统实现：进行系统主要功能模块的界面展示

第六部分系统测试：检验程序是否达到预期目标

1

1
# 第二章 相关技术介绍
## 2.1Java技术
Java是一种非常常用的编程语言，在全球编程语言排行版上总是前三。在方兴未艾的计算机技术发展历程中，Java的身影无处不在，并且拥有旺盛的生命力。Java的跨平台能力十分强大，只需一次编译，任何地方都可以运行[1]。除此之外，它还拥有简单的语法和实用的类库，让编程人员可以尽可能将精力集中在问题的求解上，并且许多开源项目和科研成果都是采用它实现的。

在1995年这一年的5月份，著名的Sun Microsystems公司在程序开发设计上面郑重推出一种面向对象开发的程序设计语言——Java，最开始的时候Java是由詹姆斯.高斯林这位伟大的JAVA之父来进行主导，但是在后来由于各种原因，让甲骨文公司这个针对商业程序创建了oracle大型数据库的公司收购了Java。Java的平台总共算下来有3个，分别为javaME和javaSE以及javaEE这3个java平台。下面将对其进行分别介绍。

（1）在电脑桌面程序的开发上面需要选择JavaME，这个用得也比较多。

（2）企业也会根据工作以及业务需要开发各种软件，那么就会选用JavcEE这个支持企业版软件的开发的Java平台，JavcEE主攻运用在企业领域上面的web应用，JavcEE也在javaSE的基础上获得了比如jsp技术 ，Servlet技术等程序开发技术的支持。

（3）现在生活中手机的普及化，也使得手机端这样的移动设备的软件的兴起，JavaME这个迷你版java平台就能运用于移动端的软件开发操作。
## 2.2MYSQL数据库
MySQL是典型的关系数据库系统，拥有开源免费、稳定、高效等特点，一直是中小型web项目的最佳数据库选择。MySQL作为当今IT领域使用人数最多的开源关系型数据库软件之一，在2018年的数据库使用率排名中位居第二，仅次于目前为止最成功的商业版数据库Orcle[13]。MySQL最大的优势之一就是无偿使用，这也是它成功的关键。

MySQL支持标准化数据库查询语言SQL。MySQL是一款非常适合个人开发者或小型组织开发团体的数据库管理系统，因为它是开源并且免费的，体积小、速度快、成本低以及其最重要的一点开放源码，深受程序设计人员的喜爱，这也让它成为了许许多多中小型开发网站数据库的首选，同时提供了多种开发的连接API。MySQL将数据的存放按照记录之间的关系存放到了不同的表中，减少了数据的冗余并且提高了开发的工作效率。MySQL支持开发中需要用的大型数据库，并能处理数以万计的记录。因为MySQL是开源的软件，所以在项目的预算中的时候不用花费额外的资金，大大降低了开发的总体成本，这也是MySQL数据库在中小型企业和独立的开发者中广泛流行的原因[5]。
## 2.3 B/S结构 
在早期的程序开发中，使用得最多的莫过于C/S架构了，现在的生活中软件在生活的各个方面落地，使用了C/S架构开发出来的软件也是不在少数的，比如企业日常办公使用到的微软的OFFICE软件，我国自己研发的文档处理软件WPS，还有娱乐软件腾讯的QQ，腾讯的微信，以及电脑上安装的杀毒软件金山杀毒软件，瑞金杀毒软件等都是C/S架构。但是在Internet网络盛行之后，鉴于大家对数据信息共享的需求，在原来的C/S架构上进行了升级改进之后，有了现在的主流架构B/S架构，B/S架构就是在C/S架构上多了一个浏览器，让原来的直接访问服务器的方式，变成了通过浏览器去访问服务器。充分运用到了当下不断成熟的浏览器技术。也让软件的开发成本以及维护成本降低了。可以说B/S这种新型的架构模式让软件的开发变得便利化。
## 2.4 SSM框架
本视频播放系统基于Spring、SpringMVC、Mybatis框架进行开发设计。

Spring 框架是在2004年首次发布，之后出现了多次的重大修订。Spring框架是由七个不同的模块组成，分别是SpringCore、Spring AOP、Spring ORM、Spring DAO、Spring Web Flow、Spring Context和Spring Web MVC[16]。这些模块提供不同的平台来开发不同的企业应用程序 ，本课题使用Spring Web MVC模块开发基于MVC的应用程序。

Spring Web MVC是基于Servlet API的原始Web框架，从一开始就包含在Spring 框架中。“Spring Web MVC”是该框架的正式名称，但通常被简称为“Spring MVC” [17]。Spring MVC框架提供了模型模块-视图模块-控制器的架构和可用于直接开发的Web应用程序的现成组件。Spring MVC模式将应用程序的不同方面分开，使元素之间形成松散耦合。

MyBatis原名叫做iBatis属于持久层框架，消除了大部分JDBC代码和参数的设置以及结果集的检索。这个框架不仅支持普通SQL查询和存储过程，还支持高级的映射[18]。MyBatis使用.xml和注解来做原始映射和配置，将接口和Java对象映射成数据库记录。


# 第三章 系统分析
## 3.1 可行性分析
需要使用大部分精力开发的基于SSM的视频播放系统为了充分降低开发风险，特意在开发之前进行可行性分析这个验证系统开发是否可行的步骤。本文就会从技术角度，经济角度，还有操作角度等进行综合阐述。
### 3.1.1技术可行性
本文将开发的系统，将采用的关键技术包括JAVA编程语言、SSM框架、MYSQL数据库存储技术等。另外，程序开发需要在自己电脑上安装的软件并不多，在win7操作系统的大环境下，能够完全搭建好程序开发的操作环境，比如Myeclipse工具，MYSQL数据库工具，以及处理程序图片的Photoshop工具等都能安装在自己的电脑上。总的说来，开发这个程序在技术上是可以实现的，该项目的开发是有保障的。
### 3.1.2经济可行性
开发这个程序软件并不会涉及到经济上面的开销，在开发软件的选择上也不会额外付费安装软件，在开发软件的官网上面就可以下载需要的软件，并根据提示的安装步骤安装软件到自己的电脑上面。因此，该项目的实施在经济上完全可行。
### 3.1.3操作可行性
操作可行性主要是针对系统用户而言，一个系统再完美，技术再先进，用户不去使用，或者用户根本不会使用，该系统存在的价值也是不大的。本系统拟采用的是B/S架构，用户只要通过点击浏览器即可轻松访问，而用户对浏览器操作非常熟练，所以从用户的角度而言，没有任何学习成本，因此，操作上是可行性的。
### 3.1.4时间可行性
从时间上看，在三个月的时间里学习相关知识，开发本基于SSM的视频播放系统，时间上是有点紧，但是不是不可能实现，在做毕业设计的这几个月里，我通过努力使得功能应该基本可以实现。

从上面几个部分的可行性分析得出，这次开发的基于SSM的视频播放系统在开发上面没有什么大问题，值得开发。
## 3.2系统性能分析
### 3.2.1 系统安全性
程序在使用中是不允许其他访问者随意窃取程序里面的隐秘信息，也不允许其他操作者越权操作其他管理用户操作的功能，要真正杜绝这些现象就必须在程序开发之前把程序的安全性给考虑进去。

比如现在很多程序都会把用户注册的功能给考虑进去，让用户在注册页面功能区填写自己的个人信息，这些数据信息涵盖了用户本人的姓名，用户对程序登录设置的密码，用户经常使用的邮箱，用户的常用联系方式还有用户的所住地址等信息，这些信息都是设计到用户本人的隐私，那么这些信息在传输给程序后台时，是需要进行管理并保存至对应的数据库文件里面。要是有人恶意窃取程序的数据信息，也就会让那些注册了此程序软件的用户的个人隐秘信息都会遭到泄露。这些信息落入其他不法分子手里，他们极有可能根据用户的隐私信息去骚扰用户，并把这些信息用于各种商业用途谋取其他非法的利益。所以数据安全性是一个系统能不能使用的首要标准。
### 3.2.2 数据完整性
数据完整性是确保数据信息是否具有可靠性，是否具有参考价值的一个重要因素，数据信息只描述一部分，或者必有的数据信息反而为空等现象都是代表着这个数据信息不完整，有数据缺陷，这是个很严肃的问题，因为这样的数据信息跟垃圾信息没什么两样。

说到数据完整性，不得不提最常用的程序表单功能。这些表单主要就是提取广大用户的数据信息的，需要广大用户根据表单上的要求，填写自己的姓名信息，以及自己的联系方式信息，有些也会有额外的信息填写要求，有必须要填的选项，也有不需要必填的选项。假如广大用户为了保护自己的隐私，或者不想受到其他人的骚扰，不填写必填项等信息，广大用户在最后提交此表单的时候，往往都是提交不了的。

由于数据表之间也会存在一定的联系，所以同一个数据也会出现在另一个表格里面，那么这两个表格记录的同一个数据应该是一样的。不能够是同样的数据信息在不同表中不一样。
### 3.2.3系统可扩展性
一切事物都是一直在发展，程序员开发软件也需要带着发展的思维去进行软件开发操作，这样的话，开发出来的程序在应对管理所需时，也会相对应的进行程序升级与更新。不论是功能完善还是数据库升级都能在原来的基础上对原有程序进行迭代升级。让开发出来的程序能够走得越来越远。这也是广大用户对程序软件的使用要求。
## 3.3系统流程分析
### 3.3.1注册流程
未有账号的用户可进行注册操作，用户注册流程图如图3.1所示。

![](/md/blog.001.png)

图3.1注册流程图
### 3.3.2登录流程
登录模块主要满足了管理员和用户的权限登录，用户登录流程图如图3.2所示。

![](/md/blog.002.png)

图3.2 登录流程图
### 3.4.3论坛发帖流程
用户论坛发帖前提必须是登录后才能进行，发帖内容不能为空，且合法才能进行提交发表成功。详见图3.3所示。

![](/md/blog.003.png)

图3.3  论坛发帖流程图
## 3.4系统功能分析
本基于SSM的视频播放系统主要分管理员和用户两大功能模块，下面将详细介绍管理员和用户分别实现的功能。
### 3.4.1用户功能分析
用户在系统前台可查看系统信息，包括首页、视频、投稿、商城以及资讯等，用户要想实现留言反馈、论坛发帖等操作，必须登录系统，没有账号的用户可进行注册操作，注册登录后主要功能模块包括个人中心、我的发布、我的订单、我的地址以及我的收藏。用户用例图如图3.4所示。

![](/md/blog.004.png)

图3.4 用户用例图
### 3.4.2管理员功能分析
管理员可登录系统后台对系统进行全面管理操作，管理员主要功能模块包括个人中心、用户管理、视频管理、投稿管理、分类栏管理、商城管理、商品类型管理、留言板管理、论坛、系统管理以及订单管理。 管理员用例图如图3.5所示。

![](/md/blog.005.png)

图3.5 管理员用例图

# 第四章 系统设计
## 4.1系统概要设计
本视频播放系统采用B/S结构来开发，这种结构是在互联网兴起后出现的，是一个适用于互联网环境下的模型结构，用户只要能上网通过浏览器就可以在任何时间、任何地点的使用。系统工作原理图如图4-1所示：

![](/md/blog.006.png)

图4.1 系统工作原理图
## 4.2 系统结构设计
系统整体设计是一个将一个庞大的任务细分为多个小的任务的过程，这些小的任务分段完成后，组合在一起形成一个完整的任务。本基于SSM的视频播放系统主要包括用户功能模块和管理员功能模块，系统功能模块图如图4.2所示。

![](/md/blog.007.png)

图4.2 系统功能模块图
## 4.3 数据库设计
### 4.3.1数据库E-R图设计
E-R图是一种描述显示数据类型间的关系的数据描述方法，E-R图可以完整地映射出现实模型的关系。E-R图中的三个最为重要的元素就是实体、属性、关系。本基于SSM的视频播放系统的E-R图如下所示：

（1）论坛信息实体E-R图如图4.3所示：

![](/md/blog.008.png)

图4.3 论坛信息实体属性图

（2）管理员信息实体E-R图如图4.4所示：

![](/md/blog.009.png)

图4.4  管理员信息实体属性图

（3）订单信息实体E-R图如图4.5所示：

![](/md/blog.010.png)

图4.5 订单信息实体属性图

（4）商城信息实体E-R图如图4.6所示：

![](/md/blog.011.png)

图4.6 商城信息实体属性图

（5）用户信息实体E-R图如图4.7所示：

![](/md/blog.012.png)

图4.7用户信息实体属性图

（6）视频信息实体E-R图如图4.8所示：

![](/md/blog.013.png)

图4.8 视频信息实体属性图
### 4.3.2数据库表设计
基于SSM的视频播放系统采用MYSQL数据库作为数据存储，下面介绍数据库中的各个表的详细信息。

表4.1 forum论坛信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|title|varchar|200|是|帖子标题|
|content|longtext||是|帖子内容|
|parentid|bigint|20|是|父节点编号|
|userid|bigint|20|是|用户编号|
|username|varchar|200|是|用户名|
|isdone|varchar|200|是|状态|

表 4.2  users管理员信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|username|varchar|100|是|用户名|
|password|varchar|100|是|密码|
|role|varchar|100|是|角色|
|addtime|timestamp||是|新增时间|

表 4.3  orders订单信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|下单时间|
|orderid|varchar|200|是|订单编号|
|tablename|varchar|200|是|商品表名|
|userid|bigint|20|是|用户编号|
|goodid|bigint|20|是|商品编号|
|goodname|varchar|200|是|商品名称|
|picture|varchar|200|是|商品图片|
|buynumber|int|11|是|购买数量|
|price|float||是|价格|
|discountprice|float||是|折扣价格|
|total|float||是|总价格|
|discounttotal|float||是|折扣总价格|
|type|int|11|是|支付类型|
|status|varchar|200|是|状态|
|address|varchar|200|是|地址|
|tel`|varchar|200|是|电话|
|consignee|varchar|200|是|收货人|

表4.4  shangcheng商城信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|shangpinmingcheng|varchar|200|是|商品名称|
|shangpinfenlei|longtext||是|商品分类|
|fahuodi|bigint|20|是|发货地|
|xiaoliang|bigint|20|是|销量|
|canshu`|varchar|200|是|参数|
|xiangqing|varchar|200|是|详情|
|tupian|varchar|200|是|图片|
|thumbsupnum|int|11|是|赞数|
|crazilynum|int|11|是|踩数|
|clicktime`|datetime||是|最近点击时间|
|clicknum|int|11|是|点击次数|
|price|float||是|价格|

表4.5  yonghu用户信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|zhanghao|varchar|200|是|账号|
|mima|varchar|200|是|密码|
|xingming`|varchar|200|是|姓名|
|shenfenzheng|varchar|200|是|身份证|
|nianling`|int|11|是|年龄|
|xingbie|varchar|200|是|性别|
|`shouji`|varchar|200|是|手机|
|youxiang|varchar|200|是|邮箱|
|touxiang|varchar|200|是|头像|
|money|float||是|余额|

表4.6  shipin视频信息表

|列名|数据类型|长度|允许空|说明|
| - | - | - | - | - |
|id|bigint|20|否|编号|
|addtime|timestamp||是|创建时间|
|shipinmingcheng|varchar|200|是|视频名称|
|fabushijian|datetime||是|发布时间|
|fenlei|varchar|200|是|分类|
|shipin|varchar|200|是|视频|
|jianjie|varchar|200|是|简介|
|fengmian|varchar|200|是|封面|
|zhanghao|varchar|200|是|账号|
|xingming|varchar|200|是|姓名|
|thumbsupnum|int|11|是|赞数|
|crazilynum|int|11|是|踩数|
|clicktime`|datetime||是|最近点击时间|
|clicknum|int|11|是|点击次数|
# 第五章 系统的实现
## 5.1 用户功能模块的实现
### 5.1.1系统主界面
用户进入本系统可查看系统信息，系统主界面展示如图5.1所示。

![](/md/blog.014.png)

图5.1网站主界面
### 5.1.2视频详情界面
用户可选择视频查看视频详情信息，并可进行视频播放操作，视频详情界面展示如图5.2所示。

![](/md/blog.015.png)

图5.2视频详情界面
### 5.1.3用户注册界面
未有账号的用户可进入注册界面进行注册操作，用户注册界面展示如图5.3所示。

![](/md/blog.016.png)

图5.3用户注册界面
### 5.1.4用户登录界面
用户在登录界面可输入正确的登录信息，点击提交按钮进行登录操作，用户登录界面展示如图5.4所示。

![](/md/blog.017.png)

图5.4用户登录界面
### 5.1.5投稿界面
用户登录后可进行投稿操作，投稿界面展示如图5.5所示。

![](/md/blog.018.png)

图5.5投稿界面
### 5.1.6商品详情界面
用户可选择商品查看详情，登录后可进行加入购物车或者购买操作，商品详情界面展示如图5.6所示。

![](/md/blog.019.png)

图5.6 商品详情界面
## 5.2 管理员功能模块的实现
### 5.2.1管理员登录界面
管理员要想进入系统后台对系统进行管理操作，必须登录系统后台，管理员登录界面展示如图5.7所示。

![](/md/blog.020.png)

图5.7  用户管理界面
### 5.2.2用户管理界面
管理员可查看新增、修改和删除用户信息，用户管理界面展示如图5.8所示。

![](/md/blog.021.png)

图5.8  用户管理界面
### 5.2.3视频管理界面
管理员可增删改查视频信息，视频管理界面展示如图5.9所示。

![](/md/blog.022.png)

图5.9  视频管理界面
### 5.2.4商城管理界面
管理员可添加、修改和删除商城商品信息，商城管理界面展示如图5.10所示。

![](/md/blog.023.png)

图5.10 商城管理界面
### 5.2.5投稿管理界面
管理员可查看用户投稿信息，并可对其进行审核、修改和删除操作，投稿管理界面展示如图5.11所示。

![](/md/blog.024.png)

图5.11 投稿管理界面
### 5.2.6论坛管理界面
管理员可查看所有论坛帖子信息，并可对其进行管理，论坛管理界面展示如图5.12所示。

![](/md/blog.025.png)

图5.12 论坛管理界面
### 5.2.7订单管理界面
管理员可管理所有订单信息，订单管理界面展示如图5.13所示。

![](/md/blog.026.png)

图5.13 订单管理界面

# 










