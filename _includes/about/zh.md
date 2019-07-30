> 写写代码，做做设计。
> 离开世界之前，一切都是过程。

Hey，我是高鹏飞，多出没于[博客](https://gpfworld.github.io)、[简书](https://www.jianshu.com/u/e8bc608a4a17)、[CSDN](https://blog.csdn.net/GPFYCF521)、[微博](weibo.com/gpfworld)、[知乎](https://www.zhihu.com/people/pengfeigao)、[Github](http://github.com/gpfworld)、等地带，绝招尚在开发中。

职业是视觉算法工程师，目前是北京邮电大学在读研究生（2017.09-2020.07），曾在Aibee、美团实习。

##### My Programming Languages Spectrum

- 熟悉深度学习基本理论、CNN、RNN、主流目标检测算法
- 掌握 C++、Python、linux 开发、图像处理，熟练使用 OpenCV
- 熟悉基本算法和数据结构、Tensorflow、Pytorch、Hadoop、Spark
- 熟悉智能优化算法(GA,PSO,TS,Memetic 等算法)
- 通过 CET6，具备基本的日常交流能力和英文文献阅读能力

##### 项目经验

###### 视觉算法实习生   爱笔(北京)智能科技有限公司（2018.07---2018.10）                 
- 工作简介: 主要是完成多相机时钟校准、同步项目，校准后误差为 20ms 左右(一帧 40ms)。 
- 完成相机电子时钟识别(包括数据采集，模型训练与识别)
- 视频解码时间戳，以及时间的获取
- 相机实际网络环境模拟，模拟相机所处的高网络流量环境
- 多相机时钟误差原因分析，误差校准及时钟同步

###### 百度-西交大·大数据竞赛  2018—商家招牌的分类与检测（前 10%）（2018.04---2018.06）
- 项目概况:根据给定的商标图像，如肯德基、麦当劳等，构建算法模型，进行商标图像分类 
- 数据处理:去均值，图像增强(计算图像平均大小(260*550)，crop5+wrap 原图(200*400))
- 模型训练:VGG16 和 Resnet50，使用 BN、滑动平均模型、Adam 优化算法，模型融合(VGG16,ResNet50，
SENet50,ResNeXt50)采用投票策略，评测准确率达到 0.99

###### ICPR MTWI 2018 挑战赛二:网络图像的文本检测 （前 10%）（2018.02---2018.05）
- 项目概况:合成图像、产品描述、网络广告文本图像中的文本检测。
- 数据处理:制作 VOC 数据集、随机划分训练验证测试集 5:2:3、去均值
- 模型训练:FasterRCNN 的 mAP 为 0.36，改进 FasterRCNN(Anchor:aspect ratios:1.2:1、2.8:1、5.4:1，
scales:3、6、9)提升到 0.47，改用 CTPN 的 F-measure 为 0.62

###### ICPR MTWI 2018 挑战赛三:网络图像的端到端文本检测和识别（前 2%）（2018.02---2018.05）
- 项目概况:合成图像、产品描述、网络广告文本图像中的文本检测和识别
- 数据处理:制作 VOC 数据集、随机划分训练验证测试集 5:2:3、去均值
- 模型训练:文本检测使用 CTPN 和文本识别使用 CRNN 的模型

###### 京东猪脸识别比赛 （290/370（2017.10---2017.11）
- 项目概况:根据给定的 30 类猪的视频，构建算法模型，进行猪的图像分类。 
- 数据处理:视频中抽取图像，随机划分训练验证测试(8:1:1)，去均值、10-crop 
- 模型训练:Inceptionv3 迁移学习，训练全连接层，dropout 防止过拟合，Adam 优化算法，测试集准确
率 94.6%

###### 基于客流数据的公交发车时刻表智能优化研究 国家自然科学基金项目（2018.06---2019.03）
- 项目概况:根据公交客流以及相关数据，设计了结合遗传算法和局部搜索算法的文化基因算法，优化线 路的发车时刻表，使得乘客等车成本和公交运营成本最小。实验表明，优化后的发车时刻表，固定成本 降低 4.5-12.8%，乘客的平均等待时降低了 11.9-37.8%。
- 提出新的评价函数，公交运力差值和乘客等待成本最小; 
- 优化全天、非均匀发车时刻表; 
- 结合问题设计文化基因算法，在解的质量和收敛速度都超越遗传算法; 
- 项目成果:在 GECCO(遗传与演化计算) 投递论文一篇，已录用，待发表。

###### 公交站点间客流推断 国家自然科学基金项目 （2017.03---2018.04）
- 项目概况:该项目是根据公交的 IC 卡刷卡数据、公交线路站点信息进行客流量预测。一开始的想法对 用户分类做用户画像，采用 K 均值聚类的方法试图分析不同类用户可能存在的出行规律，效果不理想。 于是观察用户乘车规律，结合统计概率学方法，得出预测方法如下:(1)基于规则(抽象家和工作站点)针 对规律型乘客的下车站点预测方法(2)基于多线路推断方法(3)基于站点吸引和乘车站距推断方法(4)基于 乘客换乘思想下车站点推断方法。准确率最高达到 80%。 
- 项目成果:已应用于天津、济南、厦门、南京公交客流推断;
- 主要技术:Python Pandas、Numpy、Redis、机器学习。
