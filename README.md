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
* [百度智能云](https://cloud.baidu.com/product/imagerecognition/general)：通用物品和产品识别
1. 识别精准：基于海量数据，利用深度学习技术及高精度算法不断迭代模型，准确率行业领先
2. 稳定高效：算法适应多种场景，具有较好的抗干扰能力，运行稳定，并支持毫秒级的识别响应能力，快速高效
3. 简单易用：支持标准化接口封装，调用简单，只需上传单张图片，即可获取识别结果
* [百度AI开发平台](https://ai.baidu.com/tech/body/num)：人流量统计
1. 算法领先：高精度头肩检测算法，准确率90%以上，静态人数统计不限人数，适应各种人群密集场所
2. 灵活易用：提供稳定易用的在线API、离线SDK、私有化部署包，适配各类终端接入需求
3. 服务稳定：可提供企业级稳定、精确的大流量服务，拥有毫秒级识别响应能力及99.9%的可靠性保障
* [高德开放平台](https://lbs.amap.com/api/webservice/guide/api/trafficstatus/?sug_index=2)
1. 城市级多元异构数据融合：面向城市级的多元异构数据融合能力，包括路网及设施渠化、信号控制、流量采集、视频卡口、公共交通、共享单车、手机信令及互联网数据等
2. 态势评价更全面更准确：通过多元数据融合去重、多层加权等处理有效整合，比对纠偏，并能够预测数据缺失区域，交通态势指标体系计算全面，准确
3. 多维统一的交通指标体系：针对目前交通评价多种角度冲突的问题，统一交通运行状态、交通优化、交通服务水平等评价模型和标准，实现发现问题、分析问题、治理问题、治理效果的全链路评价体系

#### 5.需求列表与人工智能API加值
用户需求|API接口|价值排序
--|:--|:--
随时随地获取一幅画作的信息|通用物体和场景识别API|重要
观展前获取馆内的实时人流量|人流量统计API|重要
前往展馆前查询周边路况|交通态势API|次重要

#### 具体应用场景
1. 8岁的小宇在读一年级，放暑假的时候和妈妈一起逛商场，商场的通道挂着大大的画展广告牌，小宇对广告牌上的画很感兴趣，他指着广告牌上的图案问妈妈那是什么，妈妈一时回答不上来又担心误导孩子，这时候妈妈拿起手机打开Art Platform对着广告牌上的画画进行拍照扫描，得到画作的相关正确信息并告诉孩子；
2. 小宇的妈妈前几天察觉到小宇对画作的兴趣，打算在暑假的休闲时间带上孩子去展馆，但由于孩子身高不高，如果遇到馆内有太多人的情况下则会影响到孩子的观感体验，考虑到错峰观展，妈妈使用Art Platform查看展馆内的实时人流量并推测是否合适带上孩子去观展；
3. 上班族大勋，平时喜欢艺术，周末想自驾去离家较近的展馆，但由于休息日担心路况不好，希望可以节省时间成本到达目的地，他打开Art Platform定位到展馆，并且通过数据反馈得知途经道路的交通态势，并且选择了路况最优的路线
