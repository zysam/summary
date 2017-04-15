## koag 基于 koa 的项目脚手架，一年之后，仍然是一个脚手架，还是一个庞然大物？

## 项目设计
logger 加入
responeWrap 加入
restify 的简单封装
mongoose promise - bluebird，-- swen
request 的引入
test nock 的引入
mongodb options 的加入
socket 的加入， -- hank
lib/ date, number 等工具函数的引入
joi 工具的引入
Makefile 的改变
docker 目录的改变
core 目录的引入
index 文件的引入
event 引入

## 12 个项目
- klg-admin-user
- klg-proxy
- klg-persona
- klg-agenda
- klg-finance (中途废弃)
- klg-transfer (中途废弃)
- klg-logColletion
- klg-对账（中途废弃）
- klg-loanbase
- klg-note (并入klg-loanbase)
- fin_koa_loanTransfer
- fin_koa_trading

## 引申 

jenkins 配合使用
mongobooster 配合使用
docker 配合使用， docker registry.
docker-compose 使用
容器集群管理工具：shipyard, daocloud, 灵雀云, rancher，k8s 的调用
集群后；负载均衡 ha 的探索, DNS 研究，https 加密证书研究，共享储存系统的探索。
日志管理： ELK

## 团队建设：
运维：
- zstack 打造私有云的实验，测试环境
- 内网 rancher 集群管理9台 agent
- 内网 bind9 DNS 系统搭建， webmin 的管理
- 内网 docker registry, r.b.cailve.cn, 公网 registry, r.p.cailve.cn
- 容器监控
- ELK

DEV:
- 微服务下，DEV 开发模式，测试模式变更

## 未来
mq 的引入
压力测试，ELK分析
api 网关
更好的集成
更好的部署


## 总结：
从去年3月开始，koag 偷偷立项，然后争吵规范，争吵目录命名，争吵设计模式，争吵 promise, 争吵 docker, 争吵日志打印，争吵api, 争吵 config 。。。在旧系统在债务下，在运营压力下，成立 12 个项目，挤进 CI 流，集群也有点模样，DEV 在无形中使用，运维亦慢慢上手。
