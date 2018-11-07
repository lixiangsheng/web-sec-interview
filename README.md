 # web-sec-interview
 - [ ] 介绍一下自认为有趣的挖洞经历（或CTF经历）
 
 - [ ] 你平时用的比较多的漏洞是哪些？相关漏洞的原理？以及对应漏洞的修复方案？
 
 - [ ] php/java反序列化漏洞的原理?解决方案?
 
 - [ ] 如果一台服务器被入侵后,你会如何做应急响应?
 
 - [ ] 你平时使用哪些工具?以及对应工具的特点?
 
 - [ ] 如果遇到waf的情况下如何进行sql注入/上传Webshell怎么做？请写出曾经绕过WAF的经过(SQLi，XSS，上传漏洞选一) 
 
    <a href="https://xz.aliyun.com/t/265/">我的WafBypass之道（SQL注入篇）</a>
  
    <a href="https://xz.aliyun.com/t/337/">我的WafBypass之道（Upload篇）</a>
  
    <a href="https://xz.aliyun.com/t/265/">我的WafBypass之道（Misc篇）</a>
  
 - [ ] SQLi
 - [ ] 如何判断sql注入，有哪些方法
 - [ ] 介绍 SQL 注入漏洞成因，如何防范？注入方式有哪些？除了数据库数据，利用方式还有哪些？
 - [ ] 为什么有的时候没有错误回显，用php举例
 - [ ] 宽字符注入的原理？如何利用宽字符注入漏洞，payload如何构造？
 - [ ] 你都了解哪些sql 的bypass技巧
 - [ ] CRLF注入的原理
 - [ ] sqlmap如何对一个注入点注入?
   - 如果是get型，直接，sqlmap -u “诸如点网址”. 
   - 如果是post型，可以sqlmap -u “注入点网址” –data=”post的参数” 
   - 如果是cookie，X-Forwarded-For等，可以访问的时候，用burpsuite抓包，注入处用*号替换，放到文件里，然后sqlmap -r “文件地址”
 - [ ] mysql的网站注入，5.0以上和5.0以下有什么区别？
   - 5.0以下没有information_schema这个系统表，无法列表名等，只能暴力跑表名。
   - 5.0以下是多用户单操作，5.0以上是多用户多操做。
 - [ ] mysql注入点，用工具对目标站直接写入一句话，需要哪些条件？
  - root权限以及网站的绝对路径。
 - [ ] 以下链接存在 sql 注入漏洞，对于这个变形注入，你有什么思路？ 
 > demo.do?DATA=AjAxNg== 

 - [ ] Domain
 - [ ] 解释一下同源策略
 - [ ] 同源策略，那些东西是同源可以获取到的
 - [ ] 如果子域名和顶级域名不同源，在哪里可以设置叫他们同源
 - [ ] 如何设置可以跨域请求数据？jsonp是做什么的？

 - [ ] Ajax
 - [ ] Ajax是否遵循同源策略？
 - [ ] json注入如何利用

 - [ ] 浏览器策略
 - [ ] 不同浏览器之间，安全策略有哪些不同，比如chrome，firefox，IE
 - [ ] CSP是什么？如何设置CSP？

 - [ ] XSS
 - [ ] xss的发生场景？
 - [ ] 如果给你一个XSS漏洞，你还需要哪些条件可以构造一个蠕虫？
 - [ ] 在社交类的网站中，哪些地方可能会出现蠕虫？
 - [ ] 如果叫你来防御蠕虫，你有哪些方法？
 - [ ] 如果给你一个XSS盲打漏洞，但是返回来的信息显示，他的后台是在内网，并且只能使用内网访问，那么你怎么利用这个XSS？
 - [ ] 如何防范 XSS 漏洞，在前端如何做，在后端如何做，哪里更好，为什么？
 
 - [ ] PHP
 - [ ] php里面有哪些方法可以不让错误回显？
 - [ ] php.ini可以设置哪些安全特性
 - [ ] php的%00截断的原理是什么？
 - [ ] webshell检测，有哪些方法
 - [ ] php的LFI，本地包含漏洞原理是什么？写一段带有漏洞的代码。手工的话如何发掘？如果无报错回显，你是怎么遍历文件的？

 - [ ] CSRF
 - [ ] CSRF漏洞的本质是什么？
 - [ ] 防御CSRF都有哪些方法，JAVA是如何防御CSRF漏洞的，token一定有用么？

 - [ ] HTML5
 - [ ] 说说HTML5有哪些新的安全特性
 - [ ] HTML5白名单要有哪些标签

 - [ ] java
 - [ ] 你都了解哪些java框架？
 - [ ] java的MVC结构都是做什么的，数据流向数据库的顺序是什么？
 - [ ] 了解java沙箱吗？
 - [ ] ibats的参数化查询能不能有效的控制sql注入？有没有危险的方法可以造成sql注入？
 - [ ] 说说两次struts2漏洞的原理
 - [ ] ongl在这个payload中起了什么作用？
 - [ ] \u0023是什么字符的16进制编码？为什么在payload中要用他？
 - [ ] java会不会发生执行系统命令的漏洞？java都有哪些语句，方法可以执行系统命令
 - [ ] 如果叫你修复一个xss漏洞，你会在java程序的那个层里面进行修复？
 - [ ] xss filter在java程序的哪里设置？
 - [ ] 说下java的类反射在安全上可能存在哪些问题

 - [ ] 中间件
 - [ ] tomcat要做哪些安全加固？
 - [ ] 如果tomcat重启的话，webapps下，你删除的后台会不会又回来？
 - [ ] 常见的网站服务器中间件容器。
  - IIS、Apache、nginx、Lighttpd、Tomcat
  - JAVA中间件[Tomcat/Jetty/JBOSS/WebLogic/Coldfusion/Websphere/GlassFish]
 - [ ] 说说常见的中间件解析漏洞利用方式  
  - IIS 6.0
    - /xx.asp/xx.jpg "xx.asp"是文件夹名
  - IIS 7.0/7.5
    - 默认Fast-CGI开启，直接在url中图片地址后面输入/1.php，会把正常图片当成php解析
  - Nginx
    - 版本小于等于0.8.37，利用方法和IIS 7.0/7.5一样，Fast-CGI关闭情况下也可利用。
    - 空字节代码 xxx.jpg%00.php
  - Apache
    - 上传的文件命名为：test.php.x1.x2.x3，Apache是从右往左判断后缀
  - lighttpd
    - xx.jpg/xx.php

 - [ ] 数据库
 - [ ] mysql数据库默认有哪些库？说出库的名字
 - [ ] mysql的用户名密码是存放在那张表里面？mysql密码采用哪种加密方式？
 - [ ] mysql表权限里面，除了增删改查，文件读写，还有哪些权限？
 - [ ] mysql安全要如何做？
 - [ ] sqlserver public权限要如何提权
 - [ ] Windows、Linux、数据库的加固降权思路，任选其一  

 - [ ] Linux
 - [ ] 简述Linux系统安全加固需要做哪些方面
 - [ ] 你使用什么工具来判断系统是否存在后门
 - [ ] Linux的Selinux是什么？如何设置Selinux？
 - [ ] iptables工作在TCPIP模型中的哪层？
 - [ ] 如果无法升级内核，那么如何保证系统不被已知的exp提权？
 - [ ] syslog里面都有哪些日志？安装软件的日志去哪找？
 - [ ] 如何查询ssh的登录日志？如何配置syslog的日志格式？
 - [ ] syslog可不可以使用vi等工具直接查看？是二进制文件吗？

 - [ ] 信息采集
 - [ ] 踩点都要采集哪些信息？
 - [ ] DNS在渗透中的作用
 - [ ] 如何绕过CDN获取目标网站真实IP，谈谈你的思路？  
 
 - [ ] 如果给你一个网站,你的渗透测试思路是什么?
 在获取书面授权的前提下。 
 - 1)信息收集， 
   - 1，获取域名的whois信息,获取注册者邮箱姓名电话等。 
   - 2，查询服务器旁站以及子域名站点，因为主站一般比较难，所以先看看旁站有没有通用性的cms或者其他漏洞。 
   - 3，查看服务器操作系统版本，web中间件，看看是否存在已知的漏洞，比如IIS，APACHE,NGINX的解析漏洞 
   - 4，查看IP，进行IP地址端口扫描，对响应的端口进行漏洞探测，比如 rsync,心脏出血，mysql,ftp,ssh弱口令等。 
   - 5，扫描网站目录结构，看看是否可以遍历目录，或者敏感文件泄漏，比如php探针 
   - 6，google hack 进一步探测网站的信息，后台，敏感文件
 - 2）漏洞扫描 
   - 开始检测漏洞，如XSS,XSRF,sql注入，代码执行，命令执行，越权访问，目录读取，任意文件读取，下载，文件包含， 
 远程命令执行，弱口令，上传，编辑器漏洞，暴力破解等 
  - 3）漏洞利用 
    - 利用以上的方式拿到webshell，或者其他权限 
  - 4）权限提升 <br>
    - 提权服务器，比如windows下mysql的udf提权，serv-u提权，windows低版本的漏洞，如iis6,pr,巴西烤肉， 
    - linux脏牛漏洞，linux内核版本漏洞提权，linux下的mysql system提权以及oracle低权限提权 
  - 5）日志清理 <br>
  - 6）总结报告及修复方案<br>
 
 - [ ] 谈一谈Windows系统与Linux系统提权的思路？  
 
 - [ ] 列举出您所知道的所有开源组件高危漏洞(十个以上)  
 
 - [ ] 反弹 shell 的常用命令？一般常反弹哪一种 shell？为什么？
 
 - [ ] 描述一个你深入研究过的 CVE 或 POC。
 
 - [ ] CSRF 和 XSS 和 XXE 有什么区别，以及修复方式？ 
 
   - XSS是跨站脚本攻击，用户提交的数据中可以构造代码来执行，从而实现窃取用户信息等攻击。修复方式：对字符实体进行转义、使用HTTP Only来禁止JavaScript读取Cookie值、输入时校验、浏览器与Web应用端采用相同的字符编码。 
  
   - CSRF是跨站请求伪造攻击，XSS是实现CSRF的诸多手段中的一种，是由于没有在关键操作执行时进行是否由用户自愿发起的确认。修复方式：筛选出需要防范CSRF的页面然后嵌入Token、再次输入密码、检验Referer。
  
   - XXE是XML外部实体注入攻击，XML中可以通过调用实体来请求本地或者远程内容，和远程文件保护类似，会引发相关安全问题，例如敏感文件读取。修复方式：XML解析库在调用时严格禁止对外部实体的解析。
  
 - [ ] CSRF、SSRF和重放攻击有什么区别？ 
 
   - CSRF是跨站请求伪造攻击，由客户端发起 
  
   - SSRF是服务器端请求伪造，由服务器发起 
  
   - 重放攻击是将截获的数据包进行重放，达到身份认证等目的
  
 - [ ] 说出至少三种业务逻辑漏洞，以及修复方式？ 
 
   - 密码找回漏洞中存在密码允许暴力破解、存在通用型找回凭证、可以跳过验证步骤、找回凭证可以拦包获取等方式来通过厂商提供的密码找回功能来得到密码 
  
   - 身份认证漏洞中最常见的是会话固定攻击和 Cookie 仿冒，只要得到 Session 或 Cookie 即可伪造用户身份 
  
   - 验证码漏洞中存在验证码允许暴力破解、验证码可以通过 Javascript 或者改包的方法来进行绕过
  
 - [ ] 发现 demo.jsp?uid=110 注入点，你有哪几种思路获取 webshell，哪种是优选？ 
 

 
  - [ ] CMD命令行如何查询远程终端开放端口
 
  - [ ] 服务器为IIS+PHP+MySQL，发现root权限注入漏洞，讲讲你的渗透思路  
 
  - [ ] 说出XSS的三种类型，且在过滤”<>”号下如何绕过  
  
  - [ ] 请写出Mysql5数据库中查询库’helloworld’中’users’表所有列名的语句  
 
  - [ ] 下面这段代码存在漏洞吗？如果存在请说出存在什么漏洞并利用  
 
 >     http://www.exp.com/1.php  
 >     <?php  
 >     $s_func = $_GET['s_func'];
 >     $info = $_GET['info'];
 >     $s_func($info);
 >     ?>
 
 - [ ] 菜刀被waf拦截后要怎么处理?
 
      <a href="https://xz.aliyun.com/t/2739/">菜刀HTTP流量中转代理过WAF</a>
   

  
  - [ ] 在渗透过程中，收集目标站注册人邮箱对我们有什么价值？

    - 丢社工库里看看有没有泄露密码，然后尝试用泄露的密码进行登录后台。
 
    - 用邮箱做关键词进行丢进搜索引擎。
 
    - 利用搜索到的关联信息找出其他邮进而得到常用社交账号。
 
    - 社工找出社交账号，里面或许会找出管理员设置密码的习惯 。
 
    - 利用已有信息生成专用字典。
 
    - 观察管理员常逛哪些非大众性网站，拿下它，你会得到更多好东西。
 
 - [ ] 判断出网站的CMS对渗透有什么意义？

   - 查找网上已曝光的程序漏洞。

   - 如果开源，还能下载相对应的源码进行代码审计。

 - [ ] 一个成熟并且相对安全的CMS，渗透时扫目录的意义？

   - 敏感文件、二级目录扫描

   - 站长的误操作比如：网站备份的压缩文件、说明.txt、二级目录可能存放着其他站点


