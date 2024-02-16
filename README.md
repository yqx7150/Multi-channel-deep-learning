# Multi-channel-deep-learning
## 多通道信息在成像重建和视觉显示中的应用

# 多通道的思想被广泛应用于各种成像系统设计及图像视觉算法中
## 如我们今天所熟知的相控阵雷达、合成孔径成像、核磁共振-并行成像、多层螺旋CT、多摄像头智能手机中都广泛地配置或设置了多通道的设计。他们往往具有“以空间换取时间”的内在逻辑，从而实现快速采样或者精确成像的目的。    
## 此外，在后期的信号处理及视觉显示中，多通道的思想也被广泛使用。如我们所熟知的图像去噪近十几年的进步之一在于：在同一噪声水平下，增加尽可能“相似”的像素平均！近些年来被广泛使用的图像块这个建模对象组合起来可以用来进行稀疏、低秩等多种信号处理。

 <div align="center"><img src="https://github.com/yqx7150/Multi-channel-deep-learning/blob/main/1666443591498.png" width = "1300" height = "800">  </div>

# 多通道先验信息无监督学习用于成像重建和图像恢复
## 直觉感官和通常的系统设计经验告诉我们，多通道数据所蕴含的信息往往更加丰富。根据这一准则，我们可以利用目前的一些无监督学习工具，先通过无监督学习将更多通道的数据的先验信息“学习好”。然后，利用更多通道数据与待处理数据的关系，设计算法将“学习好”的先验信息用于我们待处理数据的任务中。       
## 目前我们先后使用去噪自编码、扩散生成模型等工具实现这一理念，在磁共振快速成像重建、CT低剂量成像重建、灰度图像恢复等应用中均取得较为出色的效果。   
 <div align="center"><img src="https://github.com/yqx7150/Multi-channel-deep-learning/blob/main/1666445214426.png" width = "1300" height = "800">  </div>

  * Highly Undersampled Magnetic Resonance Imaging Reconstruction using Autoencoding Priors  
[<font size=5>**[Paper]**</font>](https://cardiacmr.hms.harvard.edu/files/cardiacmr/files/liu2019.pdf)  [<font size=5>**[Code]**</font>](https://github.com/yqx7150/EDAEPRec)   [<font size=5>**[Slide]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide) [<font size=5>**[数学图像联盟会议交流PPT]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide)

  * High-dimensional Embedding Network Derived Prior for Compressive Sensing MRI Reconstruction  
 [<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/abs/pii/S1361841520300815?via%3Dihub)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/EDMSPRec)
 
  * Denoising Auto-encoding Priors in Undecimated Wavelet Domain for MR Image Reconstruction  
[<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/pii/S0925231221000990) [<font size=5>**[Paper]**</font>](https://arxiv.org/ftp/arxiv/papers/1909/1909.01108.pdf)  [<font size=5>**[Code]**</font>](https://github.com/yqx7150/WDAEPRec)
   
  * Homotopic Gradients of Generative Density Priors for MR Image Reconstruction  
[<font size=5>**[Paper]**</font>](https://ieeexplore.ieee.org/abstract/document/9435335)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/HGGDP) [<font size=5>**[Slide]**</font>](https://github.com/yqx7150/HGGDP/tree/master/Slide)  

  * Iterative Reconstruction for Low-Dose CT using Deep Gradient Priors of Generative Model  
[<font size=5>**[Paper]**</font>](https://ieeexplore.ieee.org/abstract/document/9703672)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/EASEL)   [<font size=5>**[PPT]**</font>](https://github.com/yqx7150/HGGDP/tree/master/Slide)

  * Multi-Channel and Multi-Model-Based Autoencoding Prior for Grayscale Image Restoration  
[<font size=5>**[Paper]**</font>](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8782831)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/MEDAEP)   [<font size=5>**[Slide]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide)  [<font size=5>**[数学图像联盟会议交流PPT]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide)

# 多通道数据转换以实现信息增强或存储减少
## 通过深度学习等工具，除了可以利用现有的多通道信息外，我们还可以通过深度学习等工具来实现多通道数据先验信息的增强或者多通道数据的通道压缩，达到信息的更高精度获取或者更好更便捷传输。
## 通过可逆网络等工具和变量增加等网络设计改进，我们先后在图像域的多通道数据以及k域多通道数据等数据形式上分别实现了多通道数据先验信息的可逆增强和多通道数据的通道可逆压缩。
 <div align="center"><img src="https://github.com/yqx7150/Multi-channel-deep-learning/blob/main/1666445236837.png" width = "1300" height = "800">  </div>
   
  * Virtual Coil Augmentation for MR Coil Extrapolation via Deep Learning  
[<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/abs/pii/S0730725X22001722)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/VCA)   

  * Variable Augmentation Network for Invertible MR Coil Compression  
[<font size=5>**[Paper]**</font>](https://arxiv.org/abs/2201.07428)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/VAN-ICC)
 
  * Variable Augmented Network for Invertible Modality Synthesis and Fusion   
[<font size=5>**[Paper]**</font>](https://ieeexplore.ieee.org/abstract/document/10070774)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/iVAN)    
  
  * Variable Augmented Network for Invertible Decolorization (基于辅助变量增强的可逆彩色图像灰度化)  
[<font size=5>**[Paper]**</font>](https://jeit.ac.cn/cn/article/doi/10.11999/JEIT221205?viewType=HTML)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/VA-IDN)    

  * Synthetic CT Generation via Invertible Network for All-digital Brain PET Attenuation Correction    
[<font size=5>**[Paper]**</font>](https://arxiv.org/abs/2310.01885)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/PET_AC_sCT)        

  * Variable augmented neural network for decolorization and multi-exposure fusion    
[<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/abs/pii/S1566253517305298)   [<font size=5>**[Code]**</font>](https://github.com/yqx7150/DecolorNet_FusionNet_code)   [<font size=5>**[Slide]**</font>](https://github.com/yqx7150/EDAEPRec/tree/master/Slide)   

