## 评估诊断：成功迈出敏捷推进的第一步

无论是想做敏捷但不知道怎么去选择方法，还是不管三七二十一直接套用成熟的实践经验，抑或以自己不具备条件为借口犹犹豫豫不敢去做，这些问题反映的都是大家没有做前期的评估诊断，因此不了解自己的现状，不清楚自己的痛点，不知道从哪里下手去推进敏捷。

一定要由了解敏捷，了解业界敏捷实践情况，参加过相关培训的人员负责推进。

### Step 1: 挑选代表性项目

类似抽样：可以是业务上有代表性的，或者研发模式上，以及规模大/中/小上。这样才能更真实地反映企业现状。

### Step 2: 访谈评估

再确定需要评估的项目范围后，需要对项目中的团队成员进行访谈，从流程、组织、人员技能、度量和技术等维度，对项目进行深度评估。这一步的目的是有意识地探查项目的痛点。

### Step 3: 制定转型计划

痛点不同，计划也不同。如果问题是跨部门、跨团队沟通协作不畅，则需要优先考虑团队组织的问题，必要时要做组织变革；如果团队的问题集中在开发完成到上线前这一段，那么计划中就要优先考虑建设DevOps流水线。

### Step 4: 沟通

在正式进行敏捷实践前，需要和相关人比如团队成员、主管，以及推进敏捷的内部负责人等，沟通评估结果和相应计划，以便整个团队达成一致意见。如果不沟通，大家对现状了解不一致，那么在配合上就会有偏差；更严重地，大家互相拆台，这样计划再好也无法落地了。

## 团队试点：让敏捷实践“事半功倍”

试点工作的展开可以分为**试点前的准备**和**试点推进过程**。

### 为什么试点？

敏捷实践毕竟属于一场变革。如果不先在试点试水，就贸然在全局上推广，一旦在推进过程中遇到水土不服等问题，不只阶段性的成果会前功尽弃，想倒回去做新的改变也更不容易，最终整个变革大概率会走向失败。

### 试点前的准备

#### 选择试点团队

有以下特征的团队会成为首选：

- 采纳敏捷的意愿相对强烈
- 业务价值高或者采纳敏捷会在短期内给团队带来很大收益

这样的项目一般比较重要，上下关注度高，团队也会更重视自己的实践活动是否能取得成果。一旦成功，敏捷在公司的影响力会更大。

#### 准备工作细则

##### 组织和人员

要查看当前项目组织结构是否适合做敏捷，如果不适合，要重新组织。对参与试点的人员进行培训。

适合敏捷的组织结构应该是“高内聚，低耦合”的。即全功能小团队内、小团队内部成员间的沟通合作更紧密；而团队之间的沟通协作要远比内部的少。划分组织结构的框架有很多，但本质都是“高内聚，低耦合”。

###### Spotify框架

一个组织结构的通用典范。分两层：

- 下层Squad。指的是一个个全功能小团队，每个团队由自己的业务分析师，开发人员，测试人员和迭代经理（Iteration Manager），能够端到端负责一个需求或者产品。
  - 一般来说，团队人数限制在5-9人。当超过9人时会被拆分成不同Squad。
- Tribe。当Squad超过5个，一般要考虑将这些Squad划分到不同的Tribe中去。

在敏捷中，我们就是按照从Tribe到Squad这样的线条去管理团队的。几个Squad之外设立产品负责人用来把我整个产品。在组织重组完成之后，定义各个角色的描述和职责，并进行宣讲，在团队内达成一致。

###### 敏捷培训

- 进行敏捷思想基础和敏捷实践基础两门基础课程培训
- 组织拆书会，选择一些敏捷基础的书籍，每个人都来读一节，一起来分享，这样团队成员很快就有了一定的敏捷只是储备。

除了对要参加敏捷试点的团队进行培训意外，我们还可以对相关项目的干系人做一些宣讲，例如兄弟公司时如何做敏捷，取得了什么成效等等。以上都是试点启动前的培训，在试点过程中，我们还会根据团队实践情况，针对大家对敏捷认知模糊的部分，随时做出讲解。比如深入讲解需求条目化、怎么做用户故事以及怎么拆分等等。

##### 管控治理规则

在敏捷试点前就跟大家明晰，保证整个试点工作有序进行。比如，架构和设计的治理规则，质量管理策略规则等等。

##### 需求范围

需求是逐渐涌现出来的，但要想顺利开展后续迭代，前期需求的准备必不可少。前期准备：

- 项目的高阶需求范围、高阶发布计划
- 高阶的史诗级故事
- 近期2个迭代要开发的用户故事，要有优先级排序

如何准备好这些用户故事？通常可以开几个工作坊，头脑风暴一下，然后排序。注意用户故事不仅要有故事描述，还要有验收标准。

##### 架构

做好需求就要开始架构。因为敏捷中需求是分步提出来的，相应地，要采用**演进式架构**，可以搜索了解一下“Scott W. Ambler”提出的“*架构预测Architectural Envisioning*”。

思考实现需求的高层设计策略，从技术图表（如UML）、用户交互流程图、领域图和变更流程四个方面建模。

