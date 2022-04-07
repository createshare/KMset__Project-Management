# 目录
[[_TOC_]] 

# 开发流程：Git 管理

## 分支管理

### feature 分支

feature 分支，用于开发各个模块功能。

feature 分支开发流程：

- 根据产品软件需求，新建一个 “小 Task” 的 feature 分支
- feature 分支命名：方法一：以功能命名（例 wi-fi-rw007） 方法二：以自己的名字命名：（例：blues）
- 完成此 feature 的代码和功能开发
- 在此 feature 分支完成 单元测试
- 单元测试通过，Merge 到 develop 分支。（如果项目比较大，多人一起开发，则需要提 Merge 到 develop分支的 PR， 需要有一个人管理 develop 分支）



### develop 分支

- 当有代码或文档 commit / merge 到 develop 分支时，自动触发：代码静态扫描、CI 编译代码、CI 编译文档

### master 分支
- 当需要 Release时，需要 在Gitlab上提Merge Request， merge 当前面 develop 分支 到 master 分支；
- master 分支，用于Release 和 Review；
- 当有代码或文档 commit / merge 到 master 分支时，自动触发：代码静态扫描、CI 编译代码、CI 编译文档；

### Tag
- 每次 Release 时，必须从 master 分支上，建一个 Tag。
- Tag 命名：以软件版本号命名。