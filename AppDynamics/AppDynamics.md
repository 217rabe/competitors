## AppDynamics
分析时间：2018/9/4

分析人：欧旸晖

-----
## 第一章 产品演变

&emsp;&emsp;在这一章主要从AppDynamics的产品功能发展，目标用户及需求，投融资情况和产品定价和对AppDynamics的产品进行产品演变的分析。<br>
### 1.1 产品功能发展

&emsp;&emsp;AppDynamics于2008年4月1日由Bhaskar Sunkara和Jyoti Bansal在加州创建，以投融资时间为主线研究其发展情况，如表1所示。<br>
<center>表1.AppDynamics功能发展情况表</center>

| 融资轮    |  产品既有功能 | 产品功能动向|
| :------: |  :----:  |  :----:  |
| A[^1]   |  | 通过易于使用的事务流监控和深度诊断为高度分布式应用程序提供快速问题解决的能力 |
| B[^2]   |   应用产品的分布式管理  |应用程序的映射（application mapping），事物流监控（transaction flow monitoring），代码级别诊断（code-level diagnostics），云编排（cloud orchestration）|
| C[^3]    |  在前者的基础上支持.net，大数据和Agile的发布跟踪  |对web应用程序的性能管理 |
| D[^4]     | 应用容量管理，扩展，监控，故障排除和用户体验 |应用程序监控服务|
| E[^5]     |  利用java，.net，node.js ，PHP，NoSQL，Native Mobile和web端应用为软件应用程序提供管理|IT运营和业务分析|
| F[^6]     | 复杂环境故障排除及统一监控，集成的应用程序监控 |升级应用程序分析，通过ADQL语言进行数据查询|

### 1.2 目标用户及需求

&emsp;&emsp;通过查阅官方网站，可以将AppDynamics的用户和需求按照用例，用户角色和行业整理为表2。<br>
<center>表2.AppDynamics的目标用户及需求表</center>

| 用例  |  用户角色 | 行业 |
| :------: |  :----:  |  :----:  |
|DevOps<br>微服务(Microservices)<br>云迁移(Cloud Migration)<br>云监控(Cloud Monitoring)<br>持续交付(Continuous Delivery)<br>统一监控(Unified Monitoring)<br>IBM大型机可见性(IBM Mainframe Visibility)|IT运营(IT Operations)<br>应用开发(App Development)<br>首席信息官(CIO)<br>企业主和分析师(Business Owner and Analyst)<br>移动开发人员(Mobile Development)<br>市场总监(CMO)|金融服务(Finacial Services)<br>零售行业(Retail)<br>媒体和娱乐(Media and Entertainment)<br>电子信息(Telecom)<br>保险行业(Insurance)<br>卫生保健行业(Healthcare)<br>政府部门(Government)|

&emsp;&emsp;从表2可以看出AppDynamics的目标用户主要是IT行业的开发者，运维人员以及应用产品架构师等，为各大行业提供代码级别的应用性能管理和监控。以金融行业客户Nasdaq为列[^6],他们主要使用AppDynamics的平台收集数据，查看和了解应用程序的运行状况，快速跟踪事务并诊断问题。他们认为AppDynamics的优势主要在于快速部署和界面化的交易跟踪能力。以下是Nasdaq的企业解决方案技术高级副总裁Heather Abbott对AppDynamics的评价：<br>

>"It’s a tool that offers seamless traceability and a view that bridge both the APM and the Business product usage effectively."----------Heather Abbott, Senior Vice President of Corporate Solutions Technology

### 1.3 投融资情况

&emsp;&emsp;就crunchbase给出的AppDynamics投融资信息主要将2008年到2015年的五轮重要融资进行总结，如表3所示：<br>
<center>表3.AppDynamics的5轮融资表</center>

| 融资轮   | 宣布时间   | 融资金额 | 领投人| 
| :------: |  :----:   | :----:  |  :----:  | :----:  |
| A   | 2008/5/15 |   \$5.5M   | Greylock Partners , Lightspeed Partners |
| B   | 2010/5/3 |   \$11M   | Greylock Partners , Lightspeed Partners | 
| C     |  2012/1/17  |   \$20M   | Kleiner Perkins Caufield , Byers|
| D    |    2013/1/23    |  \$50M  | Greylock Partners, Kleiner Perkins Caufield & Byers, and Lightspeed Venture Partners| 
| E |  2014/7/22  |  \$70M|Battery Ventures, ClearBridge Investments and Sands Capital.| 
| F    |   2015/11/30   | \$158M  |General Atlantic and Altimeter Capital| 

