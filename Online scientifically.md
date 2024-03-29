# 科学上网方案
*更新于2023/02/24*
## 前言
本文旨在提供想要科学上网的朋友一点指导，准备探索墙外资源的朋友可以将本文作为入门参考，如果你是已经遨游太空多年的老手，就请飘过。

在你准备撸起袖管开干之前，我先要给你泼点冷水，**翻墙违法**❗️  
👉[参考资料](https://www.66law.cn/laws/1080414.aspx)👈

还准备继续吗？那就先了解一下这几个概念：

1️⃣墙、高墙、GFW
>Great FireWall，阻断网络数据传输的技术。

2️⃣翻墙、科学上网
>网络数据请求穿透GFW，实现漂洋过海。

3️⃣VPN（虚拟专用网络）
>首先要理解vpn不是专门用来翻墙的，而是数据代理的一种方式，是指定你的数据请求传送到另一个设备或程序。

文中不涉及具体操作细节，只提供教程链接。
## 方案一（初级入门）

使用封装的vpn app应用，内置了服务器线路，例如xx加速器、骆驼vpn、熊猫vpn等，此方案上手快门槛低，但容易被监控钓鱼，注意隐私泄露，手贱嘴快喜欢跟风发帖的就别用了，早晚被请喝茶。而且线路质量差网速慢，开发者有卷款跑路的风险。

也有境外老牌的vpn运营商，例如ExpressVPN等，但在国内水土不服，似乎道高一尺，墙高一丈。

对于刚准备入坑，还不清楚科学上网走出国门能干什么的，推荐Openvpn这个app上手，这是一个在Github上开源的项目。

官网地址：
https://openvpn.net
（可能需要科学上网）

App Store链接直达👇（苹果ios须登陆外区App Store）
https://itunes.apple.com/us/app/openvpn-connect/id590379981?mt=8

## 方案二（中级进阶）

使用客户端代理应用🔗翻墙服务器提供商（俗称机场或鸡场）。

### 客户端代理应用

Windows、Android、Mac、ios的客户端应用工具各不相同，本篇只介绍苹果ios系统。

苹果手机ios系统的主流代理工具有两个，Shadowrocket小火箭和QuantumultX，都是外区app store的一次性付费应用。新手推荐安装shadowrocket小火箭，中国区苹果App Store没有的，只有假的，必须登陆苹果国外App Store账号购买安装，涉及两步操作👇：

#### 1️⃣申请苹果境外账号。
参考教程：
https://zhuanlan.zhihu.com/p/367821925?utm\_id=0

#### 2️⃣给这个账号充值
用于购买app，可以淘宝买apple gift card充值，也可以用自己的外币信用卡充值。
参考教程：
https://zhuanlan.zhihu.com/p/476434200?utm\_id=0

❗️❗️❗️**重要提示：苹果手机只能在App Store里切换登陆账号，绝对不要在设置里登陆，绝对不要变更设置里的iCloud账号，否则自己的国区账号会被封号**❗️❗️❗️

### 机场推荐：

1. https://console.bywa.art/aff.php?aff=202
2. https://portal.shadowsocks.au/aff.php?aff=34097
3. 或者👇这个链接里的鸡场自行挑选试用。
   
   https://9.234456.xyz/abc.html?t=638154915450878078

⚠️如果以上链接失效，Contact Me。

在上述的准备工作都完成之后，就可以将鸡场的服务器导入Shadowrocket开启科学上网了。机场网站内有教程说明，根据教程操作。这里引用一篇👉[教程链接](https://console.bywa.art/index.php/knowledgebase/2/iOSShadowrocket.html)供参考。

>这个方案涉及较多操作步骤，却可以一劳永逸，熟悉客户端代理工具的使用，根据机场网站的教程操作，可以解决科学上网的大部分问题。
>
>建议常备多个机场轮换使用，以防机场服务器故障维护或被同行攻击。
>
>建议购买短期套餐，近2年已发生过多起鸡场主卷款跑路的情况。
>
>服务器是共享的，成百上千的人在同时使用，出口流量容易被堵塞断流。
>
>同样有后台窃取用户隐私信息的风险。

## 方案三（高阶）

使用客户端代理应用🔗自己搭建境外服务器。

客户端操作同方案二，重点是如何搭建个人专用的境外服务器，需要一些网络知识储备，涉及域名注册、域名DNS解析、Linux命令行操作……

### 服务器厂商推荐：

#### Oracle甲骨文
Oracle的终身免费服务器，一个账号可以申请2台服务器，10T/月总流量，性价比最高，日常使用绝对够用了，除非有超大数据量或特殊应用需求。缺点是一个账号只能固定一个地区线路，在注册时选择后不能更改。
申请参考教程：
https://zhuanlan.zhihu.com/p/352736372?utm\_id=0

⚠️Ps：据说甲骨文近期已停止对个人用户开放注册，而且出台了试用服务器的回收政策。

👉[官网原文链接](https://docs.oracle.com/en-us/iaas/Content/FreeTier/freetier_topic-Always_Free_Resources.htm)
👉[防回收攻略](https://lala.im/8589.html)

#### AWS亚马逊
亚马逊云服务器的Lightsail和ECC（EC2），新注册账号后，Lightsail服务器免费试用3个月，100G/月总流量，ECC服务器免费试用一年，同样100G/月总流量。两种类型都可以随意选择区域线路。Lightsail和ECC是分开计费的，所以试用期内可以各申请一台。由于亚马逊云服务器的计费方式限制了使用时间750小时/月和30G/月弹性储存容量，所以增加服务器数量会被反薅收费。
申请参考教程：
https://www.youtube.com/watch?v=GXIVvAEGP6w （须要科学上网）

#### 搬瓦工及其他付费类服务器供应商
这是土豪方案，根据自己需求选择服务器性能。但这类服务器是高墙重点封控对象，某些特殊时期可能会被封控断流。
参考教程：
https://youtube.com/playlist?list=PL781TkNqYVmpUmAf5DpOXbEoEAStYYZoH （须要科学上网）

#### 关于中转服务器
国内的阿里云、腾讯云服务器可以尝试作为中转节点连接境外服务器，用来提速科学上网。因其都有各自专用的出境线路，出口带宽要远大于个人用户的出口带宽。但需付费基本没有薅羊毛方案，非必选项。只要自己的境外服务器没有被墙，直连的网速也够用了。

### 配置服务器
在拥有了自己的服务器后，如何建站配置服务器的科学上网环境，就根据网上教程自学吧。提供以下资料源供参考：（须要科学上网）

* https://www.youtube.com/watch?v=_618At72evs&list=PL5TbbtexT8T3d_7UX2aSFhoMYk-cl4kf4
* https://www.youtube.com/watch?v=Stdj6U568S0
* https://www.youtube.com/watch?v=d3WixFDz5BA
* https://www.v2fly.org
* https://github.com/XTLS/Xray-core
* https://github.com/kirin10000/Xray-script
* https://github.com/mack-a/v2ray-agent

……
# 后记
## 这里再给新手做一些科普。
有了一家鸡场，或者自己已经搭建了一台境外服务器，是不是能够畅游全球了？
>答：不是的！不能够！
>>举例来说，一台vpn服务器可以让你和ChatGPT互动的，却未必能够全解锁Netflix，能够全解锁Netflix的，却未必能够全解锁Disney+。即使这些都可以，你还是不能直接看TikTok。这些应用网商都对客户数据请求来源有严格的要求，会检测ip，会探测是否使用了代理工具。当然所有的问题都是有解决办法的，看有没有硬需求去学习吧。但不要期望一证通行，入坑之后就学无止尽了。

为什么科学上网的网速没别人家的快？而且使用同样的鸡场，同样的套餐；或者相同地区的服务器，相同性能的机型。
>答：影响网速体验的因素很多，列举以下几点，但不限于这些。
>>服务器（或称节点）只是数据传送过程中的一个环节，网速会受到传输链瓶颈的限制，比方说你家里的带宽只有50Mbps，那么即使服务器厂商能够提供你100Mbps出口带宽，你也只能体验50Mbps的网速。
>>
>>本地网络运营商（ISP）电信、移动、联通的宽带（简称三网）在高峰时段限速，从而影响到网速表现。
>>
>>本地的设备性能和组网方式也都会影响网速体验。    

同一个网站，为什么别人家里能直接打开，我却要开启翻墙才能打开？
>答：墙有高低，环境有优劣。
>>举例来说，github这个开源项目托管网站在一些地区是被封锁的，但在我这里没有被封，可以直接打开。
>>
>>再举例，Ookla的speedtest这个全球最好的测速工具，我朋友家用的电信宽带要翻墙才能使用，只能解析到境外的测速服务器，这样实际测试的是墙外回程网速，而非本地宽带网速。本人用的移动宽带是可以直接解析到本地服务器测速宽带网速的。
>>
>>继续举例，家庭组网会玩软路由或是会刷路由器的，就可以配置科学上网应用到路由器里，实现局域网内所有设备都能翻墙，不需要在终端上开启代理应用了。这样有人就会凡尔赛了“我直接就能打开了呀”🤙🤙🤙
