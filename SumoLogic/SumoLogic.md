# sumo logic竞品分析报告

分析时间：2018/8/10

分析人：欧旸晖
- - - - - 


## 第一章 产品演变

&emsp;&emsp;在这一章主要从Sumo Logic的产品功能发展，目标用户及需求，投融资情况，产品定价和对Sumo Logic的产品进行产品演变的分析。

### 1.1 产品功能发展

&emsp;&emsp;sumo logic由Kumar Saurabh和Christian Beedgen于2010年在加州创建，以投融资时间为主线研究其产品发展情况，如表1所示。

<center><font size = "2">表1.Sumo Logic产品功能发展情况表</font></center>

| 融资轮    | 宣布时间 | 产品既有功能 | 产品功能动向|融资金额 | 领投人| 资金走向 |
| :------: |  :----:  |  :----:  |:----:  |:----:  |:----:  |:----:  |
| B[^1]   |  2012/1/31|为企业提供基于云服务器的PB级数据分析，通过分析网络日志文件帮助企业用户洞悉运维漏洞  | 下一代日志管理和分析产品的研发 | $15M |Greylock Partners | 技术研究及市场营销 | 
| C[^2] | 2012/11/29 |对大数据的实时查询，分析，监控和可视化操作，使得应用程序和基础设施在数据中心和混合云环境中纠错变为可能 |  | $30M |Accel | 扩大技术研究和销售市场 |
| D[^3][^4]     | 2014/5/20   |企业安全分析&异常监测&应用商店 | 加强其企业安全分析，异常检测和应用商店模块的功能|$300M|Sequoia Capital| 进军欧洲、中东和非洲以及亚太地区, 洞悉潜在市场   | 
| E[^5]     | 2015/6/1  |云端集成 |增大运维和安全分析的客户用例| $80M |DFJ Growth| 提高对大数据的分析量   | 
| F[^6][^7]      |  2017/6/27 |标准化云计算&DevOps&标准化机器学习 |加强应用程序性能管理和扩展对物联网的监控| $75M| Sapphire Ventures| 促进跨界工程，销售和全球运营的业务增长  |

### 1.2 目标用户及需求

&emsp;&emsp;按照官方网站的说法“Our customers rely on Sumo Logic to transform machine data into continuous intelligence”，sumo logic的用户主要是B端企业用户，这些公司通过使用他们的产品对机器数据进行分析，将大数据转化为有用信息。<br>
&emsp;&emsp;Sumo logic主要通过产品功能和行业对其用户进行划分，如表2所示。
<center><font size = "2">表2.sumo logic用户划分</font></center>


| 功能   | 行业  |  
| :------: |  :----:   | 
|安全合规<br />持续交付<br/>监控排错 | 教育<br />能源<br/>金融服务<br />政府<br />医疗<br/>制造业<br/>娱乐媒体<br/>制药业<br/>房地产<br/>电商零售<br/>科技<br/>通信<br/>旅游 |  


&emsp;&emsp;目前，Sumo Logic有1500名付费用户（譬如Zuora、丰田、Airbnb和Delta）和3万名活跃用户，每天分析的数据高达100pb。<br>
&emsp;&emsp;以澳大利亚领先的汽车分类网站carsales[^8]为列，他们使用Sumo Logic的云原生数据分析平台，以实现全栈可见性和对其应用程序状态进行实时观测，这都得益于其简单的日志查询，分类功能，可自定义的仪表板以及报告和警报功能的巨大优势。<br>
&emsp;&emsp;以下是工程总监Michael Ridgway对sumo logic产品的评价：

>Before Sumo Logic we were working blind. Only certain individuals had access to our application logs, which were typically accessed if there was some failure. Now, our entire development team has real-time access and can get instant visibility into what’s going on within our environment at any time.”

&emsp;&emsp;可以看出sumo logic确实在帮助他们实现了网站运营的实效性和高速性。


### 1.3 产品定价

&emsp;&emsp;Sumo Logic的付费用户[^9]定价如表4所示。
<center><font size = "2">表4.Sumo Logic的付费用户</font></center>

