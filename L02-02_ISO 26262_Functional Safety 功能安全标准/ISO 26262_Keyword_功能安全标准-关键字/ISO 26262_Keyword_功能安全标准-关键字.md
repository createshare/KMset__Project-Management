# ISO 26262_Keyword_功能安全标准-关键字

## ■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■

## FS  功能安全  Functional Safety

Functional Safety 功能安全，指不存在由电气/电子系统的功能异常表现引起的危害而导致不合理的风险。

## Functional Safety Concept  功能安全概念

Functional  Safety Concept 功能安全概念，指为了实现安全目标，定义功能安全要求及相关信息，并将要求分配到架构中的要素上，以及定义要素之间的必要交互。

## Functional Safety Requirement  功能安全要求

Functional Safety Requirement  功能安全要求，指定义了独立于具体实现方式的安全行为，或独立于具体实现方式的安全措施，包括安全相关的属性。

注1：功能安全要求可以是由安全相关的电气/电子系统或基于其他技术的安全相关系统所执行的安全要求，目的是通过考虑确定的危害事件，使相关项达到或保持在安全状态。

注2：功能安全要求的定义可独立于产品开发概念阶段中使用的技术。

注3：安全相关的属性包括ASIL等级信息。



## Safety Culture 安全文化

Safety Culture 安全文化，指组织中持久的价值观、态度、动机和认知，即：在决策和行为中， 安全优先于与之冲突的目标。

## Safety Goal 安全目标

Safety Goal 安全目标，指作为整车层面危害分析和风险评估结果的最高层面的安全要求；     

注：一个安全目标可能与几种危害有关，几个安全目标可能与一种单一的危害有关。

## 安全生命周期

包含了在概念阶段、产品开发、生产、运行、服务和报废期间的主要安全活动。



## SLC 软件生命周期 (Software Life Cycle)

https://baike.baidu.com/item/%E8%BD%AF%E4%BB%B6%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F/861455

https://wiki.mbalib.com/wiki/%E8%BD%AF%E4%BB%B6%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F

软件生命周期(Software Life Cycle,SLC)是软件的产生直到报废或停止使用的生命周期。软件生命周期内有问题定义、可行性分析、总体描述、系统设计、编码、调试和测试、验收与运行、维护升级到废弃等阶段，也有将以上阶段的活动组合在内的迭代阶段，即迭代作为生命周期的阶段。

## Lifecycle 生命周期

生命周期，指相关项从概念到报废的全部阶段，包含了在概念阶段、产品开发、生产、运行、服务和报废期间的主要安全活动。

## ASIL 汽车安全完整性等级

Automotive Safety Integrity Level 汽车安全完整性等级；
ASIL包括四个等级（A、B、C、D），每一个等级定义了相关项(Item)或者要素（Element）的必要要求和安全措施。其中，A代表最低严格等级，D代表最高严格等级。 

## ASIL Capability ASIL 等级能力

相关项或要素满足假定的、被分配了给定ASIL等级的安全要求的能力；
注：作为硬件安全要求的一部分，如果需要，还包括实现分配给要素的相应随机硬件故障度量目标值。

## ASIL Decomposition ASIL 等级分解

为有助于实现同一安全目标，将冗余的安全要求分配给具有充分独立性的要素，以降低分配给相关要素的冗余的安全要求的ASIL等级；
注1：ASIL等级分解是设计过程中ASIL等级剪裁方法的基础；
注2：ASIL等级分解不适用于随机硬件失效要求。

## QM 质量管理 Quality Management

Quality Management（QM） 质量管理，指用来指导和控制组织的针对质量的协调活动。
注：QM不是一个ASIL等级，但可以在危害分析和风险评估中定义。

## Safety Plan 安全计划

Safety Plan 安全计划，指管理和指导开展项目安全活动的计划，包括日期、里程碑节点、任务、可交付成果、职责和资源。

## Safety Case  安全档案

Safety Case 安全档案，指实现相关项或要素功能安全、收集整理开发过程中安全活动的工作成果证据来满足功能安全的论据。

将收集了开发过程中安全活动的工作成果作为证据，证明完整地实现了相关项的安全要求。

注：安全档案可被扩展，以涵盖 ISO26262 标准范围外的安全问题。

## Safety Activity 安全活动

在安全生命周期的一个或多个子阶段进行的活动。

## Safety 安全

没有不合理的风险。

## Safe State 安全状态

