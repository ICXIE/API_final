# API_final
API课程期末项目
## 价值主张设计
#### 1.加值宣言：互联网时代，信息迅速发展更新，大众对文化底蕴的追求愈加强烈，越来越多的人想挖掘自己的艺术细胞和丰富文化底蕴；当听到一首好听的歌却不知道歌名时，可以打开音乐app听歌识曲，当看到某种植物却不知道到底叫什么时，也可以打开植物app拍照识物；而当看到一副画作时，却不知道该如何通过图片来获取更多信息。因此，一款能够支持随时随地拍照识画的手机app可以解决这个烦恼，同时支持获取某一城市的展馆实时人流量以及周边交通态势，为用户提供更加高效、愉悦的观感体验。
#### 2.核心价值：本产品着眼于满足用户的精神需求，帮助用户在日常生活中了解艺术品或者艺术家的相关背景知识，同时解决用户前往美术馆时的前提需求。
#### 3.用户痛点：
核心价值|用户痛点
--|:--:
高效性|用户想要了解一幅艺术品时往往只能通过搜索名称，使用本产品的拍照识画功能即可将图片内容转化为文本叙述知识
便捷性|观赏一个展览，最怕的就是遇到浏览高峰时间段，使用本产品即可获得馆内人流量的实时动态
简易性|前往一个地点，可以提前获知途经道路的路况，使用本产品可以快速获知交通态势以选择最优路线