<table>
<tr>
<td>地区</td>
<td>Professional</td>
<td>Enterprise</td>
</tr>
<tr>
<td rowspan="3">德国</td>
<td>3GB/天  324$/月</td>
<td>3GB/天  540$/月</td>
</tr>
<tr>
<td>5GB/天  540$/月</td>
<td>5GB/天  900$/月</td>
</tr>
<tr>
<td>10GB/天  1080$/月</td>
<td>10GB/天  1800$/月</td>
</tr>
<tr>
<td rowspan="3">欧洲</td>
<td>3GB/天  297$/月</td>
<td>3GB/天  495$/月</td>
</tr>
<tr>
<td>5GB/天  495$/月</td>
<td>5GB/天  825$/月</td>
</tr>
<tr>
<td>10GB/天  990$/月</td>
<td>10GB/天  1650$/月</td>
</tr>
<tr>
<td rowspan="3">亚太</td>
<td>3GB/天  324$/月</td>
<td>3GB/天  540$/月</td>
</tr>
<tr>
<td>5GB/天  540$/月</td>
<td>5GB/天  900$/月</td>
</tr>
<tr>
<td>10GB/天  1080$/月</td>
<td>10GB/天  1800$/月</td>
</tr>
<tr>
<td rowspan="3">美国</td>
<td>3GB/天  270$/月</td>
<td>3GB/天  450$/月</td>
</tr>
<tr>
<td>5GB/天  450$/月</td>
<td>5GB/天  750$/月</td>
</tr>
<tr>
<td>10GB/天  500$/月</td>
<td>10GB/天  1500$/月</td>
</tr>
<tr>
<td colspan="3">额外1000DPM(data points per minute)的metrics定价为15$/月</td>
</tr>
</table>

&emsp;&emsp;Sumo Logic的账户类型分为四种：free，trail，professional和enterprise。其中付费用户为professional和enterprise，其按照德国，欧洲，亚太和美国四个地区进行定价，按照每日分析数据量进行价格划分。<br>
&emsp;&emsp;可以看出，对德国和亚太两个地区的定价相同，欧洲和美国的定价略有差异，但价格浮动不大。当然对于其他地区，Sumo Logic通过邮件联系的方式给用户提供了人性化定制。<br>


## 第二章 技术需求及功能模块


&emsp;&emsp;在这一章将主要从技术需求和功能模块两个部分进行分析。



###  2.1 技术需求


&emsp;&emsp;Sumo Logic的产品主要是实现对机器数据实现实时分析，将数据可视化，实现网站的智能运维。因此他们的产品在技术上需要的是强大的机器学习算法，聚类算法实现对网络日志的分类，这也是他们产品的核心需求，同时也需要拥有强大的app library供用户选择；在界面交互上需要的是简洁大方且功能分布清晰的页面设计，便于用户操作，特别是在数据可视化的部分，需要支持多类图形显示分析结果。


###  2.2 功能模块

&emsp;&emsp;通过对sumo logic产品的研究，简单将其功能分为三个模块：数据分析查询模块，数据可视化模块以及报警功能模块。以下就这三部分功能进行详细分析。

#### 2.2.1数据分析查询模块（viewing data）

&emsp;&emsp;在数据分析查询模块，用户登录网站后进入search page可以通过输入search query对指定的文件进行分析，也可以通过左侧导航栏Manage Data分类下的collection中的collection对已有的文件进行查看，然后通过install app 可以实现对数据的分析，具体如图1所示。

&emsp;&emsp;数据来源分为两类，一类是local log file，另一类是streaming data，对这两类数据的分析流程不尽相同，具体如图2所示。其中在对local log file的添加上分为两种添加途径，可以通过setup wizard添加，也可以通过left bar的manage data下的collection选项中collection界面的add source选项进行添加。

<center><img src = '../Sumologic/_image/1.png' width = '600'></center>

<center>图1、Sumo Logic数据查询分析模块</center>

<center><img src = '../Sumologic/_image/2.png' width = '300'><img src = '../Sumologic/_image/3.png' width = '300'></center>

<center>图2.sumo logic对两类数据分析来源操作流程</center>


#### 2.2.2 数据可视化模块（data visualization）