Safe State 安全状态：也就是当前系统的状态是不会造成危害的。 举个例子：如果枪可能发生走火，那么，枪里没有弹药就是一个安全状态。
在系统设计中，故障降级往往是普遍采用的一种方式，但故障降级并不一定就是安全状态。例如，一辆自动驾驶汽车的某一个核心传感器失效，车辆从原本的 80km/h 降至 20km/h 运行，车辆的功能受到了限制，但 20km/h 仍然具备出现汽车事故的可能性。那么，这种状态就并不是一个安全状态。

## Safety Anomaly 安全异常

Safety  Anomaly 安全异常，指偏离预期并可能导致伤害的情况；     

注：安全异常可在评审、测试、分析、编译、 组件的使用、或适用文档的使用等过程中被发现；     

示例：偏差可以是在需求、规范、设计文档、用户文档、标准或经验方面。

## Safe Fault 安全故障

Safe  Fault 安全故障，指不会显著增加违背安全目标的概率的故障；     

注1：非安全相关和安全相关要素都可能有安全故障；     

注2：单点故障、残余故障和双点故障不视为安全故障；     

注3：除非在安全概念中表明具有相关性，否则，大于2阶的多点故障可被认为是安全故障。

## Safety Architecture 安全架构

Safety Architecture 安全架构，指用来实现安全要求的一系列要素以及它们之间的交互。

## Safety Measure 安全措施

Safety Measure 安全措施，指用来避免或控制系统性失效，探测或控制随机硬件失效，或减轻它们有害影响的活动或技术解决方案；

注：安全措施包括安全机制；

示例：FMEA 或未使用全局变量的软件。

## Safety Mechanism 安全机制

Safety Mechanism 安全机制，指为了保持预期功能或者达到/保持某种安全状态，由电气/电子系统的功能/要素或者其他技术来实施的技术解决方案，以探测并减轻/容许故障、或者控制/避免失效。
注1：在相关项中实施安全机制以避免故障导致单点失效和防止故障成为潜伏故障；
注2：安全机制也可是：

- a)能够使相关项过渡到或保持在安全状态；
-  b)如同在功能安全概念中定义的，能够向驾驶员发出提醒以控制失效的影响。 

## Safety-Related Element  安全相关要素

Safety-Related Element 安全相关要素，指有潜在可能导致违背安全目标或有助于实现安全目标的要素；
注：如果失效-安全要素可能违背至少一个安全目标，那么该失效-安全要素被认为是与安全相关的。

## Safety-Related Function 安全相关功能

Safety-Related Function 安全相关功能，指有潜在可能导致违背安全目标或有助于实现安全目标的功能；

## Safety-Related Incident 安全相关事件

Safety-Related Incident 安全相关事件，提安全相关失效的发生。

## Safety-Related Special Characteristic 安全相关的特殊特性

Safety-Related Special Characteristic 安全相关的特殊特性，指相关项、 要素自身或其生产过程的特性，这些特性的合理可预见偏差可能影响、促使或造成任何潜在的功能安全降低；
注1：安全相关的特殊特性在相关项或要素的开发阶段中得出；
注2：安全相关的特殊特性不同于安全机制，也不宜和安全机制混淆；
示例：温度范围、有效期限、紧固力矩、生产公差、配置。

## Safety Validation 安全确认

Safety Validation 安全确认，指基于检查和测试，确保安全目标是充分的，并已达到且具有足够的完整性等级。
注：ISO 26262 Part-4 提供了合适的安全确认方法。





## Item 相关项

实现车辆层面功能或部分功能的系统或系统组。

system or combination of systems, to which ISO 26262 is applied, that implements a function or part of a function at the vehicle level.
Note 1 to entry: See vehicle function .

至于 item 和 element 的区别请查看Part 1的术语，功能安全很注重术语，举个例子（如何区分 confirmation/verification/audit/assessment/qualification/validation），所以真正想把功能安全理解透，多看看标准很有裨益。

## Element 要素

系统、组件（硬件、软件）、硬件元器件或软件单元。

system, components(hardware or software), hardware parts, or software units.
Note 1 to entry: When “software element” or “hardware element” is used, this phrase denotes an element of software only or an element of hardware only, respectively.
Note 2 to entry: An element may also be a SEooC.





## SEooC 独立于环境的安全要素 Safety Element Out Of Context

在我们的功能安全开发中一般会有两种方式：

