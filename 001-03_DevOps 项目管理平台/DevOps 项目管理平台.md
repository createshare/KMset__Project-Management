# DevOps 项目管理平台



# DevOps 

## DevOps 简介

DevOps 包括组织文化、自动化、精益、反馈和分享等不同方面。组织架构、企业文化与理念等，需要自上而下设计，用于促进开发部门、运维部门和质量保障部门之间的沟通、协作与整合，简单而言组织形式类似于系统分层设计。

DevOps 强调的是高效组织团队之间如何通过自动化的工具协作和沟通来完成软件的生命周期管理，从而更快、更频繁地交付更稳定的软件。DevOps 是把人员、流程、产品进行结合，给用户提供持续价值的一个过程，既涉及到人员、流程、工具，也涉及到产品。

DevOps 最终目的是给客户提供持续交付的价值，流程包括：产品的规划跟踪、软件开发、构建测试、产品部署、运维、监控和优化。
通常把 DevOps 这些流程通过一个流水线的方式串联起来称为一个 DevOps 的流水线，其核心目标就是持续给用户交付有价值的产品。

DevOps 已经从开发运维一体化，扩大到“端到端”的概念。

![DevOps](figures/DevOps.png)

DevOps = 人（People）+ 流程（Process）+ 平台（Platform）

![DevOps = 人（People）+ 流程（Process）+ 平台（Platform）](figures/DevOps = 人（People）+ 流程（Process）+ 平台（Platform）.png)

## DevOps 好处与价值

对于业务与产品而言，DevOps的好处更多基于持续部署与交付。

从组织结构而言，DevOps是部门间沟通协作的一组流程和方法，有助于改善公司组织文化、提高员工的参与感。主要包括代码管理、持续集成、自动化测试、自动化部署、基础设施自动化管理等方面的工程能力。

- 代码的提交直接触发：消除等待时间，快速反馈。
- 每个变化对应一个交付管道：使问题定位和调试变得简单。
- 全开发流程高效自动化：
  - 自动化是指所有的操作都不需要人工参与，全部依赖系统自动完成，持续交付过程必须自动化才有可能完成快速迭代。
  - 稳定，快速，交付结果可预测。
  - 简化重复性工作和减少不必要的等待。
  - 建设自动化、可重复、可靠的持续交付流水线（IT服务供应链）。
- 持续进行自动化回归测试：提升交付质量。
  - 每次代码提交都需要经过流水线验证.
  - 每次部署的版本都经过多环境验证
- 设施共享并按需提供：资源利用最大化。
  - 部署频率可以得到提升
  - 周期时间（从代码提交到部署上线）的时间可以到分钟级

## DevOps 能力环

![DevOps 能力环](figures/DevOps 能力环.png)

# DevOps 与 敏捷、精益

时刻关注正在做什么，尝试识别问题范围，找出解决方案和改善途径。

持续且快速、可靠的自动交付软件给用户：

![DevOps、敏捷开发、瀑布式开发，关系与演进](figures/DevOps、敏捷开发、瀑布式开发，关系与演进.png)

# DevOps 与 持续集成、持续交付（CD/CD）

DevOps的应用场景往往是一个庞大复杂的背景和流程的场景，大都包含一个持续交付流水线。

DevOps 是一个完整的面向 IT 运维的工作流，以 IT 自动化以及持续集成（CI）、持续部署（CD）为基础，来优化程式开发、测试、系统运维等所有环节。

- 开发人员：IDE、Git 等开发和编译工具
- 版本控制系统：分支策略、语义化版本
- 构建服务器：持续集成、代码质量检查
- 工件库：存放二进制包
- 系统的包管理器：编译或测试环境系统上管理二进制包
- 环境一致性
- 预发布或生产：预发布环境与生产环境互换（蓝绿发布）
- 发布管理：在高程度自动化测试的基础上实践自动化或半自动化（人工介入）部署
- 问题管理系统



## 典型的 CI/CD 流水线过程

- 项目开发编写代码，然后把代码推送到 GitLab 里存储，通过 GitLab 的 hook 使 Jenkins 执行一些 CI 的过程，比如做一些单元测试，构建 Docker image。
- 再把这个 Docker image 调用 helm 部署到开发环境或测试环境。
- 在测试环境里通过 Jenkins 触发一个集成测试的功能。
- 完成后就可以把它部署到生产环境。
- 通过 Kubernetes addon 的方式，把 Prometheus、Grafana 等监控组件部署到集群里，实现一整套从 CI 到 CD 的监控过程。