&emsp;&emsp;Sumo Logic在数据可视化方面主要采用图表结合的方式进行实现，如图3所示。分为两种情况：<br>
（1）官方模版：用户直接通过left bar下library的overview文件查看其官方提供的dashboard查看Visitor Locations，Traffic Distribution by Server，Traffic Volume and Bytes Served和Responses Over Time等仪表。<br>
（2）自定义：用户可以在search page通过search query的形式对分析结果进行整合，可以将分析结果生成table，bar chart，column chart，line chart，area chart，pie chart和Box Plot chart的形式，再将其添加到dashboard中。<br>
&emsp;&emsp;对于dashboard，sumo logic支持添加文字描述，用户自定义样式和分享给团队的功能。

<center><img src = '../Sumologic/_image/4.png' width = '600'></center>
<center>图3.Sumo Logic数据可视化</center>

&emsp;&emsp;Sumo Logic根据用户加载的app不同会生成不同的仪表盘模版，下面就以Nginx为例，说明官方提供的仪表盘模版。<br>
&emsp;&emsp;在install app成功后会生成五种仪表盘的文件，如图4所示：<br>

<center><img src = '../Sumologic/_image/5.png' width = '300'></center>
<center>图4.Nginx 仪表盘文件目录</center>

 1. Overview文件内容分别显示访问者的位置，跨服务器的流量分布，响应类型随时间的细分以及随时间推移的流量/字节数。
 2. Visitor Access Type提供有关站点访问者环境的信息，包括操作系统/平台，移动设备类型，浏览器，操作系统和操作系统版本。
 3. Visitor Lcation文件提供站点用户地点分布信息。
 4. Visitor Traffic Insight文件提供用户对文件点击数量排行，推荐网页点击排行，文件类型以及热门搜索字词的信息。
 5. Web Server Operation文件提供有关Web服务器活动的信息，包括检测到的机器人和有关错误的信息。

#### 2.2.3报警功能模块（alert）

&emsp;&emsp;在报警功能模块，主要分为两类模式，log alerts和metrics alerts，如图5所示。

<center><img src = '../Sumologic/_image/7.png' width = '600'></center>

<center>图5. Sumo Logic报警功能模块</center>

&emsp;&emsp;设置log alerts主要对需要接受报警信息的search page进行操作，点击save as后选择schedule this search，对报警频率进行设置，最后选择alert type，sumo logic一共提供了五种alert type，分别是为email，script action，servicenow connection，webhook以及save to index，用户可以通过个人需求进行选择。<br>
&emsp;&emsp;设置metrics alerts可以通过两种途径设置，一种是直接打开metrics page通过创建query设置，另一种是通过left bar中manage data的alerts选项下的metrics page页面进行设置。<br>

## 第三章 信息架构

&emsp;&emsp;在这一章主要通过分析其信息架构来了解sumo logic的具体功能情况。就其页面功能分布方面主要集中在left bar和nav bar下，两个bar的具体功能设置如图6所示。<br>

<center><img src = '../Sumologic/_image/8.png' width = '300'><img src = '../Sumologic/_image/9.png' width = '300'></center>

<center>图6. Sumo Logic bar结构设置</center>

&emsp;&emsp;可以看出在nav bar上主要分为三个部分，即home，library和new。在home部分又分为home，learn和certification部分，在home部分可以快速进入search，metrics和live tail三个界面，对新手用户设置了setup wizard入口，同时也可以通过home查看recent page；在library部分可以快速查看文件目录；在learn为用户提供了产品功能学习资料，主要以视频和文档的形式出现；在new部分支持用户快速添加三类界面，即search，metrics和live tail。<br>
left bar部分分类较多：<br>
（1）app catalog主要以分类的形式列出了可供用户选择的app。<br>
（2）manage data部分分为collection，settings和alerts选项，在collection界面用户可以查询已有的collectors和sources，在setting部分可以对一些功能进行设置，在alerts部分主要设置metrics alerts。<br>
（3）administration部分分为account，users and roles以及security，主要支持用户对其账号信息的查询，设置和升级。<br>
（4）help部分主要连接到其官方网站，提供用户对帮助文档的查询。<br>
（5）user page部分，主要分为notification，preferences，sign out和upgrade，用户可以通过preferences进行偏好设置，通过sign out登出账号，以及通过upgrade升级账号。<br>
（6）recent部分用户可以查看近期操作。<br>
（7）favorites部分可以查看被用户star的folders和dashboards。<br>
（8）personal部分主要列出用户创建的个人文件目录。<br>
（9）library部分用户可以通过设置shared content view同时查看个人创建文件和团队分享文件或者设置browse by creator模式查看个人创建文件目录，也即上面提到的personal部分。<br>

