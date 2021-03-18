
为了不遗漏作业内容，这里有一份checklist方便同学们快速检阅。
- [ ] fork仓库，和伙伴商讨如何通过github协作/代码规范等
- [ ] 编程实现
  
    - [ ] 功能一，操作爬取的论文列表
    - [ ] 功能二，爬取结果分析展示
    - [ ] 功能三，爬取论文信息(附加功能，实现有附加分)
    - [ ] 其他附加功能
    - [ ] 部署
    - [ ] 发布release版本，发起pull request
- [ ] 撰写博客，在截止之前提交一份博客
    - [ ] 包含作业描述和目录
    - [ ] 核对评分标准

---

上一次结对作业中，大家都和小伙伴完成了原型的设计，那么现在再联合小伙伴动手实现原型中的部分功能吧。因为了解到大家基本都有一定的web基础，本次作业便要求大家采用web技术来实现原型中的功能。


## 一、作业内容

### 1. 基础功能

#### 功能1：对已爬取的论文列表进行操作

- 可对论文列表进行删除；
- 可对论文列表进行查询详细信息（支持模糊查询，查询结果的展示、排序等功能可自行设计）;

#### 功能2：分析已爬取到的论文信息，提取top10个热门领域或热门研究方向

- 形成如关键词图谱之类直观的查看方式，点击某个关键词可展现相关的论文；
- 可对多年间、不同顶会的热词呈现热度走势对比，以**动图**的形式呈现（这里将范畴限定在计算机视觉的三大顶会CVPR、ICCV、ECCV内）



### 2. 附加功能
#### 功能3：获取待爬取论文列表及论文信息爬取

- 支持用户输入单个论文题目，也支持批量导入论文列表；
- 通过论文列表，**爬取**论文的摘要、关键词、原文链接；
	- 数据来源网站：CVPR、ICCV、ECCV
	- 至少爬取三年、三大顶会各300篇论文
	- 可编写爬虫代码实现，也可使用爬虫工具（如八爪鱼）爬取

**此功能为附加功能，实现此功能将获得附加分(详情见评分细则)，如果技术上存在难度，可使用助教提供的数据来完成功能1和功能2**



### 3. 本次项目需要部署到云服务器上，并且在博客中给出链接



### 4. **推荐基于Web来开发**，使用Web框架，如常见的JSP、Servlet、spring系列、flask、php、express等，如果技术存在难度**也可以直接使用纯前端来进行开发**，数据写在代码中，持久化在storage。Web使用的持久化建议持久化在嵌入式数据库中，如sqllite或derby。采用的技术应该具有平台兼容性，不依托于具体的环境。本次作业以实现功能为主要目标，技术考量仅仅占一定的分数。切勿用原型工具生成代码，一经发现直接0分。



### 5. 可以扩展你想扩展的功能，扩展功能会被记入作为附加分（不超过编码部分的15%）。



## 二、编码要求

### 1、github使用

本次作业继续沿用Github，相比寒假作业二考察基础git使用，这一次主要考察Git的合作。

1. Fork下面仓库，然后在根目录中新建一个以**学号1&学号2**（两位结对成员的学号）命名的文件夹，并至少进行20次以上的commit修改，两人至少分别提交10次以上，commit记录应该符合项目实情，如果虚构会被扣去所有分数。仓库目录结构没有硬性要求，但要保证可以依靠此仓库提供的代码来构建项目。
https://github.com/kofyou/PairProject

2. 对于非仓库要求的代码，如编译器生成的项目文件、输出文件、class、jar包、exe等，应该使用.gitignore进行忽略，并确保不会提交到github上。
3. 为自己的仓库编写README.md，内容包括，作业链接、结对学号、项目介绍。
4. 在这次编程合作中学习使用Git分支、Release发布及其他高级功能。建立一条dev分支，让你的队友和你在dev分支上开发，开发结束后再合并到main分支。在基本功能开发完成后发布release包，标注版本为1.0.0，后边完成更多功能可以继续发布新的release包。
5. 在完成项目后，**deadline之前**，请正确发起一个Pull Requet ，并确保自己的代码最终成功签入。（如果成功签入会在原始项目主页看到自己学号为名的文件夹）

### 2、代码规范制定

这一次作业仍然需要编写一份codestyle.md作为代码规范，但是要求该代码规范来自于主流的官方规范或者大公司推荐的规范，并在代码规范顶部标注来源。

### 3、技术和框架

本次作业不限制语言，也不限制库的使用。

## 三、博客撰写要求