- 一是由OEM自顶向下的分解需求，分配FSR给各个子部件进行开发，这种开发目标有清晰明确的上下文，这种开发就是 “item development”。
- 还有另外的一种开发方式 SEOOC（Safety Elements out of Context）,就是讲没有上下文的开发，这种开发方式一般是具体项目无关的团队进行开发的方式。
  - 不会受限制于某个具体的项目，因此这种开发方式我们不能称之为 item，只能称为 element，当然有很多细节就会不同了。
  - SEooC 是与安全相关的要素，它不是为了一个特定相关项（Item）而开发的。这意味着它不是在一个特定车辆环境中开发出来的；
  - SEooC 可以是系统，系统组合，子系统，软件组件，硬件组件或者零部件；
  - SEooC 是基于假设开发的，假设了一个既定的功能以及包含外部接口的使用环境，主要就是定义我们开发的这个要素（Element）运行在什么样的环境中，有什么功能，以及对外部接口的要求。 
  - 示例：可集成到不同 OEM 系统中的基于假设安全要求的通用雨刮系统。 
  - 基于 SEooC 的 开发的范围可大可小，比如说开发一个 system，subsystem, component.大到一个ECU，一个单板，一个MCU，小到一个中间件，一个AUTOSAR组件等等。
  - 当然现在汽车嵌入式市场上，包括底层软件、芯片，无一不是按照 SEooC 开发的，我们产品工程师在使用的时候，不仅仅去看五花八门的安全机制，一定要分析SEooC assumptions和item details之间的差别。
  - 





## Baseline 基线

基线，指已批准的可作为变更基础的一组单一或多个工作成果、 相关项或要素的版本；
基线通常置于配置管理之下。在生命周期中，通过变更管理流程，基线被用作进一步开发的基础。
基线库的管理包括：基线的创建、基线标识、基线比较、基线控制和基线查询等。



## Branch Coverage 分支覆盖率 

Branch Coverage 分支覆盖率，指在测试中，已执行计算机程序的控制流分支所占的比率；
注1：100%分支覆盖率意味着100%语句覆盖率；
注2：一个if语句总有两个分支，即条件为true和条件为false，不依赖于else语句是否存在。





## Assessment 评估

对相关项或要素的特性是否实现标准目标的检查。

## Audit 审核

针对过程目标对已实施过程的检查。

Audit 和 Assessment 的区别：

- Audit 针对流程
- Accessment 针对产品



## walk-through 走查

systematic examination of work products in order to detect safety anomalies.
Note 1 to entry: Walk-through is a means of verification.	
Note 2 to entry: Walk-through differs from testing in that it does not normally involve the operation of the associated item or element.	
Note 3 to entry: Any anomalies that are detected are usually addressed by rework, followed by a walk-through of the reworked work products .	
	
EXAMPLE	
	During a walk-through, the developer explains the work product  step-by-step to one or more reviewers. 
	The objective is to create a common understanding of the work product and to identify any safety anomalies within the work product. 
	Both inspections  and walk-throughs are types of peer review, where a walk-through is a less stringent form of peer review than an inspection.

## Verification 验证

验证：上下文之间的验证，例如，完成架构之后，需要验证  目前的架构，是否满足需求（覆盖所有需求）

## Validation 确认

验证（verification）和确认（validation）

- 确认阶段，一般是在Item级别（整车），即大V
- 如果没有Item，没有大V，只有软件小V  或硬件小V，则“验证”和“确认”可能是一样的。
- 认证评审（CR，由第三方来做）/验证评审（VR，由公司自己来做）

## CR  认可评审 Confirmation Review

认可评审，指确认工作成果能够提供充分且具有说服力的证据，证明其促成了考虑标准相关目的和要求的功能安全的实现。
注1：功能安全标准提供了一份完整的认可评审清单。
注2：认可评审的目的是确保符合功能安全标准。



## Confirmation Measure 认可措施

Confirmation Measure 认可措施，指与功能安全相关的认可评审、审核或评估。



## ■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■

## Architecture 架构

相关项或要素的结构的表征，用于识别结构模块及其边界和接口，并包括将要求分配给结构模块。

注意：软件的架构设计即需要实现软件安全需求，也需要同时实现软件的非安全性需求。

## Availability 可用性

在定义的生命周期内，产品在给定条件下按照要求提供规定功能的能力。

## BFR 基础失效率 Base Failure Rate

在给定用例中作为安全分析输入的硬件要素失效率。

## Base Vehicle 基础车辆

