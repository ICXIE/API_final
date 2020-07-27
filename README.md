# API_final
API课程期末项目
## 价值主张设计
#### 1.背景：互联网时代，信息迅速发展更新，大众对文化底蕴的追求愈加强烈，越来越多的人想挖掘自己的艺术细胞和丰富文化底蕴；当听到一首好听的歌却不知道歌名时，可以打开音乐app听歌识曲，当看到某种植物却不知道到底叫什么时，也可以打开植物app拍照识物；而当看到一副画作时，却不知道该如何通过图片来获取更多信息。因此，一款能够支持随时随地拍照识画的手机app可以解决这个烦恼，同时支持获取某一城市的展馆实时人流量以及周边交通态势，为用户提供更加高效、愉悦的观感体验。
#### 2.加值宣言（一句话版本）：本产品着眼于满足用户的不同需求，帮助用户在日常生活中了解更多关于艺术的知识，同时解决用户前往艺术场馆时的前提需求。
#### 3.加值宣言（一分钟版本）：随着生活水平的提高，大众对艺术文化底蕴的追求愈加强烈，Art Platform是一款集知识输出与实时动态为一体的APP。首先，用户使用Art Platform可以随时随地使用拍照识画的功能，当看到一幅喜欢的艺术画作想要了解其背景信息时，本产品即可满足用户的基本需求，当希望用更低的时间成本体验一次极佳的观展时，打开Art Platform，通过即可得知场馆的实时人流密度信息（拥挤/稀疏），还可以得知场馆周边道路的交通态势（拥挤/稀疏），为用户选择是否在某一时间点前往场馆提供前提条件；使用本产品，有助于用户提升观展体验感，并且在日常生活中更加便捷的获取与艺术相关的知识。
#### 4.核心价值： 本产品着眼于满足用户的不同需求，帮助用户在日常生活中了解更多关于艺术的知识，同时解决用户前往艺术场馆时的前提需求。
#### 5.用户痛点：
核心价值|用户痛点
--|:--:
高效性|用户想要了解一幅艺术品时往往只能通过搜索名称获取信息，使用本产品的拍照识画功能即可将图片内容转化为文本内容
便捷性|观赏一个展览，最怕的就是遇到浏览高峰时间段，使用本产品即可获得馆内人流密度实时情况
简易性|前往一个场馆之前可以获知途经道路的路况，使用本产品可以简便的知道场馆周边道路的交通态势以选择最优路线