![典型的 CI-CD 流水线过程](figures/典型的 CI-CD 流水线过程.png)





# DevOps 完整过程

## 一个完整的过程

- 开发团队接到任务，需要完成一个变更
- 为了更加顺利地开发，将这个变更分拆为几个小变更
- 开发人员在本地开发并且测试，如果使用了测试驱动开发，在编写功能代码之前会先编写测试，然后编写能够让测试通过的实际代码
- 开发人员将代码提交到企业内部的Git版本控制系统上
- 构建服务器获取这个变更并初始化构建流程，单元测试之后，变更可以被发布到二进制库里
- 配置管理系统根据“策略”，在测试环境中安装应用了新的变更
- 新安装触发自动化回归测试，测试成功后，质量保证团队开始做人工测试
- 人工测试通过后，质量保证团队将“已通过”标识给予这个变革
- 变更在预发布环境中进行验收测试
- 验收测试完成后，预发布环境被切换成生产环境，而生产环境变为新的预发布环境



# DevOps 工具集

![DevOps 工具集](figures/DevOps 工具集.jpg)

![DevOps 工具集](figures/DevOps 工具集2.png)



## DevOps 平台搭建工具项目管理（PM）: Jira、Asana、Taiga、Trello、Basecamp、Pivotal Tracker

运营可以上去提问题，可以看到各个问题的完整的工作流，待解决未解决等；代码管理：gitlab。jenkins或者K8S都可以集成gitlab，进行代码管理，上线，回滚等。

## 配置管理：Ansible、Chef、Puppet、SaltStack、ScriptRock GuardRail



## 代码管理（SCM）：GitHub、GitLab、BitBucket、SubVersion

## 构建工具：Ant、Gradle、maven

## 持续集成CI（Continuous Integration）：GitLab CI、Bamboo、Hudson、Jenkins

开发人员提交了新代码之后，立刻进行构建、（单元）测试。根据测试结果，我们可以确定新代码和原有代码能否正确地集成在一起。

## 持续交付CD（Continuous Delivery）：GitLab CD

## 压力测试：JMeter、Blaze Meter、loader.io

## 自动部署：Capistrano、CodeDeploy



## 编排：Kubernetes、Core、Apache Mesos、DC/OS

## 容器：Docker、LXC、第三方厂商如AWS

## 镜像仓库：VMware Harbor



## 日志管理：Cat+Sentry，还有种常用的是ELK

## 公司内部文档：Confluence

## 平台： Rancher

## 服务注册与发现：Zookeeper、etcd、Consul

## 系统监控：Prometheus、Datadog、Graphite、Icinga、Nagios

## 性能监控：AppDynamics、New Relic、Splunk

## 预警：PagerDuty、pingdom、厂商自带如AWS SNS

## 日志管理：Cat+Sentry、ELK、Logentries

## 负载均衡：Nginx

## 网关：Kong，zuul

## 应用服务器：Tomcat、JBoss

## Web服务器：Apache、Nginx、IIS

## 数据库：MySQL、Oracle、PostgreSQL等关系型数据库；cassandra、mongoDB、redis等NoSQL数据库

## 产品和UI图：蓝湖

## 脚本语言：Python、ruby、shell





# DevOps 注意事项

DevOps 绝不是推荐一定要在某一方面达到极致，而是从“整体”入手，充分激发“体系”的最佳效率。

DevOps 的有效实施需要依赖一定的土壤，即敏捷的基础设施服务，现实只有云计算的模式才能满足整体要求。

DevOps  涉及多个技术支撑：敏捷开发、持续集成&部署、微服务、容器、云环境等。



# AA 一级标题

## BB 二级标题

### CC 三级标题



# AA 一级标题

## BB 二级标题

### CC 三级标题



# AA 一级标题

## BB 二级标题

### CC 三级标题



# AA 一级标题

- xxxxxxxx
- xxxxxxxx

## BB 二级标题

- [ ] xxxxxxxx
- [ ] xxxxxxxx

### CC 三级标题

1. xxxxxxxx
2. xxxxxxxx



```bash

```



![XXX](figures/XXX.drawio.png)

![XXX](figures/XXX.jpg)



