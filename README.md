# Learning_Microservice
微服务学习，本项目旨在搭建一套微服务架构的在线教育SaaS平台。技术栈会尽量选用最新稳定版。
## 技术栈
- Java 21
- Spring Cloud Alibaba 2023.0.3.2
- Spring Cloud 2023.0.5
- Spring Boot 3.2.12
- Nacos 3.0.1
- Sentinel 1.8.6
- Seata 2.0.0
- RocketMQ 5.1.4
- MySQL 8.0.42
## 项目代码结构
```
Learning_Microservice       # 项目根目录
|-- auth-service            # 认证服务50100        
|-- question-service        # 题库服务50200
|-- plan-service            # 计划服务50300
|-- exam-service            # 考试服务50400
|-- evaluation-service      # 考评服务50500
|-- certificate-service     # 证书服务50600
|-- order-service           # 订单服务50700
|-- ops-service             # 运营服务50800
|-- gateway-service         # 网关服务50010
```
## 搭建开发环境
1. 启动容器：docker-compose up -d
2. 使用DBeaver连接MySQL数据库，并在nacos数据库执行数据库脚本 nacos-mysql.sql
3. 访问Nacos：http://localhost:50020，账号密码：nacos/nacos

使用DBeaver连接时可能会报“Public Key Retrieval is not allowed”，解决办法是在url连接上加：?allowPublicKeyRetrieval=true&useSSL=false
## 功能清单
### 后台管理端
### PC考生端
### PC考试桌面端
### H5考生端