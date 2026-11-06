# 技术栈建议

定位：前后端分离的 Java 全栈求职项目；后端采用模块化单体。以下为指导方案，具体依赖版本在用户初始化前重新核对并锁定，不视为已经安装。

| 层面 | 建议 |
| --- | --- |
| 前端 | Vue 3、TypeScript、Vite |
| 路由与状态 | Vue Router、Pinia |
| HTTP | Axios |
| 样式 | 普通 CSS，按需使用 Element Plus |
| Java | Java 21 |
| 后端 | Spring Boot 4.0.x、Spring MVC |
| 数据访问 | MyBatis，用户亲手编写 SQL |
| 数据库 | MySQL 8.4 LTS |
| 安全 | Spring Security；Session/Token 方案在登录设计前讨论 |
| 后续缓存 | Redis，仅在实际业务需要时引入 |
| 构建与版本 | Maven、npm、Git |
| 测试 | Spring Boot Test、JUnit、MockMvc、Vitest |
| 后续运行交付 | Docker Compose、Nginx |

前端和后端可放在同一 Git 仓库中，分别启动与构建，通过 HTTP API 通信。早期不引入微服务和消息队列。

参考：
- Vue：https://vuejs.org/guide/quick-start
- Spring Boot：https://docs.spring.io/spring-boot/4.0/tutorial/first-application/index.html
- MyBatis：https://github.com/mybatis/spring-boot-starter
- MySQL：https://dev.mysql.com/doc/refman/8.4/en/mysql-releases.html

先学会请求、SQL、事务、数据归属与失败处理，再引入更多组件；技术亮点依据实际实现和测试记录，不虚构并发量或性能指标。