在安装车辆上装设备之前，原始设备制造商（OEM）的T&B车辆配置。
注：车辆上装设备可安装在包括所有驾驶相关系统（发动机、传动系、底盘、转向、制动、驾驶室和驾驶员信息）的基础车辆上。
示例： 带有动力系统和驾驶室的卡车底盘、带动力系统的滚动底盘。

## BB 车辆上装制造商 Body Builder

将卡车、 客车、 挂车和半挂车（T&B）的车身、货运工具或设备增加到基础车辆上的组织。
注1：T&B车身包括卡车驾驶室、 客车车身、步入式车厢等。
注2：货运工具包括货箱、平板床、汽车运输架等。
注3：设备包括作业设备和机械，如水泥搅拌机、倾卸床、雪铲、升降机等。 

## Body Builder Equipment 车辆上装设备

安装在T&B基础车辆上的机械、车身或货运工具。

## Calibration Data 标定数据

Calibration Data 标定数据，在开发过程中，软件构建后将用作软件参数值的数据。
示例： 参数（例如，低怠速值、发动机万有特性图）、车辆特定参数（适应值，例如，节气门限位）、变量编码（例如，国家代码、左舵/右舵）。
注：标定数据不包含可执行代码或注释代码。

## Candidate 候选项

与已经发布并在运行的相关项或要素的定义和使用条件相同、或具有高度通用性的相关项或要素。
注：该定义适用于在用证明中使用的候选项。

## CCB 变更控制委员会 Change Control Board 



## CR  变更需求 Change Request 

## PM 项目经理 Project Manager

1.计划项目的所有活动，并在项目计划中记录计划的项目活动；
2.指导项目中的项目活动；
3.维护和跟踪项目项目计划的进度；
4.验证该组织是否已为功能安全活动提供了所需的资源。

## SM 安全经理 Safety Manager 

Safety Manager 安全经理，指对实现功能安全所必需的活动，负责监督和确保其开展的人员或组织；
注：在相关项开发的不同层面，每个涉及的公司可按照内部矩阵组织对任务的划分，指派一个或多个不同人员。

1.规划项目安全生命周期中的所有安全活动，并将计划的安全活动记录在安全计划中；
2.指导项目中的安全相关活动；
3.维护并跟踪项目安全计划的进度；
4.与客户和供应商实现功能安全；
5.准备和维护安全状态。

## CM  配置经理 Configuration Manager

1.负责项目的配置管理；
2.配置管理环境的创建；
3.配置库的建立和管理；
4.配置状态统计及发布。

## CM 配置管理（Configuration Management）

https://baike.baidu.com/item/%E9%85%8D%E7%BD%AE%E7%AE%A1%E7%90%86/10090499
配置管理（Configuration Management，CM）是通过技术或行政手段对软件产品及其开发过程和生命周期进行控制、规范的一系列措施。配置管理的目标是记录软件产品的演化过程，确保软件开发者在软件生命周期中各个阶段都能得到精确的产品配置。

配置管理：主要针对 软件开发： 本指南适用于内部软件项目所涉及的配置管理。
配置管理 主要参考：《SWEBOK 》软件工程  配置管理部分  和 Apsice。

功能安全管理流程可以从配置管理开始，配置管理的目的是保证对安全工作产物以及开发这些产物的原则、适用条件进行唯一标识，并且在任何时候能可控地对其复现。配置管理另一个重要的目的是在多次迭代开发之后，能保证当前版本与历史版本的互相追溯。



配置管理的实现不仅仅需要对开发产物的管控，开发活动中的人员、权限、开发环境和分工合作等，都会对最终产物产生影响。因此，良好的配置管理不能单纯寄希望于项目参与人员和管理人员。随着开发活动的深入，开发工作的细分会迅速增加，仅靠人力管理无法保证全面覆盖。



从项目成立开始，我们就需要相应的专业工具进行配置管理。项目立项后，项目经理负责组建项目团队，而功能安全经理则负责组建安全开发团队。从团队成立那一刻开始，配置管理就需要对项目团队人员构成、不同角色的权限、工作活动的分配、每一阶段工作产物的评审、归档等工作进行管理。这个管理需要贯穿整个开发活动，直至全部开发活动结束。



## Configuration Item 配置项

常用的配置项包括需求规格说明书、设计规格说明书、源代码、测试计划、测试用例、用户手册等相关的工作产品的集合，被认为是一个独立的实体并置于配置控制之下。

## 配置管理系统

配置管理系统用于管理配置项（如GitLab、Git等）的存储库。