### 1.4 产品订价

&emsp;&emsp;通过AppDynamics的官网了解到，在应用性能管理上用户分为三种，即APM Pro，APM Advanced和APM Peak，其中APM Pro可以免费试用15天，APM Advanced和APM Peak的定价需要和其销售联系。在终端用户监控上用户分为两种，即Real User Monitoring Pro和Real User Monitoring Peak，其中Real User Monitoring Pro也支持免费试用15天，Real User Monitoring Peak的售价同样需要和产品销售联系。

## 第二章 技术需求及功能模块

&emsp;&emsp;在这一章将主要从技术需求和功能模块两个部分进行分析。

### 2.1 技术需求

&emsp;&emsp;AppDynamics的产品主要是实现对应用程序代码级别的监控，需要实现应用系统运行可视化，提取相关指标设定健康规则和动态创建报警基线。所以他们的产品在技术上的需求核心是的机器学习算法，通过算法对数据进行抓取、学习和训练来设定基线，然后通过前端技术实现数据的可视化和业务系统的实时监控。

### 2.2 功能模块

&emsp;&emsp;AppDynamics的功能模块如图1所示：<br>

<center><image src = "images/1.png" width = '600'></center>
<center>图1.AppDynamics功能模块图</center>

&emsp;&emsp;AppDynamics的功能模块主要分为五个部分，即应用程序监控模块，基线设定和报警模块，端到端业务可见性模块，应用诊断模块和应用分析模块。下面就这五个模块进行功能分析。<br>

#### 2.2.1 应用程序监控模块

&emsp;&emsp;应用程序监控模块如图2所示：<br>

<center><image src = "images/2.png" width = '600'></center>
<center>图2.AppDynamics应用程序监控模块图</center>

&emsp;&emsp;AppDynamics的应用程序监控模块主要分为两个部分，代理和控制器部分，其中代理部分主要可以通过部署在应用内部的插件或者扩展，用于监视应用程序代码在运行时的行为和性能，支持的语言环境如图2所示。控制器从代理接收指标并向他发送指令，所有的活动性能都通过控制器的UI界面查看。<br>

### 2.2.2 基线设定和报警模块

&emsp;&emsp;基线设定和报警模块如图3所示：<br>

<center><image src = "images/3.png" width = '600'></center>
<center>图3.AppDynamics基线设定和报警模块图</center>

&emsp;&emsp;应用程序模块是AppDynamics属于AppDynamics的智能化功能模块，在这一模块中分为四部分。在监控模块中代理将详细的性能和业务指标发送到控制器，控制器通过机器学习算法为每个指标创建动态的基线。AppDynamics通过基线来标记应用程序的正常行为，当性能偏离基线的时候，AppDynamics向工作人员发送异常报告。健康规则是通过基线建立的性能阈值，当超过阈值时会触发对应的事件，触发的事件由相应的策略决定。性能指标主要分为四种性能：严重，警告，正常和未知。当应用的状况发生改变时控制器UI界面会发出警报。

### 2.2.3 端到端业务可见性模块

&emsp;&emsp;端到端业务可见性模块如图4所示：<br>

<center><image src = "images/4.png" width = '600'></center>
<center>图3.AppDynamics基线设定和报警模块图</center>

&emsp;&emsp;端到端业务可见性模块主要分为两个部分，即拓扑图和业务追踪。AppDynamics自动发现业务交易，并以拓扑图的形式显示整个交易的流程，如图5所示，显示应用环境的层，节点，消息队列和数据库，突出显示流经他们的业务，为业务创建基线的时候，基线由拓扑图中红色，黄色和绿色表示。<br>

<center><image src = "images/5.jpg" width = '600'></center>
<center>图5.AppDynamics拓扑图</center>

&emsp;&emsp;业务追踪展现业务所必需的服务，这些服务被调用来实现用户发起的请求。如图6所示，在进行搜索，向购物车添加内容或者推出登陆时需要调用各种应用程序，web服务，第三方API和数据库，这些都可以从业务追踪中体现。

