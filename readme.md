### Savoria外卖总体介绍

Savoria外卖是一款专门为餐饮企业（如餐厅、饭店）定制的软件产品，旨在提供高效、便捷的外卖解决方案。该项目包括系统管理后台和小程序端应用两部分，实现了从用户浏览下单到商家接单以及管理的完整流程。
### 功能演示

#### 商家登录页面
![login.png](assets/login.png)
#### 商家控制台页面
![admin-console.png](assets/admin-console.png)
#### 商家菜品管理页面
![admin-dish.png](assets/admin-dish.png)
#### 用户小程序浏览界面
![user-page.png](assets/user-page.png)
#### 用户小程序下单界面
![user-pay.png](assets/user-pay.png)

### 功能介绍

**管理端功能：**
- 员工登录/退出
- 员工信息管理
- 分类管理
- 菜品管理
- 套餐管理
- 菜品口味管理
- 订单管理
- 数据统计
- 来单提醒

**用户端功能：**
- 微信登录
- 收件人地址管理
- 用户历史订单查询
- 菜品规格查询
- 购物车功能
- 下单
- 支付
- 分类及菜品浏览

### 端的分类

项目分为两个端：
1. **管理端**：供餐饮企业内部员工使用，进行餐厅的分类、菜品、套餐、订单、员工等的管理维护。
2. **用户端**：供消费者使用，通过小程序实现在线浏览菜品、下单、支付等功能。

### 业务流程

Savoria外卖项目涵盖了以下业务流程：
- 用户通过小程序浏览菜品和套餐
- 用户将菜品添加到购物车并进行下单
- 用户完成支付
- 管理端接收订单并进行处理
- 订单状态更新和来单提醒
- 数据统计和分析

### 架构设计

项目采用前后端分离的开发模式，主要包含以下几个部分：

- **管理端前端**：
    - 基于Vue.js框架开发的SPA单页应用
    - 使用ElementUI组件库构建用户界面
    - 集成ECharts实现数据可视化
    - 通过Nginx部署静态资源并实现反向代理

- **用户端小程序**：
    - 基于微信小程序开发框架
    - 使用原生微信小程序组件
    - 集成微信支付等原生API

- **后端服务**：
    - 基于SpringBoot的单体架构应用
    - 使用MyBatis进行数据库访问
    - 集成JWT实现身份认证
    - 使用WebSocket实现实时通信
    - 集成Swagger生成API文档

- **中间件与存储**：
    - Redis缓存中间件，提升系统性能
    - 阿里云OSS对象存储，用于文件存储
    - MySQL关系型数据库，存储业务数据

### 技术栈
##### Abstract
SpringBoot, MySQL, MyBatis, AliOSS, Redis, AOP, JWT, HttpClient, Swagger, Spring Cache, Spring Task, 微信支付、WebSocket、Git

##### 项目中使用到的技术框架和中间件包括但不限于：
- **前端技术**：H5、Vue.js、ElementUI、apache echarts
- **网关技术**：Nginx
- **后端技术**：SpringBoot、MyBatis、PageHelper、Spring Data Redis
- **数据库技术**：MySQL、Redis
- **缓存技术**：Redis
- **API文档工具**：Swagger
- **支付技术**：微信支付API集成
- **文件处理**：Apache POI
- **实时通信**：WebSocket
- **云存储服务**：阿里云OSS

### 技术亮点

1. **前后端分离**：采用前后端分离架构，提升开发效率和维护性。
2. **SpringBoot单体架构**：使用SpringBoot框架快速开发，满足业务需求的同时保持代码简洁高效。
3. **Redis缓存系统**：使用Redis进行数据缓存，提高数据访问性能和系统响应速度。
4. **Spring Cache与Spring Data Redis**：集成缓存抽象和支持，简化缓存操作。
5. **JWT身份验证**：使用JWT进行安全的身份验证和授权，保障系统安全。
6. **WebSocket实时通信**：用于来单/催单功能，实现实时消息推送。

Savoria外卖项目通过结合现代软件开发技术和合理的架构设计，提供了一个完整的外卖订餐系统解决方案，不仅满足了餐饮企业的日常运营需求，也为消费者提供了便捷的点餐服务。
