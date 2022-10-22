# Multi-channel-deep-learning
## 多通道信息在成像重建和视觉显示中的应用

## 多通道的思想被广泛应用于各种成像系统设计及图像视觉算法中。
如我们今天所熟知的相控阵雷达、合成孔径成像、核磁共振-并行成像、多层螺旋CT、多摄像头智能手机中都广泛地配置或设置了多通道的设计。他们往往具有“以空间换取时间”的内在逻辑，从而实现快速采样或者精确成像的目的。
此外，在后期的信号处理及视觉显示中，多通道的思想也被广泛使用。如我们所熟知的图像去噪近十几年的进步之一在于：在同一噪声水平下，增加尽可能“相似”的像素平均！近些年来被广泛使用的图像块这个建模对象组合起来可以用来进行稀疏、低秩等多种信号处理。

 <div align="center"><img src="https://github.com/yqx7150/Multi-channel-deep-learning/blob/main/1666443591498.png" width = "1300" height = "800">  </div>

## Learning from DAE to DSM
 <div align="center"><img src="https://github.com/yqx7150/Multi-channel-deep-learning/blob/main/1666445214426.png" width = "1300" height = "800">  </div>

  * Highly Undersampled Magnetic Resonance Imaging Reconstruction using Autoencoding Priors  
[<font size=5>**[Paper]**</font>](https://cardiacmr.hms.harvard.edu/files/cardiacmr/files/liu2019.pdf)  [<font size=5>**[Code]**</font>](https://github.com/yqx7150/EDAEPRec)   [<font size=5>**[Slide]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide) [<font size=5>**[数学图像联盟会议交流PPT]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide)

  * High-dimensional Embedding Network Derived Prior for Compressive Sensing MRI Reconstruction  
 [<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/abs/pii/S1361841520300815?via%3Dihub)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/EDMSPRec)
 
  * Denoising Auto-encoding Priors in Undecimated Wavelet Domain for MR Image Reconstruction  
[<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/pii/S0925231221000990) [<font size=5>**[Paper]**</font>](https://arxiv.org/ftp/arxiv/papers/1909/1909.01108.pdf)  [<font size=5>**[Code]**</font>](https://github.com/yqx7150/WDAEPRec)

## Learning from DAE to DSM
 <div align="center"><img src="https://github.com/yqx7150/Multi-channel-deep-learning/blob/main/1666445236837.png" width = "1300" height = "800">  </div>
