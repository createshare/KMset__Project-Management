# GitLab 企业内部的仓库管理系统

GitLab  是一个用于仓库管理系统的开源项目，使用 Git 作为代码管理工具，并在此基础上搭建起来的 Web 服务。



2022 年 2 月消息，极狐（GitLab）正式宣布推出极狐 GitLab SaaS （JihuLab.com），为中国用户提供从源代码托管到开发运维的全栈式一体化 DevOps SaaS 平台与企业级专家咨询服务。

# GitLab 基本概念

GitLab 是一个基于 MIT 协议的开源项目，代码仓库地址是 https://github.com/gitlabhq/gitlabhq

GitLab 最初是由程序员 Dmitriy Zaporozhets 和 Valery Sizov 利用 Ruby 编写的一个基于 Git 的代码仓库托管系统，后来一些部分被 Go 重写。

最初的 GitLab 完全免费，自2013年，GitLab 被拆分为免费的社区版本和基于社区版且包含了更多高级功能的收费企业版。

2014年，GitLab 有限公司成立，GitLab己经由GitLabInc.拥有。
GitLab 能被部署到自己的服务器上，更安全可靠，适合企业级别的团队内部协作开发，已被很多大公司或组织采用，如IBM、NASA、阿里巴巴等。



# GitLab 的功能描述

现如今，GitLab 已经不完全将自己定位成代码托管工具，而是扩展并整合了项目管理、持续集成工具，由项目规划到代码版本控制，再到持续集成/持续交付的全流程覆盖的一站式项目管理工具。使之演变为完整的项目开发运维 DevOps 工具链。

GitLab 自带相应的 web 服务提供了良好的交互界面，并且有完善的问题追踪和 Wiki 功能。

## GitLab vs GitHub

- 同 GitHub 一样，GitLab 也是第三方基于 Git 打 造的代码托管工具。
- 现如今使用最为广泛的仓库托管平台依然是GitHub，这依赖于其强大的开发者社区。
- 搭建在自有服务器
  - GitHub只有企业版能搭建在自有服务器，但是价格高昂。
  - GitLab 除了云端托管服务，其最典型的场景是提供安装包搭建在私有服务器上，对于企业来说会更加安全可靠。而 GitLab 社区版是免费的。
- 在仓库开发管理功能上，相比于GitHub，GitLab的优势是：
  - 通过受保护的分支（protectedbranch），让项目管理者针对分支的创建、并入（merge）或者推送(push)设定权限，如设定仅维护者可以向develop分支推送代码、任何人都不能向master分支合并代码等。GitHub中仅有付费用户有受保护分支的功能。
  - 除了仅面向开发者设置的读、写权限以外，对项目成员的权限设置更加细致，有 Guest、Reporter、Developer、Maintainer和Owner等多角色设定。
  - 通过容器注册（containerregistry）功能，可以直接将仓库代码打包上传到 GitLab 的docker镜像服务器，制作自己的docker镜像。为后续的部署或持续集成做准备。
  - 提供内置的持续集成 CI 解决方案，不再需要用额外的 Jenkins 等工具打造 CI 流程，极大地方便了项目的交付集成管理。
  - GitLab 的免费私有项目没有核对合作者数量的限制，而且项目可见度除了可设置公开或私有外，还有另一选项——内部（Internal)，内部项目只对进入 GitLab 的用户可见。
- GitLab 在权限管理、持续集成整合等方面的独到之处，在企业级别的大团队协作开发项目中越来越流行。



## GitLab 云托管服务：Git 

GitLab 提供了类似于 GitHub 的免费云托管服务，打开 GitLab 的主页 https://about.gitlab.com/  后可以看到，注册步骤很简单，仅需填写用户名、邮箱就能注册成功，登录后就能看到简洁的项目托管界面。

- 可以创建项目(Project)，这里的项目是指核心的Git代码仓库外加 issue 跟踪、Wiki 等周边服务，还能创建类似于 GitHub 中组织的团体（group），并浏览查找其他开源项目。
- GitLab 项目创建好后，可以直接在web界面添加分支、编辑、提交代码等，或者将仓库克隆到本地，在本地进行开发工作。
- GitLab 为付费用户提供了更多高级功能，如代码质量扫描、更强大的 Cl pipeline 资源、安全测试检测、技术支持等。

## GitLab CI/CD

GitLab CI/CD（后简称 GitLab CI）是一套基于 GitLab 的 CI/CD 系统，需要让开发人员在仓库根目录下创建 .gitlab-ci.yml 文件在项目中配置 CI/CD 流程，并且使用Gitlab Runner执行该脚本。在提交后，系统可以自动/手动地执行任务，完成 CI/CD 操作。

而且，它的配置非常简单，CI Runner 由 Go 语言编写，最终打包成单文件，所以只需要一个 Runner 程序、以及一个用于运行 jobs 的执行平台（如裸机+SSH，Docker 或 Kubernetes 等，我推荐用 Docker，因为搭建相当容易）即可运行一套完整的 CI/CD 系统。





## Wiki 功能



## issue 跟踪











![XXX](figures/XXX.jpg)



