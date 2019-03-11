# 什么是 JeeIT
## 概览
欢迎来到 JeeIT 的世界！

JeeIT 致力于帮助您快速的搭建企业级微服务生态体系。JeeIT 提供了一组简单易用的应用系统，帮助您快速实现网关路由、权限管理、用户通用数据管理等功能。

JeeIT 帮助您更敏捷和容易地构建、交付和管理微服务平台。 JeeIT 是构建以“服务”为中心的现代应用架构的服务脚手架。

## 
服务（Service）是 JeeIT 世界的一等公民。JeeIT 几乎构建了所有主流类型的“服务”的架构和管理：
* 网关服务：gateway-server
* 权限服务：oauth-server
* 用户资源服务：upms-server
* ......

## JeeIT 的关键功能包括:

* 完善登录：账号密码模式、短信验证码模式、社交账号模式均整合Spring security oAuth
* 单点登录：基于Srping security oAuth 提供单点登录接口，方便其他系统对接
* 用户管理：用户是系统操作者，该功能主要完成系统用户配置。
* 机构管理：配置系统组织机构，树结构展现，可随意调整上下级。
* 菜单管理：配置系统菜单，操作权限，按钮权限标识等。
* 角色管理：角色菜单权限分配、设置角色按机构进行数据范围权限划分。
* 动态路由：基于zuul实现动态路由，后端可配置化。
* 灰度发布：自定义ribbon路由规则匹配多版本请求。
* 终端管理：动态配置oauth终端，后端可配置化。
* 字典管理：对系统中经常使用的一些较为固定的数据进行维护，如：是否等。
* 操作日志：系统正常操作日志记录和查询；系统异常信息日志记录和查询。
* 服务限流：多种维度的流量控制（服务、IP、用户等）
* 消息总线：配置动态实时刷新
* 分库分表：shardingdbc分库分表策略
* 数据权限: 使用mybatis对原查询做增强，业务代码不用控制，即可实现。
* 文件系统: 支持FastDFS、七牛云，扩展API几行代码实现上传下载
* 消息中心：短信、邮件模板发送，几行代码实现发送
* 聚合文档：基于zuul实现 swagger各个模块的实现
* 代码生成：前后端代码的生成，支持Vue
* 缓存管理：基于Cache Cloud 保证Redis 的高可用
* 服务监控: Spring Boot Admin
* 分布式任务调度： 基于elastic-job的分布式文件系统，zookeeper做调度中心
* zipkin链路追踪： 数据保存ELK，图形化展示
* pinpoint链路追踪： 数据保存hbase，图形化展示

## JeeIT 架构
```
jeeit
├── jeeit-fintech
├
├
├
└── jeeit-cloud -- 生态应用组群
      ├── jeeit-ui -- element-vue-admin实现
      ├── jeeit-oauth -- 授权服务提供
      ├── jeeit-common -- 系统公共模块 
      ├── jeeit-config -- 配置中心
      ├── jeeit-eureka -- 服务注册与发现
      ├── jeeit-gateway -- 网关
      ├── jeeit-modules -- 微服务模块
      ├    ├── jeeit-daemon-service -- 分布式调度中心
      ├    ├── jeeit-mc-service -- 消息中心
      ├    ├── jeeit-sso-client-demo -- 单点登录客户端示例
      ├    └── jeeit-upms-service -- 权限管理提供
      ├── jeeit-visual  -- 图形化模块 
      ├    ├── jeeit-monitor -- 服务状态监控、turbine 
      └──├── jeeit-zipkin-elk -- zipkin、ELK监控
            └── jeeit-cache-cloud -- 缓存管理、统一监控
```


## JeeIT 应用群组开发进度

 ![kaifajindu](/img/kaifajindu.png)

 
## 问题反馈

1. 欢迎提交 issue，请写清楚遇到问题的原因，浏览器和操作系统环境，重现的流程。 如果有开发能力，建议在本地调试出出错的代码。

2. 不接受功能请求的issue，功能请求可能会被直接关闭，请谅解（正确的方式是打赏并附言）。


## 系统展示

 ![kaifajindu](/img/zhanshi1.png)












## 下一步
继续阅读 [快速开始](http://localhost:8080/zh-cn/docs/quick/quick-start.html) 以快速上手 JeeIT。