&emsp;&emsp;Nav bar和left bar在功能结构上也有一定的联系，同时存在library的入口，同时存在查看recent page的入口。通过分析sumo logic的bar结构可以看出其功能结构设置比较清晰，分类比较明确，在进行数据分析时便于用户操作。<br>
&emsp;&emsp;在导航设计上，整个导航栏设置为可隐藏和展开的形式，如图7所示：<br>

<center><img src = '../Sumologic/_image/10.png' width = '300'><img src = '../Sumologic/_image/11.png' width = '300'></center>

<center>图7. left bar设置</center>

&emsp;&emsp;其中recent，favorite，personal和library横向排列，在下方有固定独立窗口可以查看对应项目详情。在独立窗口下方纵向排列app catalog，manage data，administration，help和personal选项，点击对应选项可在下方展开或隐藏其子目录。

&emsp;&emsp;其nav bar部分设置如图8所示：<br>

<center><img src = '../Sumologic/_image/12.png' width = '600'></center>
<center>图8. nav bar设置</center>

&emsp;&emsp;在左边固定home和library图标，在library设置了一个弹性标签窗口，支持用户对标签进行滑动操作，最多可添加52个标签，在最右边固定了一个new图标，用于快速新建窗口，当鼠标滑过标签时可以对其进行关闭，命名和复制操作。<br>

## 第四章 UI设计

&emsp;&emsp;在这一部分主要通过交互设计来进行分析，主要分为页面布局，色调选取和导航及主要文件icon样式设置进行分析。整体页面如图9所示。

<center><img src = '../Sumologic/_image/13.png' width = '600'></center>

<center>图9. Sumo Logic页面设计</center>

### 4.1页面布局

&emsp;&emsp;在页面布局上主要分为两个大部分，左侧导航栏及右侧内容页，用户点击导航栏选项，在右侧会实现相应页面跳转。

### 4.2 色调选取

&emsp;&emsp;在色调选取上，Sumo Logic的页面设计主要采用黑，白，灰的经典配色。其图标颜色选取上采用橘红，黄色，绿色和紫色调，在按钮，提醒页面和用户当前操作选项上则采用的是与其logo相同的天蓝色。整个页面以冷色调为主，加入暖色调作为点缀，简洁大方而不失设计感。


### 4.3 图标设置

&emsp;&emsp;在导航及主要文件icon样式设置上，如表4所示，按照功能分为15个图标形式，均采用扁平化设计，对于有子选项的分类，其子选项图标会继承其母选项，比较特别的是user page下的preference，sumo logic为其设置了特定图标。


<center>表4.Sumo Logic图标设置</center>

<center><img src = '../Sumologic/_image/14.png' width = '300'></center>

&emsp;&emsp;通过对其UI设计的分析可以看出，Sumo Logic界面简洁，功能入口比较明确方便用户操作。

##	第五章 个人观点

&emsp;&emsp;该部分将基于以上四个部分对Sumo Logic的产品从功能和交互设计上提出个人意见。

### 5.1 产品功能
在功能设置上，提出以下4点意见。<br>

1. 对于用户页可以进行一个功能整合，将left bar的administration页面功能整合到user page里，合并为一个大的用户信息页面，方便用户进行账户信息查询和设置。同时可以将产品定价设置到用户页中，方便用户了解不同等级账号功能和售价。<br>
2. 对于文件夹的管理方面，可以去掉personal的独立选项，直接在library中设置模式切换模式即可。<br>
3. 可以将用户登录和注销账号接口放置在nav bar上，方便用户快速注销或者切换账户。<br>
4. 对于left bar的设置可以添加用户自定义功能，如支持排序和添加删除等功能。<br>

### 5.2 交互设计

&emsp;&emsp;在交互设计上，主要对比两个产品在仪表盘和仪表的设计上提出意见。<br>
&emsp;&emsp;根据尼尔森原则，夏洛克的仪表盘在操作过程中两方面问题：

1. 用户有自由控制权，在操作失误后可返回，但用户体验感较差。
2. 在图形界的展示过程中不满足易读性，难以体现图表的简洁美感。