##### 敏捷方法和工具

根据第一步评估诊断时的访谈结果，根据痛点选择适合的敏捷方法。

- 研发作业流程管理工具：Jira、Trello
- 持续集成工具：Jenkins

##### 办公环境设施

物理看板、开放式工位、敏捷宣传海报等等。

### 如何推进敏捷试点

如果说在准备工作中，最重要的是组织和人员的准备，那么在推进试点过程中，关键点就是**打造一支活力与战斗力并存的敏捷团队**。团队是敏捷实践的根基。组建完团队之后，还需要想办法来唤醒、激发团队，让它更有活力和战斗力。做好这一步，无论团队采纳哪种敏捷方法都可以推进得得心应手。

#### 一起制定社会契约

社会契约（Social Contract）是指一个社会里的全体成员为了更好地生活制定的一些基本准则，大家一起遵守。落地社会契约就是团队相互认可、磨合和协作的过程。大家一起制定，一致认可才有充分理由让大家一起执行。

1. 给大家分发贴纸，5分钟静默时间来思考：你认为加强协作、达成团队目标，需要哪些行为准则？一张纸只写一条。
2. 贴在白板上，归类相私贴纸。逐一讨论，无法达成一致的则弃之。
3. 把契约张贴到所有人可见的地方，用以激励和约束。

#### 回顾会议，引导团队的自主性

引导团队自行选择和决定推进顺序会比直接给“命令”更容易获得认可和接受。选择大家都方便的时间并固定下来。前几次可由敏捷教练来引导，等大家对流程都熟悉了就可以由组长来组织了。

会议开始后，先说明会议目的，接着让大家讨论3个问题，5分钟思考，写下：

- 团队工作中做的好的地方？
- 不好的地方？
- 此外，其它疑问？

逐一讨论，好的保持，不好的头脑风暴如何改善。对于有疑问的地方大家也可以互相提问，有些是敏捷教练需要阐释的，有些则是团队成员需要解释的。

注意⚠️：会议是有时间盒的，一般不超过1个半小时。过多问题可以安排专门时间答疑解惑。

可见会议帮助查漏补缺。

#### 成绩墙、错题集与心情曲线，记录团队敏捷的成长

- 团队为了赶进度，省略了部分测试，匆忙上线
- 迭代中间，有业务人员提出新需求，要求加进迭代中，团队成员不顾自己的研发产能，擅自将需求加进迭代中，最后却搞不定

便于总结，吸取教训。往后向其它团队宣讲时也能很快找到素材。

### 规模化推广

#### 规模化推广≠直接复制试点经验

试点中的经验教训也是可以拿来做参考的。此外，试点涉及的主要是团队内部的敏捷，而规模化推广还要涉及团队间的敏捷。因此你要考虑跨多个迭代、多个团队、多个产品的情况下推进计划和安排优先级，更要考虑团队间的依赖、更大规模地沟通协调、多团队版本控制等一系列问题。

#### 规模化推广的正确方法

关于敏捷的规模化推广， 当前有两个主流框架，[SaFe](https://www.scaledagileframework.com/) (Scaled Agile Framework)和[LeSS](https://less.works/zh-CN) （Large Scale Scrum)。但是，不要套用框架，也不要被框架限制。各取可取之处。

- **选择合适的规模化推广策略。**激进式变革还是渐进式改革？结合企业变革的急迫程度、领导支持力度选择团队能够接受的方式。
- **做好敏捷文化铺垫，培养敏捷的中坚力量。**做好必要的全员敏捷基础培训和核心敏捷人员的能力培养。
- **搭建适合敏捷的工作环境，做好必要的工具和自动化准备。**适合敏捷的工位布置，必要的物理看板和各种协同管理工具等。
- **组织级别的敏捷度量以及持续改进。**从效率、质量、成本等方面收集敏捷相关数据，做好组织级别的敏捷，度量，借以持续改进。
- **重视大型团队的敏捷导入与推广。**规模化敏捷的核心。
  - 业务人员参与度低
    - 首先要打造端到端的、从需求到开发到测试到运维到运营的敏捷全生命周期，向业务敏捷靠拢。
    - **定制度。**确立产品负责人，将以项目为中心的管理改为以产品为中心的管理。只有这样才能让业务战略和产品战略合二为一，让整个团队目标一致。
    - **定反馈机制。**在整个产品研发流程中进行数据收集和处理，做到从业务创意和机会捕捉到需求识别，到开发上线，再到业务运营的整体大反馈闭环。为端到端的研发过程提供数据支持，以便后续识别瓶颈，并改进。
  - 跨团队沟通不畅，协作效率低
    - **要建立团队间的敏捷实践，就需要提前安排支持工作。**一个团队需要的支持会被排入对方的工作列表。（避免随叫随到）
    - **建立沟通机制，对齐团队目标。**把“做什么”和“怎么做”两方面对齐后，团队间的沟通就更加有序和高效了。
    - 具体措施
      - 定期的集体计划会议
      - 将团队间的依赖放到看板上
      - 通过Scrum of Scrum来定期沟通进展。
      - 团队间的版本控制
      - 团队间的架构解藕