## SCM 软件配置管理（Software Configuration Management）

https://baike.baidu.com/item/%E8%BD%AF%E4%BB%B6%E9%85%8D%E7%BD%AE%E7%AE%A1%E7%90%86
软件配置管理（Software Configuration Management，SCM）是一种标识、组织和控制修改的技术。软件配置管理应用于整个软件工程过程。在软件建立时变更是不可避免的，而变更加剧了项目中软件开发者之间的混乱。SCM活动的目标就是为了标识变更、控制变更、确保变更正确实现并向其他有关人员报告变更。从某种角度讲，SCM是一种标识、组织和控制修改的技术，目的是使错误降为最小并最有效地提高生产效率。

软件配置管理（Software Configuration Management），又称软件形态管理、或软件建构管理，简称软件形管（SCM）。界定软件的组成项目，对每个项目的变更进行管控（版本控制），并维护不同项目之间的版本关联，以使软件在开发过程中任一时间的内容都可以被追溯，包括某几个具有重要意义的数个组合。

软件配置管理，贯穿于整个软件生命周期，它为软件研发提供了一套管理办法和活动原则。软件配置管理无论是对于软件企业管理人员还是研发人员都有着重要的意义。软件配置管理可以提炼为三个方面的内容：

- VersionControl-版本控制；
- ChangeControl-变更控制；
- ProcessSupport-过程支持。

关键活动包括：配置项、工作空间管理、版本控制、变更控制、状态报告、配置审计等。



## GitLab

GitLab 是一个用于仓库管理系统的开源项目，使用Git作为代码管理工具，并在此基础上搭建起来的Web服务。

## Git

Git是一个开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目。

## MISRA C 2012

Motor Industry Software Reliability Association  汽车工业软件可靠性联会。位于英国的一个跨国汽车工业协会。    

MISRA C是由汽车产业软件可靠性协会（MISRA）提出的C语言开发标准。其目的是在增进嵌入式系统的安全性及可移植性。





## Guide line 指南

Guide line 是 26262 标准中单独要求的，该系列文档将会规定在功能安全认证项目各个阶段的各种活动该如何进行，达到什么样的要求，有什么样的验收标准。



## MD5

MD5信息摘要算法（英语：MD5 Message-Digest  Algorithm），一种被广泛使用的密码散列函数，可以产生出一个128位（16字节）的散列值（hash value），用于确保信息传输完整一致。

## RASIC 责任矩阵

责任矩阵。以表格形式表示完成工作分解结构中工作细目的个人责任方法。



## Requirement tracking matrix （RTM）需求跟踪矩阵 

需求跟踪矩阵（RTM）是一种主要管理需求变更和验证需求是否得到了实现的有效工具，借助 RTM，可以跟踪每个需求的状态。 

在需求变更、设计变更、代码变更、测试用例变更时，需求跟踪矩阵是经过实践检验的进行变更波及范围影响分析的最有效的工具，如果不借助需求跟踪矩阵，则发生上述变更时，往往会遗漏某些连锁变化。

需求跟踪矩阵（RTM）也是验证需求是否得到了实现的有效工具，借助 RTM，可以跟踪每个需求的状态：是否设计了，是否实现了，是否测试了，是否验证了。 

## Software Unit 软件单元

Software Unit 软件单元，指软件架构中的最低层级且可被独立测试的软件组件。

## Tailor 裁剪 

功能安全的裁剪，分为两种类型、层次的裁剪：

- 公司层面上裁剪：先做公司层面的安全文化，结构搭建，流程认证，（先从公司层面，去做裁剪）
- 具体项目层面上的裁剪： 再做项目层面的流程认证，（再从项目层面，去做裁剪）



## WP 工作成果 Work Product 

一个或多个相关要求得出的文档。文档可以是包含工作成果的完整信息的单个文档，也可以是包含工作成果完整信息的一系列文档。

例如，Template、CheckList  

注意：Process 类的文档，不属于工作成果。

Guideline 指南，属于Process 类文档。





## ■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■

## FTTI 故障容错时间间隔

Fault Tolerant Time Interval；FTTI 在安全机制未被激活情况下，从相关项内部故障发生到可能发生危害事件的最短时间间隔。 

## FMEA

## DFA

## 故障树

## TCL 工具置信度水平

Tool Confidence Level 工具置信度水平。

## ■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■

## Sample 项目

Golden Sample



![XXX](figures/XXX.jpg)