<center><image src = "images/6.jpg" width = '600'></center>
<center>图6.AppDynamics业务追踪图</center>

### 2.2.4 应用诊断模块

&emsp;&emsp;应用诊断模块如图7所示：<br>

<center><image src = "images/7.png" width = '600'></center>
<center>图7.应用诊断模块图</center>

&emsp;&emsp;AppDynamics应用诊断模块提供深度诊断功能，可以观看生产中的所有内容。如果出现问题，可以立即将根本原因诊断为单独的代码行。检测到性能异常时，AppDynamics会自动捕获事务快照。这包括代码，数据库调用和基础结构指标。在单个窗格中，可以看到应用程序行为与性能之间的关联，从而快速确定问题的根本原因并可视化受影响的事务和用户，如图8所示。<br>

<center><image src = "images/8.gif" width = '600'></center>
<center>图8.AppDynamics应用诊断</center>

### 2.2.5 应用分析模块

&emsp;&emsp;应用分析模块如图9所示：<br>

<center><image src = "images/9.png" width = '600'></center>
<center>图9.应用分析模块图</center>

&emsp;&emsp;应用分析模块主要分为三个部分，交易分析结合应用性能和数据指标来关联业务，提供基于SQL的查询语言来了解性能问题和业务成果的影响。如图10所示：<br>

<center><image src = "images/10.png" width = '600'></center>
<center><image src = "images/10_2.png" width = '600'></center>
<center>图10.AppDynamics交易分析</center>

&emsp;&emsp;日志分析收集，关联和分析机器数据来分析运营绩效的实时洞察性。同样可以通过基于SQL的查询语言进行日志搜索分析，提供可视化仪表盘实现数据可视化，在搜索的基础上通过获取重要的警报来处理数据，如图11所示：<br>

<center><image src = "images/12.png" width = '600'></center>
<center><image src = "images/12_1.png" width = '600'></center>
<center>图11.AppDynamics日志分析</center>


&emsp;&emsp;浏览器移动端分析可以通过集成的浏览器，移动端和自定义的用户数据来跟踪不断变化的用户数据，深入理解用户见解，如图12所示：<br>

<center><image src = "images/11.png" width = '600'></center>
<center><image src = "images/11_2.png" width = '600'></center>
<center>图12.AppDynamics浏览器移动端分析</center>

## 第三章 信息架构

&emsp;&emsp;这一章就AppDynamics信息架构来了解其功能，其页面功能集中在顶部导航栏上，内部架构如图13所示：<br>

<center><image src = "images/13.png" width = '600'></center>
<center>图13.AppDynamics信息框架</center>

&emsp;&emsp;可以发现AppDynamics的信息架构基本与其功能模块所对应。在页面导航部分分为7个标签：<br>
1. Home分为Overview，Unified Monitoring和Getting Started，在Overview里面可以查询历史操作，Unified Monitoring提供移动端和浏览器端用户监控，应用监控，数据库监控和服务器监控的创建接口，Getting Started可以进入入门向导。<br>
2. Applicaton用于创建应用监控场景，支持导入已有应用和创建新的应用<br>
3. User Experience用于创建用户监控，支持移动端，浏览器端和外接设备。<br>
4. Database可以创建数据库监控，支持跳转到报警和提醒功能界面。<br>
5. Servers可以创建服务器监控，和数据库监控相差不大，多一个Service Availability判断服务器的状态及响应时间等。<br>
6. Dashboards&Reports用于查看仪表盘和报表。<br>
7. Alert&Respond用于设置报警机制和报警方式。<br>

## 第四章 UI设计

&emsp;&emsp;这一部分主要基于尼尔森是大交互原则来进行交互设计的分析。

- 原则一：状态可见原则

&emsp;&emsp;图14为AppDynamics的平台界面，可以看到在用户登入界面后通过蓝色当前操作可以提醒用户目前所处的功能界面，通过点击界面标签可以进入相应的功能界面，符合状态可见性原则。

<center><image src = "images/14.jpg" width = '600'></center>
<center>图14.AppDynamics平台界面</center>

- 原则二：环境贴切原则