#### 4.人工智能概率性
* [百度智能云](https://cloud.baidu.com/product/imagerecognition/general)：通用物体和场景识别
1. 识别精准：基于海量数据，利用深度学习技术及高精度算法不断迭代模型，准确率行业领先
2. 稳定高效：算法适应多种场景，具有较好的抗干扰能力，运行稳定，并支持毫秒级的识别响应能力，快速高效
3. 简单易用：支持标准化接口封装，调用简单，只需上传单张图片，即可获取识别结果
* [百度AI开发平台](https://ai.baidu.com/tech/body/num)：人流量统计
1. 算法领先：高精度头肩检测算法，准确率90%以上，静态人数统计不限人数，适应各种人群密集场所
2. 灵活易用：提供稳定易用的在线API、离线SDK、私有化部署包，适配各类终端接入需求
3. 服务稳定：可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障
* [高德开放平台](https://lbs.amap.com/api/webservice/guide/api/trafficstatus/?sug_index=2)：交通态势
1. 城市级多元异构数据融合：面向城市级的多元异构数据融合能力，包括路网及设施渠化、信号控制、流量采集、视频卡口、公共交通、共享单车、手机信令及互联网数据等
2. 态势评价更全面更准确：通过多元数据融合去重、多层加权等处理有效整合，比对纠偏，并能够预测数据缺失区域，交通态势指标体系计算全面，准确
3. 多维统一的交通指标体系：针对目前交通评价多种角度冲突的问题，统一交通运行状态、交通优化、交通服务水平等评价模型和标准，实现发现问题、分析问题、治理问题、治理效果的全链路评价体系

#### 5.需求列表与人工智能API加值
用户需求|API接口|价值排序|智能加值
--|:--|:--|:--
随时随地获取一幅画作的信息|通用物体和场景识别API|重要|是
观展前获取馆内的实时人流量|人流量统计API|重要|是
前往展馆前查询周边路况|交通态势API|次重要|是

#### 用户分析及应用场景
1. 目标用户群：无特定年龄阶段，一般为18岁以上的学生和上班族，兴趣爱好偏向艺术领域。

2. 用户画像及使用场景
<img src="https://github.com/ICXIE/API_final/blob/master/yonghuhuaxiang1.png?raw=true" width = "400" height = "250" alt="" align=center />
● 场景一：莹莹周末和儿子一起逛商场，商场的通道挂着大大的画展广告牌，儿子对广告牌上的画很感兴趣并指着广告牌上的图案问莹莹那是什么，莹莹一时回答不上来又担心误导孩子，这时候莹莹拿起手机打开Art Platform对着广告牌上的画画进行放大拍照扫描，得到画作的相关正确信息并告诉孩儿子；     
● 场景二：莹莹察觉到儿子对画作的兴趣，打算带上孩子去场馆观展，但由于孩子还小身高不高，如果遇到馆内有太多人的情况下则会影响到孩子的观感体验，为了错峰观展，妈妈使用Art Platform查看展馆内的实时人流量并推测是否适合在当下带孩子去观展；    
<img src="https://github.com/ICXIE/API_final/blob/master/yonghuhuaxiang2.png?raw=true" width = "400" height = "250" alt="" align=center />
● 场景一：上班族天天，平时喜欢艺术，周末想自驾去离家较近的场馆观展，但由于休息日担心路上塞车，希望可以节省时间成本到达目的地，他打开Art Platform定位到展馆，并且通过交通态势反馈得知场馆周边道路的实时路况，最终选择了路况最优的路线。  

## 产品原型
### 产品架构图
![](https://github.com/ICXIE/API_final/blob/master/Art+Platform.png?raw=true)

### 产品流程图（针对智能加值设计）
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%BA%A7%E5%93%81%E6%99%BA%E8%83%BD%E4%BA%A4%E4%BA%92%E6%B5%81%E7%A8%8B%E5%9B%BE.png?raw=true"/>

### 数据流程图
<img src="https://github.com/ICXIE/API_final/blob/master/%E6%95%B0%E6%8D%AE%E6%B5%81%E7%A8%8B%E5%9B%BE.png?raw=true"/>

### 界面及交互设计
![](https://github.com/ICXIE/API_final/blob/master/icon%E5%9B%BE.png?raw=true)
![](https://github.com/ICXIE/API_final/blob/master/%E4%BA%A4%E4%BA%92%E5%8F%8A%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A11.png?raw=true)
#### 打开Art Platform的首页既是画作以瀑布流形式呈现的页面，用户在该页面点击画作图片即可进入画作详情页查看更多信息。
![](https://github.com/ICXIE/API_final/blob/master/%E4%BA%A4%E4%BA%92%E5%8F%8A%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A12.png?raw=true)
#### 首页的顶部标签栏分为"画作"与"场馆"，点击"场馆"即可看到场馆信息列表，场馆推荐以城市为基础，如用户的城市在广州，则陈列广州的场馆信息；用户看到希望了解更多的场馆名称时，即可点击进入场馆详情页，该页面会以热力图的形式呈现场馆的实时人流量（拥挤/稀疏），用户还可以得知场馆周边的实时基本路况（拥挤/稀疏）。
![](https://github.com/ICXIE/API_final/blob/master/%E4%BA%A4%E4%BA%92%E4%B8%8E%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A13.png?raw=true)
#### 首页的底部标签栏分为"首页"、"识图"与"我的"，点击"识图"即可进入拍照识图功能界面，用户还可以选择相册中的图片进行扫描识别。
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%B8%AA%E4%BA%BA%E7%95%8C%E9%9D%A2%E5%9B%BE.png?raw=true" width = "600" height = "1050" alt="" align=center />

### 信息设计
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%BF%A1%E6%81%AF%E8%AE%BE%E8%AE%A11.png?raw=true" width = "600" height = "680" alt="" align=center />
<img src="https://github.com/ICXIE/API_final/blob/master/%E4%BF%A1%E6%81%AF%E8%AE%BE%E8%AE%A12.png?raw=true" width = "600" height = "700" alt="" align=center />

## API使用展示
### 通用物体和场景识别
![](https://github.com/ICXIE/API_final/blob/master/wutiapi.png?raw=true)

### 人流量统计
![](https://github.com/ICXIE/API_final/blob/master/renliuapi.png?raw=true)

### 交通态势
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