&emsp;&emsp;下面具体通过对比Sumo Logic和夏洛克的产品在仪表盘的设计，从仪表盘页面和仪表盘图表两个部分进行分析：

- 仪表盘页面

<center><img src = '../Sumologic/_image/15.png' width = '400'></center>
<center><img src = '../Sumologic/_image/16.png' width = '400'></center>

<center>图10 Sumo Logic(上)、夏洛克（下）仪表盘页面</center>

&emsp;&emsp;两个产品的仪表盘页面如图10所示，都主要分为两个区域，即功能按钮区和图表放置区，下面分两个方面就功能按钮区进行详细分析：<br>

（1）功能按钮位置安排<br>

<center><img src = '../Sumologic/_image/17.png' width = '400'></center>

<center>图11.夏洛克仪表盘功能按钮位置改进意见</center>

建议：如图11，建议将时间设置，保存和导出图片的功能接口做成按钮形式并与添加图表和添加过滤控件的按钮放置在同一行。<br>
原因：在功能上这些按钮都属于仪表盘图表编辑功能键，做成按钮的形式放置在同一行比较醒目且便于用户操作。<br>

（2）功能按钮添加<br>

<center><img src = '../Sumologic/_image/18.png' width = '400'></center>

<center>图12.夏洛克仪表盘功能按钮</center>

建议：Sumo Logic功能按钮设置如图12所示，从左到右依次是仪表盘编辑，添加过滤器，分享仪表盘，刷新仪表盘版面和更多操作。借鉴Sumo Logic设置，就优先级而言，建议添加功能按钮的顺序为：编辑按钮>分享仪表盘>刷新仪表盘版面>更多操作。<br>
原因：编辑按钮的添加优先级最高，因为夏洛克现有编辑操作入口为：App应用场景>报表>（在指定报表一行）编辑>编辑面板，需要离开仪表盘版面，如果需要多次操作编辑界面时，用户体验感较差。<br>

- 仪表盘图表

&emsp;&emsp;以下将从图表加载、图表种类、图表界面和图标样式上进行对比分析<br>

- 图表加载

<center><img src = '../Sumologic/_image/19.png' width = '300'><img src = '../Sumologic/_image/20.png' width = '300'></center>


<center>图13.Sumo Logic(左)、夏洛克（右）图表加载效果</center>

两个产品图表加载过程显示如图13，在网络状况良好的情况下对Sumo Logic页面进行刷新时，加载进度显示为顶部进度条和中心加载柱两种形式，进度条在加载到70%左右会一次性展示所有图表信息。<br>
建议：建议将加载提示信息放置在图表的中央区域，可以以百分比的形式显示加载进度且在加载图片的过程中可以不用等到图形完全加载再显示，可以随着加载过程部分显示。<br>
原因：将加载信息置中和以百分比形式提示，可以使用户更加清晰的查看加载进度；分阶段加载图表可以使用户分阶段查看数据。<br>

- 图表种类

<center><img src = '../Sumologic/_image/21.png' width = '300'><img src = '../Sumologic/_image/22.png' width = '300'></center>

<center>图14.Sumo Logic(左)、夏洛克（右）图表种类</center>

从种类上来看，除Sumo Logic提供的箱型图夏洛克中没有以外，其余的类型夏洛克都涵盖了，且在种类上比Sumo Logic全面。<br>
建议：不建议添加箱型图。<br>
原因：箱形图的使用频率低且国内鲜有人知。<br>

-  图表界面

<center><img src = '../Sumologic/_image/23.png' width = '300'><img src = '../Sumologic/_image/24.png' width = '300'></center>

<center>图15.Sumo Logic(左)、夏洛克（右）图表界面</center>

&emsp;&emsp;两个产品的图表页面安排都分为两个部分，即上方标题及功能按钮导航，下方图表展示区。从左到右，Sumo Logic的功能按钮依次表示：回到相应搜索页面，编辑对应图表过滤器以及显示该图标具体信息。<br>
建议：<br>
（1）按钮样式：建议只显示图标不显示文字，在鼠标滑过对应图标时再显示文字说明图标功能。<br>
（2）功能添加：按优先级建议在导航栏添加时间设置>回到相应搜索页面>编辑对应图表过滤器。<br>
原因：
（1）隐藏文字可以使导航栏更加简洁，在后期添加功能按钮的时候使版面显示更加简洁。<br>
（2）添加时间按钮方便用户快速编辑分析数据的时间区域；回到搜索页面的入口在基本配置中存在，将其添加到导航栏方面用户快速操作；添加过滤器方面用户对单个图表进行信息过滤。