&emsp;&emsp;AppDynamics作为一款国外应用监控软件，采用英语作为其软件语言，但不支持其他语言切换，对于标签信息的设置属于用户所熟悉的概念，逻辑上也易于理解。

- 原则三：用户可控原则

&emsp;&emsp;AppDynamics在交互设计上没有明显的撤销按钮，这使得用户在进行功能配置时十分不方便，只能通过浏览器的撤回操作进行重新设置，不满足用户可控性原则。

- 原则四：一致性原则

&emsp;&emsp;一致性原则分为结构一致性原则，色彩一致性原则，操作一致性原则，反馈一致性原则和文字一致性原则。<br>
1. 结构一致性原则：AppDynamics的功能页面基本采用由上到下的纵向设计，满足结构一致性原则。<br>
2. 色彩一致性原则：整体采用黑白灰配色，满足色彩一致性原则。<br>
3. 操作一致性原则：AppDynamics的功能页面按照由上到下的结构设计有明确的层级关系，满足操作一致性原则<br>
4. 反馈一致性原则：AppDynamics对于不同应用监控的配置页面流程都相似，满足反馈一致性原则。<br>
5. 文字一致性原则：整个页面都采用英文，满足文字一致性原则。

- 原则五：防错原则

&emsp;&emsp;AppDynamics对具体功能配置时没有明显的防错提示，不满足防错原则。

- 原则六：易取原则

&emsp;&emsp;AppDynamics将其功能组件按照导航标签的方式进行设计，方便用户进行功能选择，满足易取原则。<br>

<center><image src = "images/16.png" width = '400'></center>
<center>图16.AppDynamics导航栏</center>

- 原则七：灵活高效原则

&emsp;&emsp;如图17所示，AppDynamics有设置快速导航栏方便用户快速查看配置状态和进行配置任务的选择，满足灵活高效性原则<br>

<center><image src = "images/17.png" width = '400'></center>
<center>图17.AppDynamics的快速导航栏</center>

- 原则八：优美简约原则

&emsp;&emsp;AppDynamics从配色到页面结构都比较简洁，注重信息显示，不算优美但满足简洁原则。

- 原则九：容错原则

&emsp;&emsp;以PHP代理配置流程为列，在创建应用场景时，若未输入场景名字，AppDynamics的界面会给出错误提示，满足防错原则。<br>

<center><image src = "images/15.png" width = '400'></center>
<center>图18.AppDynamics PHP代理配置</center>

- 原则十：人性化帮助原则

&emsp;&emsp;如图19所示，AppDynamics在进行场景配置时，若是未创建过场景，可以通过按钮进入入门向导，满足人性化帮助原则。<br>

<center><image src = "images/18.png" width = '400'></center>
<center>图19.AppDynamics 场景创建</center>

&emsp;&emsp;综合以上十大原则分析，AppDynamics不满足防错原则，造成用户体验较差。

## 第五章 个人观点

&emsp;&emsp;该部分将基于以上四个部分对Sumo Logic的产品从功能和交互设计上提出个人意见。

### 5.1 产品功能

&emsp;&emsp;在功能设置上，个人认为可以参考基线设定和报警模块对夏洛克产品的报警功能进行设计。

### 5.2 交互设计

&emsp;&emsp;在交互设计上，AppDynamics设置的快速导航栏可以快速查看配置状态，可以进行参考。

## 第六章 附录

[^1]: https://www.appdynamics.com/press-release/appdynamics-secures-55-million-venture-funding-greylock-ventures-and-lightspeed/
[^2]: https://www.appdynamics.com/press-release/appdynamics-raises-11-million-series-b-round/
[^3]: https://www.appdynamics.com/press-release/appdynamics-secures-20-million-in-series-c-financing-led-by-kleiner-perkins-caufield-byers/
[^4]: https://techcrunch.com/2013/01/23/appdynamics-raises-50-million-plans-ipo-for-service-that-manages-how-apps-perform/
[^5]: http://www.pehub.com/2014/07/appdynamics-secures-120-mln-growth-funds/?utm_source=dlvr.it&utm_medium=twitter#
[^6]: https://www.appdynamics.com/appdynamics-closes-158-million-in-growth-financing-to-fuel-platform-and-sales-expansion/

