#### 4.人工智能概率性
* [百度智能云](https://cloud.baidu.com/product/imagerecognition/general)：通用物体和场景识别
1. 识别精准：基于海量数据，利用深度学习技术及高精度算法不断迭代模型，准确率行业领先
2. 稳定高效：算法适应多种场景，具有较好的抗干扰能力，运行稳定，并支持毫秒级的识别响应能力，快速高效
3.简单易用：支持标准化接口封装，调用简单，只需上传单张图片，即可获取识别结果
* [百度AI开发平台](https://ai.baidu.com/tech/body/num):人流量统计
1. 算法领先：高精度头肩检测算法，准确率90%以上，静态人数统计不限人数，适应各种人群密集场所
2. 灵活易用：提供稳定易用的在线API、离线SDK、私有化部署包，适配各类终端接入需求
3. 服务稳定：可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障
* [高德开放平台](https://lbs.amap.com/api/webservice/guide/api/trafficstatus/?sug_index=2)：交通态势
1. 城市级多元异构数据融合：面向城市级的多元异构数据融合能力，包括路网及设施渠化、信号控制、流量采集、视频卡口、公共交通、共享单车、手机信令及互联网数据等
2. 态势评价更全面更准确：通过多元数据融合去重、多层加权等处理有效整合，比对纠偏，并能够预测数据缺失区域，交通态势指标体系计算全面，准确
3.多维统一的交通指标体系：针对当前交通评价各种角度冲突的问题，统一交通运行状态，交通优化，交通服务水平等评价模型和标准，实现发现问题，分析问题，治理问题，治理效果的全氟评价体系


#### 5.需求列表与人工智能API加值
用户需求|API接口|价值排序|智能加值
--|:--|:--|:--
随时随地获取一幅画作的信息|通用物体和场景识别API|重要|是
观展前获取馆内的实时人流量|人流量统计API|重要|是
前往展馆前查询周边路况|交通态势API|次重要|是

#### 用户分析及应用场景
1. 目标用户群：无特定年龄阶段，一般为18岁以上的学生和上班族，兴趣爱好偏向艺术领域。

2. 用户画像及使用情境具体说明
<img src="https://github.com/ICXIE/API_final/blob/master/yonghuhuaxiang1.png?raw=true" width = "400" height = "250" alt="" align=center />
● 场景一：莹莹周末和儿子一起逛商场，商场的通道挂着大大的画展广告牌，儿子对广告牌上的画很感兴趣并指着广告牌上的图案问莹莹那是什么，莹莹一时回答不上来又担心误导孩子，这时候莹莹拿起手机打开Art Platform对着广告牌上的画画进行放大拍照扫描，得到画作的相关正确信息并告诉孩儿子；     
● 场景二：莹莹察觉到儿子对画作的兴趣，打算带上孩子去场馆观展，但由于孩子还小身高不高，如果遇到馆内有太多人的情况下则会影响到孩子的观感体验，为了错峰观展，妈妈使用Art Platform查看展馆内的实时人流量并推测是否适合在当下带孩子去观展；    
<img src="https://github.com/ICXIE/API_final/blob/master/yonghuhuaxiang2.png?raw=true" width = "400" height = "250" alt="" align=center />
● 场景一：上班族天天，平时喜欢艺术，周末想自驾去离家较近的场馆观展，但由于休息日担心路上塞车，希望可以节省时间成本到达目的地，他打开Art Platform定位到展馆，并且通过交通态势反馈得知场馆周边道路的实时路况，最终选择了路况最优的路线。  

#### 利益相关者图
![](https://github.com/ICXIE/API_final/blob/master/%E5%88%A9%E7%9B%8A%E7%9B%B8%E5%85%B3%E8%80%85.png?raw=true)

#### 针对人工智能类型、系统性偏差以及ESG考量的利益相关者分析
对象 | 利/害关系 | 关键API | ESG考量(问题与机会)
--|:--|:--|:--
APP使用群体 | 利 > 害：①拍照识画功能→拍摄的照片会占用用户的设备储存空间，但是同该功能的高效性及商业价值相比，问题显得微不足道；②交通态势功能→需要获取用户的位置信息才得以提供最优的线路，虽然涉及到用户的隐私，但是该功能的技术对生活的简易性及商业价值是高于问题本身的 | 物体识别API、交通态势API | ①物体识别API：虽然仍存在浪费用户的空间容量问题，但该API产品的**系统性偏差小**，可基于海量数据，丰富场景之下仍具有稳定高效的优势；②交通态势API：虽然仍涉及用户隐私，但产品团队致力于保护用户隐私，且该API面向城市级的多元异构数据融合能力，通过多元数据融合去重、多层加权等处理有效整合
API提供者 | 利 > 害：①照片缓存占用空间容量小，足以支持用户调用且等比利润是可持续发展的 | 调用三个API，均具有智能价值 | 存在云空间的损耗难以支撑高额度的调用。但同时该三个API均可提供免费调用额度，有益于增加平台粘性
APP拥有者 |利 > 害：APP下载量可为拥有者获取收益 | 调用三个API，均具有智能价值 | 存在用户量上涨时期超额度调用，需要另外的经济成本，产品的更新迭代需要根据用户反馈重复考量；在环境方面，本产品致力于线上服务，倡导无纸化原则，不存在消耗电子产品产生电子污染的情况；在社会方面，本产品严格保护用户隐私，数据的调用过程是合法且安全的；在治理方面，本产品提供的内容均是标准正确的，不存在虚假信息，并且会过滤不健康内容

## 产品原型
### [原型跳转链接](https://icxie.github.io/API-prototype/Art%20Platform/#g=1&p=%E4%B8%BB%E9%A1%B5)
### 产品架构图
![](https://github.com/ICXIE/API_final/blob/master/Art+Platform.png?raw=true)

### 用户旅程地图（针对智能加值设计）
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%BA%A7%E5%93%81%E6%99%BA%E8%83%BD%E4%BA%A4%E4%BA%92%E6%B5%81%E7%A8%8B%E5%9B%BE.png?raw=true"/>

### 数据流程图
<img src="https://github.com/ICXIE/API_final/blob/master/%E6%95%B0%E6%8D%AE%E6%B5%81%E7%A8%8B%E5%9B%BE.png?raw=true"/>

### 界面及交互设计输入/输出细节
![](https://github.com/ICXIE/API_final/blob/master/icon%E5%9B%BE.png?raw=true)
![](https://github.com/ICXIE/API_final/blob/master/%E4%BA%A4%E4%BA%92%E5%8F%8A%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A11.png?raw=true)
#### 打开Art Platform的首页既是画作以瀑布流形式呈现的页面，用户在该页面点击画作图片即可进入画作详情页查看更多信息。
![](https://github.com/ICXIE/API_final/blob/master/%E4%BA%A4%E4%BA%92%E5%8F%8A%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A12.png?raw=true)
#### 首页的顶部标签栏分为"画作"与"场馆"，点击"场馆"即可看到场馆信息列表，场馆推荐以城市为基础，如用户的城市在广州，则陈列广州的场馆信息；用户看到希望了解更多的场馆名称时，即可点击进入场馆详情页，该页面会以热力图的形式呈现场馆的实时人流量（拥挤/稀疏），用户还可以得知场馆周边的实时基本路况（拥挤/稀疏）。
![](https://github.com/ICXIE/API_final/blob/master/%E4%BA%A4%E4%BA%92%E4%B8%8E%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A13.png?raw=true)
#### 首页的底部标签栏分为"首页"、"识图"与"我的"，点击"识图"即可进入拍照识图功能界面，用户还可以选择相册中的图片进行扫描识别。
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%B8%AA%E4%BA%BA%E7%95%8C%E9%9D%A2%E5%9B%BE.png?raw=true" width = "500" height = "900" alt="" align=center />

### 信息设计(关键智能交互技术细节)
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%BF%A1%E6%81%AF%E8%AE%BE%E8%AE%A11.png?raw=true" width = "600" height = "680" alt="" align=center />
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%BF%A1%E6%81%AF%E8%AE%BE%E8%AE%A12.png?raw=true" width = "600" height = "700" alt="" align=center />

### 基于界面分析产品的可行性及用户可欲性
##### 商业可行性：
* 符合人工智能商业发展趋势，本产品在迭代过程具有可持续发展意义；
* 世界人工智能大会腾讯论坛中提出，人工智能已经成为企业数字化、产业智能化的全新主动力；

##### 市场可行性：
* 2017年，国外已有一款通过扫一扫即可知艺术品背后故事的App**Smartify**，说明市场是有该方面的需求且观念超前的；
* 互联网时代，信息迅速发展更新，大众对文化底蕴的追求愈加强烈，越来越多的人想挖掘自己的艺术细胞和丰富文化底蕴，目标用户无限定年龄人群且适用人群将持续增长；

##### 技术可行性：
* 现阶段已有成熟度极高的API接口可调用参考——百度平台的通用物体与场景识别API及高德地图的交通态势API；
* 现阶段采用的资源产品优势强、服务稳定高效；
* 越来越多的开发团队重视API的发展并投入发展；

##### 用户可欲性：
* 界面交互逻辑简单，用户可轻易上手；
* 随着时代的进步，现代社会关于艺术层面的观念趋于高追求、高质量、高级别的发展趋势，越来越多人希望在日常生活中得以丰富精神境界。


## API使用展示(代码及数据展示加值)
### API调用过程示例
![](https://github.com/ICXIE/API_final/blob/master/API%E8%B0%83%E7%94%A8%E8%BF%87%E7%A8%8B%E7%A4%BA%E4%BE%8B.png?raw=true)
### 图像识别——通用物体和场景识别API
* 接口描述：该请求用于通用物体及场景识别，即对于输入的一张图片（可正常解码，且长宽比适宜），输出图片中的多个物体及场景标签。
* 接口地址：[百度智能云之通用物体和场景识别](https://cloud.baidu.com/product/imagerecognition/general)
* 功能介绍：① 识别物体或场景名称；② 获取百科信息
* 请求方式：POST
* 请求url： https://aip.baidubce.com/rest/2.0/image-classify/v2/advanced_general
* 示例代码
![](https://github.com/ICXIE/API_final/blob/master/wutiapi.png?raw=true)

### 人脸与人体识别——人流量统计API
* 接口描述：对于输入的一张图片（可正常解码，且长宽比适宜），识别和统计图像当中的人体个数（静态统计，不支持追踪和去重）。适用于3米以上的中远距离俯拍，以头部为主要识别目标统计人数，无需正脸、全身照，适应各类人流密集场景（如：机场、车展、景区、广场等）；默认识别整图中的人数，支持指定不规则区域的人数统计，同时可输出渲染图片。
* 接口地址：[百度AI之人流量统计](https://ai.baidu.com/tech/body/num)
* 请求方式：POST
* 请求url：https://aip.baidubce.com/rest/2.0/image-classify/v1/body_num
* 解释说明：该API适用于人流密集的场所，本产品将与场馆协调达成共识以获得其实时监控图像，通过获取数据结果至后台返回给用户以热力图的呈现形式。
* 示例代码
![](https://github.com/ICXIE/API_final/blob/master/renliuapi.png?raw=true)

### web服务API——交通态势
* 功能简介：交通态势信息是由当前时刻和未来某一时刻的交通状况信息构成，目前该功能仅对当前时刻对交通状况（路况）信息进行了透出。
* 请求url：https://restapi.amap.com/v3/traffic/status/rectangle?parameters
* 示例代码
![](https://github.com/ICXIE/API_final/blob/master/jiaotongapi.png?raw=true)

## API使用对比
### 百度智能云平台：https://cloud.baidu.com/product/imagerecognition/general
![](https://github.com/ICXIE/API_final/blob/master/baiduwuti.png?raw=true)
### 阿里云开发平台：https://ai.qq.com/product/face.shtml#multiface
![](https://github.com/ICXIE/API_final/blob/master/aliyunwuti.png?raw=true)
#### 对比总结：与阿里云的图像识别结果相比，百度智能云的通用物体和场景识别之后得出的信息更加全面，识别结果更为准确；百度的通用物体和场景识别中拍照识物功能更符合本项目的需求。

### 百度AI开发平台：https://ai.baidu.com/tech/body/num
![](https://github.com/ICXIE/API_final/blob/master/baidurenlian.png?raw=true)
### 腾讯AI开发平台：https://ai.qq.com/product/face.shtml#multiface
![](https://github.com/ICXIE/API_final/blob/master/tengxunrenlian.png?raw=true)
#### 对比总结：腾讯AI的多人人脸检测api的输出结果为人脸识别列表，此功能要求图像中的人体需有正脸显示才得以被识别，由于输出结果悬殊故不太适用于人流量识别功能中，而百度AI的人流量统计api为高精度头肩检测算法，无需正脸、全身照，适用于人流密集场所，输出结果是人流量的具体数据，与腾讯AI相比结果更加精准。

### 基于数据流程设计分析产品的可行性及用户可欲性
##### Viability（商业可行性）：
* 场馆内部通过对不同展区人流量的对比，可以使管理人员统计各个区域的吸引率和繁忙度，从而对展位进行合理分布，提高用户满意度；
* 能够帮助场馆的管理控制人流，避免因客流过多而造成突发的安全事故；

##### Technical Feasibility（技术可行性）：
* 具有明确的核心价值和满足用户的使用需求；
* 与其他多人检测对比之后，本产品使用的人流量检测技术精准度高，满足用户痛点的使用场景；
* 具有明显产品优势与稳定高效的调用服务，具体可参考上方*人工智能概率性分析；

##### Market Feasibility（市场可行性）：
* 用户需求明显、应用市场广阔，且数据库的调用符合市场大部分行业的发展；
* 用户群体广泛，发展趋势符合当代发展潮流；

##### Desirability（用户可欲性）：
* 用户需求显著，本产品的最小可行性功能满足用户基本需求；
* 用户群体广泛，且可获取的信息量较全面，产品的市场未来需求趋势在逐步增长。

### [20X20 PPT](https://github.com/ICXIE/API_final/blob/master/Art%20Platform.pptx)

## 实践心得
#### 通过本次API期末项目，个人在实践过程有以下几点思考：
* 首先，想清楚比做出来更重要，虽然单凭构想具有局限性，但往往比盲目输出更有价值，明白了在项目实践之前就需要想好为什么做，如何做，然后再实施，并且这个过程可以反复几次；其次了解用户痛点后，可以通过将需求拆分成功能点以确定产品的核心价值，在搜寻痛点的过程还需要把眼光放大，思考这是在什么场景下用户遇到一个什么样问题；本项目的API使用及其优先级是通过前期用户画像及使用场景分析，将用户痛点转换为功能点，通过对比其他同类产品，设计及完善原型，在用户满意度与符合当代可持续发展及向善原则中权衡得出价值主张；
* 本项目能如愿实施，我还要特别感谢百度及高德开放平台的免费资源提供，以下是我使用的智能AI功能调用官方文档链接：
##### [百度智能云之通用物体和场景识别](https://cloud.baidu.com/product/imagerecognition/general)
##### [百度AI开发平台之人流量统计](https://ai.baidu.com/tech/body/num)
##### [高德开放平台之交通态势](https://lbs.amap.com/api/webservice/guide/api/trafficstatus/?sug_index=2)

* 此外，本项目得以完成还参考了往年师姐的作品以及已上线的同领域产品，在一定程度上为我的产品需求文档制作提供帮助，在此向其表示感谢，以下是我参考的作品链接以及相关产品链接：
##### [詹晓燕师姐的作品](https://github.com/xlayal/Art_Gallery_Tour)
##### [Vart](http://www.vart.cc/)
* 最后，还要感谢协作工具，本项目原创图标的制作网站Process On以及Axure原型制作工具：
##### [Process On官网](https://www.processon.com/)
##### [Axure官网](https://www.axure.com/)

### [迭代一最新版本——最新修改为更新实践心得](https://github.com/ICXIE/API_final/commit/444f0c26d2641a4a30dc38545e5ceefb47b1c3b9)
### [迭代二最新版本——主要改善为上传了API调用过程示例图/利益相关者图/更新系统偏差分析/ESG问题分析](https://github.com/ICXIE/API_final/commit/93063bea5d62ba37815d9d27f828a6ccdc5e851d)
### [产品迭代二过程一览](https://github.com/ICXIE/API_final/commits/master)
时间|要点
--|:--:
2020.07.21|增加API调用过程图示与利益相关者图
2020.07.22|更新20X20PPT
2020.07.24|更新系统性偏差分析及ESG问题分析，完善措辞
