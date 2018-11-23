# elk应用
## Introduction
利用docker-compose搭建一套可以使用的elk

## Solve
* 收集来自各个系统的nginx&celery等相关日志。
* 利用logstash来接收filebeat的数据。宿机上面的filebeat配置见本项目的filebeat/。
* 反向代理到nginx，并且增加简单的auth验证。

## todo
- [x] 用nginx把elk套起来
- [x] 用二级域名或二级路由代理起来
- [x] 给nginx增加简单auth
- [ ] 端口加ssl验证，才能接收数据
- [ ] 增加第三方登录系统, eg: google
