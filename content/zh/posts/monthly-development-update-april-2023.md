+++
banner = "/uploads/dev_update_april.png"
hide_front = true
categories = [ "中文" ]
date = 2023-05-05T05:00:00.000Z
description = "2023年4月，**Bee Track**制定了即将发布的Bee客户端蓝图，目的是修复调研中发现的问题。本地存储重写项目已进入测试前的最后阶段，预计将在未来几周开始测试。同时，Bee Track也在制定参与节点获取存储激励时必须满足的条件。"
references_and_footnotes = [ ]
title = "2023年4月月度进展报告"
_template = "post"
slug="monthly-development-update-april-2023-zh"
+++



![](https://blog.ethswarm.org/uploads/dev_update_april.png)

2023年4月，**Bee Track**制定了即将发布的Bee客户端蓝图，目的是修复调研中发现的问题。本地存储重写项目已进入测试前的最后阶段，预计将在未来几周开始测试。同时，Bee Track也在制定参与节点获取存储激励时必须满足的条件。

同期，**Research Track**优化了统计和信息收集功能，并正在完善安全性和多签流程。

**JS Track**发布了[新的Swarm Desktop版本](https://github.com/ethersphere/swarm-desktop/releases)，并正准备发布最新的bee-js 6.0.0版本。

公平数据协议（Fair Data Protocol）堆栈也得到了一些重要修改，包括对[Fairdrive Web应用](https://app.fairdrive.fairdatasociety.org/)的一系列更改，发布了[Fair Portal](https://fairdrive.fairdatasociety.org/apps/fportal)，发布了修复后的[Blossom](https://github.com/fairDataSociety/blossom)浏览器插件，其中包括修复了若干问题、增加了几项新特性。

在社区建设方面，[Bee安装部分](https://docs.ethswarm.org/docs/installation/quick-start)文档更加完善，官方在Swarm博客上还发表了一篇博文，[解释了如何运行一个用于测试和开发的Bee节点](https://blog.ethswarm.org/foundation/2023/build-on-swarm-how-to-run-a-bee-node-for-testing-and-development/)。此外，还有一些悬赏活动正在进行中（点击[这里](https://app.zenhub.com/workspaces/bounties-6305d6269c97be273b00e01a/issues/gh/fairdatasociety/bounties-internal/46)和[这里](https://bounties.gitcoin.co/issue/29842)）。

请您在日历上标记好6月21日，因为那是Swarm基金会将举行为期三天的[Swarm线上峰会](https://summit.ethswarm.org/)的日子。如果您正在使用Swarm为您的项目赋能，请**提交一份材料并以演讲的方式来展示您的成果**。更多详情将在**5月25日Swarm社区在线会议**中揭晓，请务必参与。同时，您可通过观看Daniel A. Nagy在Ethereum Zürich的演讲“[Swarm网络的存储激励机制](https://www.youtube.com/watch?v=MyINf__6e6o)”来了解更多相关信息。

## 项目进展

### Bee进展

- 成功发布了v1.15版本，是针对上周网络健康状况和检索的调研所出的新版本，优化了调研后所发现的一些问题。目前，系统错误率降至0%，高达83%的网络节点已采用了新版本。
- 草拟完成了本地存储重写的最后几个Pull Request，并在相应的环境中进行了测试。为了能够更深入地洞察分析系统行为，建立了一个拥有1000个节点的大规模私有测试环境。
- 确定了节点和存储激励的具体要求。

### 研究进展

- 完善了统计分析和信息整合，包括对跳过轮次和冻结节点原因的分析。
- 存储激励方面的论文已经完成，研究成果已分享给社区Discord渠道和重要合作伙伴。目前我们正在收集并处理社区的相关反馈。
- 针对测试环境和资金提取涉及的逻辑进行第四阶段的测试。
- 完成了对系统安全性和多重签名实现的升级，目前正等待进一步的审核和补充工作。

## JS进展

- [发布了Swarm Desktop v0.21、v0.22和v0.23版本](https://github.com/ethersphere/swarm-desktop/releases)，以确保Bee保持最新版本（当前版本为v1.15.0）。

## 生态进展

### [Fairdrive Web应用](https://app.fairdrive.fairdatasociety.org/)

- 进行了一系列修改与完善，旨在提高运行速度并大幅减少加载时间，这些修改已在fairdrive的[.development.](https://app.fairdrive.dev.fairdatasociety.org/)版本实现，包括：
    - [缓存pod内容列表](https://github.com/fairDataSociety/fairdrive-theapp/pull/306)
    - [出错时清除缓存](https://github.com/fairDataSociety/fairdrive-theapp/issues/311)
    - [为Blossom扩展提供缓存支持](https://github.com/fairDataSociety/fairdrive-theapp/pull/323)

### [Fair Portal](https://github.com/fairDataSociety/fair-portal)

- 发布了[Fair Portal前端](https://https//fairdrive.fairdatasociety.org/apps/fportal)，这是一个使用FDP协议并符合公平数据原则的应用目录。开发者可以向其提交并添加他们的应用。

### [Blossom](https://github.com/fairDataSociety/blossom)

- 发布了[Blossom v0.3.0](https://github.com/fairDataSociety/blossom/compare/blossom-ext-v0.2.3...blossom-ext-v0.3.0)。
    - [修复了序列化问题](https://github.com/fairDataSociety/blossom/issues/130)
    - [修复了全球邮票批次ID的问题](https://github.com/fairDataSociety/blossom/issues/121)
    - [允许加载访问并非来自bzz的链接](https://github.com/fairDataSociety/blossom/pull/122)
    - [修复了库中无效的dappId问题](https://github.com/fairDataSociety/blossom/issues/117)
    - [在readme中添加了有关swarm扩展的额外信息](https://github.com/fairDataSociety/blossom/issues/128)
    - [修复了库，使其与fdp-storage缓存对象兼容](https://github.com/fairDataSociety/blossom/pull/143)

### [FairOS](https://github.com/fairDataSociety/fairOS-dfs)

- [fairOS-cli：支持上传和下载整个文件夹](https://github.com/fairDataSociety/fairOS-dfs/issues/25)
- [更改上传的最小块大小](https://github.com/fairDataSociety/fairOS-dfs/issues/315)
- [修复KVBatch无法为字节索引工作](https://github.com/fairDataSociety/fairOS-dfs/issues/472)
- [更新了feed失败并出现“chunk已经存在”提示信息的问题](https://github.com/fairDataSociety/fairOS-dfs/issues/473)
- [在公共pods上添加文档](https://github.com/fairDataSociety/fairOS-docs/issues/51)

### [Fairdrive桌面应用](https://github.com/fairDataSociety/fairdrive-desktop-app)

- [修复了窗口操作时的异常行为](https://github.com/fairDataSociety/fairdrive-desktop-app/issues/162)

### 已完成的赏金任务

- [使用Blossom访问fdp-storage的Fairdrive PDF查看器](https://bounties.gitcoin.co/issue/29812)
- [将Slate富文本编辑器作为Fairdrive dApp实现](https://bounties.gitcoin.co/issue/29819)
- [Datafund发布了一篇关于Swarm节点运营商收益的博文](https://blog.datafund.net/why-datafund-is-a-swarm-node-operator-and-how-its-paying-off-fd92e9906785)

### 其他进展

- 发表了一篇节点运营商报告：“[Datafund如何成为Swarm节点运营商，以及它是如何得到回报的。拥有数据就是拥有基础设施。](https://blog.datafund.net/why-datafund-is-a-swarm-node-operator-and-how-its-paying-off-fd92e9906785)”
- [Swarmscan](https://swarmscan.io/)更新了节点发现算法，增强了鲁棒性，有助于发现更多活跃节点。

## DevOps进展

- 将[Bee](https://github.com/ethersphere/bee)部署到了主网（v1.14.1）。
- 发布了[Beekeeper](https://github.com/ethersphere/beekeeper)（v0.12.1）。

## DevRel

### Ethereum Zürich

- Swarm基金会创始人Viktor Tron和Daniel A. Nagy做了演讲。可在YouTube上观看Daniel的演讲"[Swarm网络中的存储激励机制](https://www.youtube.com/watch?v=MyINf__6e6o)"。

### 文档更新

- Bee安装部分更新已生效
    - https://docs.ethswarm.org/docs/installation/quick-start
    - https://docs.ethswarm.org/docs/installation/install
- 更新了Docusaurus和节点版本，增加了对LaTeX的支持，更新了相关主题

### 教育

- [Swarm开发：如何运行一个用于测试和开发的Bee节点](https://blog.ethswarm.org/zh/2023/build-on-swarm-how-to-run-a-bee-node-for-testing-and-development-zh/)

### Swarm社区会议

- 4月27日举办了月度线上活动——Swarm社区会议。

### 应用：[Etherjot](https://github.com/Cafe137/etherjot)

- Etherjot让您能够轻松在Swarm上创建博客。在最新版本中，增加了支持导入来自Jekyll或Hugo的博文。

## 近期活动

- Swarm社区会议 - 月度在线活动将于5月25日17:00 CET在[Swarm Foundation Discord](https://discord.com/channels/799027393297514537/801438093927776286)上进行（[添加至日历](https://www.addevent.com/event/yr16580319)）。同时，如果您对Swarm网络和团队有任何问题，欢迎使用[在线表格](https://airtable.com/shrBRyrMkXFsJvLS3)将问题发送给他们，这些问题会在月度在线会议上答复。
- [Swarm线上峰会——论文征集](https://summit.ethswarm.org/) - 请在日历上重点标注**6月21日**，因为届时Swarm基金会将会举办为期三天的Swarm线上峰会。更多详细信息将在5月25日Swarm社区在线会议上公布，请务必参加。

