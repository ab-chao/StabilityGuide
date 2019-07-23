
> 稳定性之于系统，就像健康之于人类，看起来重要不紧急，然而一旦失去，就追悔莫及。

> 稳定性是一切 0 前面的 1。

## 为什么要做这个专栏？
* **让无法解决的问题少一点，让世界的确定性多一点。**
* 打造国内稳定性领域知识库，降低知识获取门槛。

## 专栏建设
* 目标用户：稳定性相关的从业人员、技术决策者、爱好者等。
* 参与形式：欢迎一切有想法或兴趣的同学一起共建，可以自由选择参与内容编写、案例贡献、渠道宣传、社区维护等活动。
* 写作原则：通俗易懂、言之有物，让读者看完之后感觉有所收获（尽量避免介绍公网无法获取的内部产品或工具）。
* 内容格式：Markdown 格式，易于传播、分享与共建。
* 内容管理：文档即代码，通过 Git 管理；代码目录与内容框架目录保持一致。会定期 Review 代码/目录结构。
* 内容编写：建议内容原创或再创作。为了保障文章质量，不建议直接转载。
* 专栏输出：
	* 稳定性系列文章。
	* 稳定性系列课件（含视频与文稿）。
	* 稳定性系列丛书，如《“小白”也能玩转稳定性》
	* 稳定性行业白皮书。
	* 稳定性理论题库。
	* 稳定性实战题库（含可执行 Demo），通过故障模拟构建问题环境，诊断实战。
* 问题列表：所有人有任何问题和建议都可以通过 Issue 的形式提交，专题作者可以优先输出关注高的内容。


## 内容发布
* 发布节奏：每 2 周一个迭代，默认迭代日为周四。
* 发布流程：
	1. 内容创作（个人专属分支）。
	2. 通知管理员安排发布排期。
	3. 管理员组织文档 Review（随机分配给两名项目共建者）。
	4. 反馈修改建议。
	5. 修改完成后提交 MergeRequest。
	6. 主干统一合并发布。
	7. 更新 Release Notes。
	8. 宣传渠道统一分发（包括技术论坛、技术圈子、公众号、云栖社区等）。
	9. 数据运营反馈（文章曝光度、评论数与建议等）。


## 目录提纲
* 目录拆分尽量遵循 MCME 原则（互相独立，完全穷尽）。
* 每个专题尽量保证 3 篇及以上的优质文章。
* 内容目录一定要与代码目录保持结构一致。


## 文档提纲（仅供参考）
* 文档类型
	* 原创，注明作者与创作时间。
	* 转载，取得原作者许可，注明出处，注意许可协议风险。
* 一句话标题，提纲挈领地表达要解决的问题。
	* 标题应该表达的是问题的核心线索，而不是深层次原因。因为用户排查问题时只能看到表象。比如 SQL 慢是表象，没有创建索引是原因。
	* 可以在标题后的第一段做一些补充，对该问题做一个概括性描述，整体结构按照总-分-总模式。
* 问题的现象是什么？
* 问题产生的原因是什么？
	* 如果有前置的背景知识，可以科普一下，让读者更容易理解。
* 怎么去排查，会用到哪些工具？
	* 详细介绍排查思路与路径，最好是小白式操作，事无巨细，能够完美复现。
	* 在本模块可以介绍一些开源或云产品的使用，不要涉及内部产品，另外产品介绍不要带有太明显的主观偏向性。
* 解决后的效果如何？
	* 前后效果对比。
	* 简要的问题复盘总结，文档收尾。
* 推荐阅读/产品链接/公众号/交流群等。


## 加入我们
* 钉钉交流群号：23384706
* [GitHub 项目地址](https://github.com/StabilityMan/StabilityGuide)
* [云栖社区]()
* [GitLab 项目地址](http://gitlab.alibaba-inc.com/eagleeye/StabilityGuide/wikis/home)


## Release Notes
* 待补充。


## 框架目录
### 1. 事前防范
#### 1.1 代码规约
#### 1.2 变更管控
#### 1.3 性能压测
#### 1.4 故障演练
#### 1.5 风险预案 
#### 1.6 限流降级 
#### 1.7 业务隔离 


### 2. 事中“止血”
#### 2.1 监控
#### 2.2 告警
#### 2.3 异常巡检
#### 2.4 流量调度 


### 3. 事后诊断
#### 3.1 主机诊断
##### 3.1.1 CPU 利用率高
##### 3.1.2 Load 高
##### 3.1.3 网络诊断
##### 3.1.4 磁盘诊断


#### 3.2 JVM 诊断 
##### 3.2.1 JVM 内存诊断
###### [系统稳定系——OutOfMemoryError 常见原因及解决方法](docs/diagnosis/jvm/memory/系统稳定性——OutOfMemoryError常见原因及解决方法.md) 
###### StackOverFlowError

##### 3.2.2 线程诊断
###### 线程池满
###### 死锁

##### 3.2.3 GC 诊断
###### 咱们从头到尾说一次Java垃圾回收




#### 3.3 组件诊断
##### 3.3.1 数据库诊断 
##### 3.3.2 缓存诊断
##### 3.3.3 消息诊断
##### 3.3.4 RPC 诊断
###### 系统稳定性 - 使用 Dubbo 的 N 个注意事项
###### [系统稳定系——Dubbo 常见错误及解决方法](docs/diagnosis/plugin/rpc/系统稳定性——Dubbo常见错误及解决方法.md)

#### 3.4 在线诊断 
##### Arthas

#### 3.5 链路追踪 
#### 3.6 RootCause 
