# ons-1.x-plugin
ons skywalking plugin

公司采用的阿里云的消息队列 ONS 服务，使用的是 ons-client 库进行 RocketMQ 消息的发送和消费。
那么此时，我们就无法使用 SkyWalking 进行 RocketMQ 的链路追踪了。

方案一，参考 SkyWalking rocketMQ-4.x-plugin 插件的源码，修改成支持 ons-client 库的链路追踪。
ons-client 库的代码，和 rocketmq-client 的代码是非常接近的，把对应的包名改造好就可以了