1. 给出作业描述和目录。
2. 在开始实现程序之前，在**PSP表格**中记录下你估计将在程序的各个模块的开发上耗费的时间和实际花费的时间，实现程序后在**PSP表格**记录实际花费的时间。
3. 在文章开头给出**Github仓库地址**。
4. 给出项目部署到云服务器后的**访问链接**。
5. 展示你的成品，要求**提供10张以上的图片，或者采用GIF或者视频嵌入的方式**来展示作业要求的功能。
6. **结对讨论过程描述**，即刚开始拿到题目后，和队友怎么讨论，解决问题和查找资料的过程，并提供**两人结对讨论的截图**。。
7. **描述设计实现过程**，给出**功能结构图**。
8. 代码说明。展示出项目**关键代码**，300行左右，并**解释思路**。
9. 阅读《构建之法》第四章的内容，结合在构建之法中学习到的相关内容，结对伙伴分别撰写**结对开发**项目的**心路历程与收获**，并**评价结对队友**。

## 四、作业评分项和评分规则

本次作业总分100分

- 撰写博客 满分25分
  1. 博客排版【10%】：是否采用markdown排版，排版是否整齐，博客是否美观大方
  2. 成品展示【30%】：提供10张以上的图片介绍，或者采用GIF或者视频嵌入的方式展示，展示的效果好，能够通过展示清晰了解主要的功能。
  3. 结对讨论过程描述和设计实现过程【30%】：讨论过程描述不笼统，提供结对讨论截图，未提供结对讨论截图该项扣5分。设计合理，实现过程描述不笼统；提供功能结构图，未提供功能结构图该项扣5分；
  4. 代码说明【10%】：展示出项目关键代码，并解释思路。
  5. git仓库链接、代码规范链接【5%】
  6. 心路历程和收获&评价结对队友【15%】：不笼统，有意义，图文兼备；两个人要写各自的感想和给对方的评价。
- 编码实现 满分75分
  1. 代码规范的制定和遵守【10%】：符合所使用语言的官方规范或者行业规范，代码规范至少攘括寒假作业（2）中所要求的内容。需要严格在编码中执行。
  2. Github commit满足多于20次，要求两人均多于10次，且commit时间合理，使用分支、release、issues、pr等其它功能【15%】
  3. 项目功能完整度【75%】：
     - 1、基础功能

       （1）功能1：对已爬取的论文列表进行操作【30%】

       （2）功能2：分析已爬取到的论文信息，提取top10个热门领域或热门研究方向等统计分析效果展示【35%】

       （3）项目部署到云服务器上【10%】

     - 2、附加功能

       （1）功能3：获取待爬取论文列表及论文信息爬取【附加分：15%】

       （2）扩展功能：扩展**基础功能**以外的功能【附加分：0%~15%】
     - **注：附加功能**+**基础功能**不超过该项总分【75%】
# 附：

1、结对作业只需提交一份
2、国内云服务商域名没备案的话链接请给出IP的，否则过几天链接会因为未备案被封禁
3、若未实现部署到云服务器，则该项0分，并且需与助教协商时间现场演示

# 规则&格式

### 1、为了方便阅读以及助教评分，请大家在博客开头给出博文目录，作为内容的索引

务必包含以下大标题，标题含义相近即可，你可以个性化你自己的标题：
- git仓库链接和代码规范链接
- 成品展示
- 结对讨论过程描述
- 设计实现过程
- 代码说明
- 心路历程和收获
- 评价结对队友

### 2、 为了方便其他学校的老师或者助教了解课程实况，请大家在作业开头添加格式描述：

| 这个作业属于哪个课程 | <班级的链接>             |
| :------------------- | :----------------------- |
| 这个作业要求在哪里   | <作业要求的链接>         |
| 结对学号             | <写上两个结对同学的学号> |
| 这个作业的目标       | <写上具体方面>           |
| 其他参考文献         | ...                      |

### 3、提交规则

- 在deadline前交并完成结对登记，得实际得分 * 100%；
- 补交：在deadline 后两天内提交视为补交，得实际得分 * 50%；
- 缺交：在deadline 之后两天未补交视为博客缺交，分数为0分；
- 作业抄袭：当助教发现两篇博客文字/图片/代码过于相似时，判定两篇博客都为抄袭，分数都为-100%（注意是倒扣！）；
- 伪造提交：虽然作业博客没有完成，但是先提交到作业占位置，判定为伪造提交，分数得0分；

注：提前提交的作业，如果能积极响应助教和老师的反馈并在deadline前做出相应修改，在后续评分时，这些修改完善也会被纳入考量。提早准备好处多~

### 4、注意事项

微信班级群如果发布相关通知也是作业要求一部分，请及时查看群通知；
若需要在微信群填写相关信息，未能在deadline之前完成填写的，扣实际得分的50%；
如对作业存在疑问，请在deadline之前三天在班级群提出；
若助教对作业要求有修改，会在群内公告，请务必查看并按新的要求完善作业；
请及时回复老师或助教的点评并作出相应修改

### 5、疑惑解疑

若有对题意不清或者有不理解的地方，可在该博客下方留言，或者在微信群中直接提问
