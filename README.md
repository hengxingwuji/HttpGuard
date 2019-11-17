此项目不再维护。
请转到商业版：https://www.centos.bz/2014/06/new-http-guard-release/
4.1 httpgrard介绍

HttpGuard是基于openresty,以lua脚本语言开发的防cc攻击软件。而openresty是集成了高性能web服务器Nginx，以及一系列的Nginx模块，这其中最重要的，也是我们主要用到的nginx lua模块。HttpGuard基于nginx lua开发，继承了nginx高并发，高性能的特点，可以以非常小的性能损耗来防范大规模的cc攻击。

4.2 httpgrard防cc特效
限制访客在一定时间内的请求次数
向访客发送302转向响应头来识别恶意用户,并阻止其再次访问
向访客发送带有跳转功能的js代码来识别恶意用户，并阻止其再次访问
向访客发送cookie来识别恶意用户,并阻止其再次访问
支持向访客发送带有验证码的页面，来进一步识别，以免误伤
支持直接断开恶意访客的连接
支持结合iptables来阻止恶意访客再次连接
支持白名单功能
支持根据统计特定端口的连接数来自动开启或关闭防cc模式 
详见github地址https://github.com/centos-bz/HttpGuard
