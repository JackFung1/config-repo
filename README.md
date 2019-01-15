config-repo
jhipster-microservice-demo项目的配置仓库

Config Server 中所有的配置会覆盖微服务工程下的对应配置项的配置值（不会覆盖整个文件），可在http://localhost:8761/#/config下查看各个微服务在JHipster Registry中的配置信息

默认命名规则：{微服务名}[-dev|prod].yml
可在bootstrap[-dev|prod].yml文件中修改以下配置项来定义配置文件名：

spring:
    cloud:
        config:
            name:
application.yml对所有注册的微服务和网关生效
users[-dev|prod].yml对微服务users生效
products[-dev|prod].yml对微服务products生效
gateway[-dev|prod].yml对网关gateway生效
