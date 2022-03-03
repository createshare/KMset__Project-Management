# ISO 26262_Keyword_功能安全标准-关键字



## FS  功能安全  Functional Safety

Functional Safety 功能安全，指不存在由电气/电子系统的功能异常表现引起的危害而导致不合理的风险。

## Functional Safety Concept  功能安全概念

Functional  Safety Concept 功能安全概念，指为了实现安全目标，定义功能安全要求及相关信息，并将要求分配到架构中的要素上，以及定义要素之间的必要交互。

## Functional Safety Requirement  功能安全要求

Functional Safety Requirement  功能安全要求，指定义了独立于具体实现方式的安全行为，或独立于具体实现方式的安全措施，包括安全相关的属性。

注1：功能安全要求可以是由安全相关的电气/电子系统或基于其他技术的安全相关系统所执行的安全要求，目的是通过考虑确定的危害事件，使相关项达到或保持在安全状态。

注2：功能安全要求的定义可独立于产品开发概念阶段中使用的技术。

注3：安全相关的属性包括ASIL等级信息。

## 安全档案

将收集了开发过程中安全活动的工作成果作为证据，证明完整地实现了相关项的安全要求。安全活动

## 安全活动

在安全生命周期的一个或多个子阶段进行的活动。

## Safety Goal 安全目标

Safety Goal，作为整车层面危害分析和风险评估结果的最高层面的安全要求。 

## 安全生命周期

包含了在概念阶段、产品开发、生产、运行、服务和报废期间的主要安全活动。



## SLC 软件生命周期 (Software Life Cycle)

https://baike.baidu.com/item/%E8%BD%AF%E4%BB%B6%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F/861455

https://wiki.mbalib.com/wiki/%E8%BD%AF%E4%BB%B6%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F

软件生命周期(Software Life Cycle,SLC)是软件的产生直到报废或停止使用的生命周期。软件生命周期内有问题定义、可行性分析、总体描述、系统设计、编码、调试和测试、验收与运行、维护升级到废弃等阶段，也有将以上阶段的活动组合在内的迭代阶段，即迭代作为生命周期的阶段。

## Lifecycle 生命周期

生命周期，指相关项从概念到报废的全部阶段，包含了在概念阶段、产品开发、生产、运行、服务和报废期间的主要安全活动。

## Safe State 安全状态

Safe State 安全状态：也就是当前系统的状态是不会造成危害的。 举个例子：如果枪可能发生走火，那么，枪里没有弹药就是一个安全状态。
在系统设计中，故障降级往往是普遍采用的一种方式，但故障降级并不一定就是安全状态。例如，一辆自动驾驶汽车的某一个核心传感器失效，车辆从原本的 80km/h 降至 20km/h 运行，车辆的功能受到了限制，但 20km/h 仍然具备出现汽车事故的可能性。那么，这种状态就并不是一个安全状态。



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
  - 基于 SEooC 的 开发的范围可大可小，比如说开发一个 system，subsystem, component.大到一个ECU，一个单板，一个MCU，小到一个中间件，一个AUTOSAR组件等等。
  - 当然现在汽车嵌入式市场上，包括底层软件、芯片，无一不是按照 SEooC 开发的，我们产品工程师在使用的时候，不仅仅去看五花八门的安全机制，一定要分析SEooC assumptions和item details之间的差别。





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



## CCB 变更控制委员会 Change Control Board 



## CR  变更需求 Change Request 







![XXX](figures/XXX.jpg)



