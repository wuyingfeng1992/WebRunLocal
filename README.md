﻿# WebRunLocal
   PluginOK(牛插)中间件(原名:本网通WebRunLocal)是一个实现网页浏览器(Web Browser)与本地程序(Local Application)之间进行双向调用的低成本、强兼容、安全可控、轻量级、易集成、可扩展、跨浏览器的小程序系统，是浏览器功能扩展的最佳利器。通过本中间件可实现网页前端JS脚本无障碍操控本地电脑的各种硬件、调用本地系统API及相关组件功能，彻底解决DLL、ActiveX控件及自动化程序(如MSOffice、金山WPS、AutoCAD等)在Chrome、Edge(Chromium内核)、360极速/安全/企业、FireFox、IE、Opera、QQ、搜狗等浏览器各版本中的完美嵌入运行问题，媲美Java Applet的运行效果，并且提供的开发接口与前端语言无关，前端只需使用JS+JSON+Web Socket相关技术即可实现与B/S系统完美对接。

PluginOK(牛插)中间件及相关小程序由成都佐罗软件有限公司研发并销售，咨询热线电话：18081958957、15201358223、18051018685，公司网站：http://www.zorrosoft.com 商务邮箱：wzh@zorrosoft.com 微信在线沟通：ZorroSoft、qq972340118 咨询报价请优先通过微信和商务邮箱进行，谢谢！

系统兼容性：
1、全面兼容Windows XP、Vista、7、8.1、10等各版本32及64位桌面系统；
2、全面兼容Windows Server 2008、2012、2016、2019等各版本32及64位服务系统。

浏览器兼容性：
1、IE 8及以上版本；
2、Chrome 41及以上版本；
3、FireFox 52及以上版本；
4、Opera 36及以上版本；
5、Edge(Chrome内核) 80及以上版本；
6、360极速浏览器 9.5及以上版本；
7、360安全及企业安全浏览器；
8、QQ浏览器10及以上版本；
9、搜狗浏览器；
......

   在IE中实现网页和本地系统双向调用的方法是使用ActiveX控件技术，而在Chrome、FireFox等浏览器有类似的NPAPI插件技术。因为安全隐患及稳定性等问题，微软Chrome内核浏览器Edge不再支持ActiveX控件，而目前市场占有率高达70%的Chrome浏览器也从45版开始NPAPI插件技术也被抛弃，导致原来很多依赖这些技术实现的业务无法在新版浏览器中继续使用。

目前浏览器网页与本地程序之间双向调用的知名解决方案有以下两个：
1、FireBreath，底层实现采用的是ActiveX和NPAPI技术，已面临2015年后发布的浏览器版本不能兼容使用的问题；
2、Node.js，是一个基于Chrome V8引擎的 JavaScript 运行环境，其中FFI模块可实现在JavaScript中调用本地C语言风格的动态链接库。运行及部署依赖Python和npm，另外需要区别处理32位和64位的程序调用，尤其是不能支持ActiveX控件等面向对象的组件调用，无法和网页融为一体运行。

使用PluginOK(牛插)中间件的理由：
1、轻量级：整个程序包很小，再无依赖其它运行库或第三方支持库即可使用；
2、强兼容性：采用HTML5标准中的Web Socket技术，可确保在各个浏览器版本的兼容使用；
3、在Windows平台采用COM组件技术为上层小程序开发提供友好的集成支持，支持大多数的开发语言；
4、可配置和灵活的程序升级支持，支持OEM，方便第三方集成到自己的业务系统中。

使用场景举例：
1、网页中需要和本地电脑的硬件进行交互，比如B/S架构的OA系统中操作本地打印机；
2、网页中需要调用本地程序的ActiveX控件实现一些特殊服务，比如Office文档的内嵌在线编辑；
3、一些软件系统使用了第三方的DLL功能模块，可通过本中间件实现在B/S架构的系统中调用；
4、网银、在线支付等安全性要求高的网站，可基于本中间件开发安全控件、访问U盾等的加密模块提供访问安全性；
5、开发去中心化的分布式系统应用，如充分利用分散的系统计算能力。

针对不同的业务使用场景，PluginOK支持三种类型的小程序：
A、无界面交互的无窗口小程序(DLL)，实现为COM进程内组件，可用于封装各种硬件设备的驱动库及无界面交互的Windows API功能模块等，此类型小程序和PluginOK的主服务运行于同一进程，拥有较高的系统访问权限，一般不能访问当前桌面登录用户的注册表及相关配置；
B、有界面交互的弹窗小程序(EXE)，此类型小程序是普通的Win32执行程序，主要是封装有界面交互如打印机、扫描仪、高拍仪等的ActiveX控件给前端调用，弹出类似网页的窗口运行，权限和普通桌面应用一样；
C、有界面交互的内嵌窗口小程序(EXE)，此类型小程序也是普通的Win32执行程序，主要是封装有界面交互如视频播放、办公软件的ActiveX控件给前端以内嵌网页的形式运行，体验效果和原IE中的ActiveX控件和NPAPI插件一样。

PluginOK中间件授权：商业用途需付费使用，非商业用途可申请免费使用授权，http://local.zorrosoft.com/ 提供开发版授权可在线体验。

PluginOK中间件大记事：
PluginOK(牛插)中间件已于2019年5月发布第一个正式的单机版，实现支持无界面交互的无窗口DLL小程序及有界面交互的弹窗EXE小程序。
2020年7月13日发布网页中可内嵌窗口运行的小程序版本，同时发布了Flash Player、IE控件及新标签等内嵌窗口小程序供大家体验。
2020年8月13日正式发布网络版，不连接外网也可使用，相对于以前的单机版，软件授权费大幅度降低，欢迎申请试用！

技术咨询及获取报价信息请微信联系：ZorroSoft、qq972340118，开发交流QQ群：23126938，点击链接加入：https://jq.qq.com/?_wv=1027&k=5FxgskL

目录说明：
Bin目录，单机绿色版程序包，InstallWrl.bat执行安装中间件，RemoveWrl.bat执行卸载中间件，功能测试请参考TestWrl.txt。
WrlSDK目录，单机版SDK，包含开发接口说明、开发小程序范例工程、小程序打包工具等。

Net目录，网络版版程序包，InstallWrl.bat执行安装中间件，RemoveWrl.bat执行卸载中间件，功能测试请参考TestWrl.txt。
Server目录，网络版服务端绿色版程序，InstallService.bat执行安装服务，RemoveService.bat执行卸载服务。
ZbaSDK目录，网络版SDK，包含开发接口说明、开发小程序范例工程、小程序打包工具等。