- 图表样式

&emsp;&emsp;在该部分主要对Sumo Logic和夏洛克的仪表盘中显示的图表样式进行了对比，分重要图表和次要图表分析。

&emsp;&emsp;重要图表主要为柱状图和折线图，下面就柱状图和折线图进行分析。


- 柱状图

<center><img src = '../Sumologic/_image/25.png' width = '300'><img src = '../Sumologic/_image/26.png' width = '300'></center>

<center>图16.Sumo Logic(左)、夏洛克（右）柱状图</center>

 建议：<br>
（1）图列：在只有一种数据源时建议隐藏图列。<br>
（2）弹窗：在鼠标滑过时只显示一种具体信息弹窗且将弹窗的位置至于柱状图；建议重置弹窗大小和位置，使信息过长时可以换行，且完整显示在该图形区域中。<br>
（3）y轴显示：去掉当前鼠标指示位置y轴显示信息框。<br>
（4）边距：增大图形显示与图标界面边框的边距。<br>
原因：<br>
（1）只有一个数据源时没有隐藏显示数据必要。<br>
（2）弹窗大小固定可以使信息完整显示在该图形区域中，避免信息重叠。<br>
（3）没有必要演示当前鼠标指示位置y轴值。<br>
（4）增大边距可以使图形显示更加美观。<br>
（具体样式参考图17）<br>

<center><img src = '../Sumologic/_image/27.png' width = '300'></center>

<center>图17.Echart数据可视化实验室柱形图示列</center>

- 折线图

<center><img src = '../Sumologic/_image/28.png' width = '300'><img src = '../Sumologic/_image/29.png' width = '300'></center>

<center>图18.Sumo Logic(左)、夏洛克（右）折线图</center>

&emsp;&emsp;两个产品的折线图显示如图18所示。

建议（样式参考图19）：<br>
（1）点：线上点显示为圆形且只在鼠标滑过最值时才显示信息详情窗口。<br>
（2）当前值：当鼠标放置在折线图上的最值点时，将阴影换为虚线的形式；当鼠标放置在折线图上的最值点时，该点动态变大。<br>
（弹窗和边距改进意见同柱形图）<br>
原因：<br>
（1）点以圆形显示更美观且折线图比较关注的是最值信息，所以只需显示最值点信息即可。<br>
（2）将当前点阴影改为线形式更清晰。<br>

<center><img src = '../Sumologic/_image/30.png' width = '600'></center>

<center>图19.Echart数据可视化实验室折线图示列</center>

次要图表为饼图，面积图，雷达图，漏斗图，矩形树图和树形图。<br>

- 饼图

<center><img src = '../Sumologic/_image/31.png' width = '300'><img src = '../Sumologic/_image/32.png' width = '300'></center>

<center>图20.Sumo Logic(左)、夏洛克（右）饼图</center>

建议（样式参考图21）：<br>

（1）排版：将图形与文字说明分离，借鉴Sumo Logic，以色块注释的形式将信息列在图形右边，过长的信息可以隐藏，在鼠标滑过饼图相应位置的时候弹出窗口显示具体信息。<br>
（2）弹窗：建议将具体信息窗口位置固定，在信息过长时进行换行，使图表在仪表盘中显示时能实现每张图表的信息能包容在自己的显示区域中，以防止显示内容重叠。<br>
（3）显示信息：建议显示的信息颜色置为黑色，可以显示百分比信息。<br>
原因：饼图主要用于显示数据百分比信息，所以在默认加载情况下不用显示图块的具体信息。图形与文字分离更有利于观察。<br>

<center><img src = '../Sumologic/_image/33.png' width = '400'></center>

<center>图21.Echart南丁格尔玫瑰图</center>

- 面积图

<center><img src = '../Sumologic/_image/34.png' width = '300'><img src = '../Sumologic/_image/35.png' width = '300'></center>

<center>图22.Sumo Logic(上)、夏洛克（下）面积图</center>

&emsp;&emsp;两个产品的面积图显示如图22所示。面积图实际属于折线图的变种（具体建议参考折线图）。区别在于，面积图在折线与类别数据的水平轴（X轴）之间填充颜色或者纹理，形成一个面表示数据体积。所以面积图主要用于传达趋势的大小。（具体样式可参考图14）<br>

建议：去掉面积图边界的点。<br>
原因：面积图不用标示具体点，主要显示趋势。<br>

<center><img src = '../Sumologic/_image/36.png' width = '400'></center>

<center>图23.Echart面积图</center>

- 雷达图

<center><img src = '../Sumologic/_image/37.png' width = '300'><img src = '../Sumologic/_image/38.png' width = '300'></center>

<center>图24.夏洛克雷达图</center>
&emsp;&emsp;夏洛克雷达图如图24所示。<br>
建议：去掉具体点的显示。（弹窗，边距和弹窗改进意见同柱形图）<br>
原因：雷达图主要用于对具体数据的评估。<br>
（具体样式参考图25）<br>

<center><img src = '../Sumologic/_image/39.png' width = '400'></center>

<center>图25.Echart雷达图</center>

- 漏斗图

<center><img src = '../Sumologic/_image/40.png' width = '400'></center>

<center>图26.夏洛克漏斗图</center>

建议：（弹窗和边距改进意见同柱形图）<br>
（1）显示信息：建议将具体信息隐藏，不要和图形同时出现。<br>
（2）漏斗显示：建议将漏斗的形状放大，不同部分的色块增大。<br>
（3）消息列表：建议将最上边的信息列表纵行排列。<br>
原因：在数据量很大时，默认状态下显示每部分的具体信息会使界面十分混乱。消息列表纵向展示可以在增大可视信息。<br>
（具体样式参考图27）<br>

<center><img src = '../Sumologic/_image/41.png' width = '400'></center>

<center>图27.Echart漏斗图</center>

- 矩形树

<center><img src = '../Sumologic/_image/42.png' width = '400'></center>

<center>图28.夏洛克矩形树图</center>

建议：（弹窗和边距改进意见同柱形图）<br>
（1）按钮：建议更换按钮样式为扁平化，当鼠标滑过按钮时有弹窗提示按钮功能。<br>
（2）信息列表：建议添加以图块和具体信息对应的信息列表并以纵行排列。<br>
（3）图块：建议增大图块之间的间距，所有图块的颜色以一个色系显示。<br>
原因：在数据量较大的情况下，增大图块间距有利于区分不同数据信息，扁平化的按钮设计和一个色系的图块在视觉上显示更好看。<br>

（具体样式参考图29）<br>

<center><img src = '../Sumologic/_image/43.png' width = '400'></center>

<center>图29.Echart矩形树图</center>

-  树形图

<center><img src = '../Sumologic/_image/44.png' width = '400'></center>

<center>图30.夏洛克树形图</center>
建议：<br>
（1）节点：增大节点形状，以实心圆形显示；增大节点间的距离。<br>
（2）当前操作：可以使当前点动态增大或颜色变化，同时跳出弹窗显示具体信息。（具体样式参考图31）<br>

<center><img src = '../Sumologic/_image/45.png' width = '400'></center>

<center>图31.Echart树形图</center>

## 第六章 附录

[^1]: https://www.sumologic.com/press/2012-01-31/sumo-logic-raises-15m-series-b-round-for-next-generation-log-management-and-analytics/
[^2]: https://www.sumologic.com/press/2012-11-28/sumo-logic-raises-30-million-in-series-c-funding-to-help-enterprises-drive-actionable-insights-from-big-data/
[^3]:  https://www.datacenterknowledge.com/archives/2014/05/21/sumo-logic-nets-30-million-global-expansion
[^4]: http://www.marketwired.com/press-release/sumo-logic-partners-with-sequoia-and-raises-30-million-to-expand-globally-1911831.html
[^5]: http://fortune.com/2015/06/01/sumo-logic-80-million-it-operations/
[^6]: https://www.sumologic.com/press/2017-06-27/75-million-funding-round/
[^7]: https://techcrunch.com/2017/06/27/sumo-logic-lands-75-million-series-f-on-the-road-to-ipo/
[^8]: https://www.crunchbase.com/organization/sumo-logic
[^9]: https://www.sumologic.com/customer/






















