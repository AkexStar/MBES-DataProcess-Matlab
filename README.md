# MBES-DataProcess-Matlab

## 本项目文件构成说明
- [survey.mlx](https://github.com/AkexStar/MBES-DataProcess-Matlab/blob/main/survey.mlx) 核心程序文件，为matlab实时脚本文件，只能用较高版本matlab打开
- [RawData.mat](https://github.com/AkexStar/MBES-DataProcess-Matlab/blob/main/RawData.mat) 原始多波束数据（matlab mat数据文件格式）
- RawData.txt 原始多波束数据（txt文本文件格式）
- [svp.mat](https://github.com/AkexStar/MBES-DataProcess-Matlab/blob/main/svp.mat) 声速剖面数据（matlab mat数据文件格式）
- [svp.txt](https://github.com/AkexStar/MBES-DataProcess-Matlab/blob/main/svp.txt) 声速剖面数据（txt文本文件格式）
- [vessel.mat](https://github.com/AkexStar/MBES-DataProcess-Matlab/blob/main/vessel.mat) 船体坐标系下各仪器设备坐标，包括换能器、GNSS、MRU（matlab mat数据文件格式）
- [vessel.xlsx](https://github.com/AkexStar/MBES-DataProcess-Matlab/blob/main/vessel.xlsx) 船体坐标系下各仪器设备坐标，包括换能器、GNSS、MRU（excel数据文件格式）

## 算法原理

### 基本过程
- 声线跟踪
- 坐标转换（从多波束局部坐标系到地理坐标系）
- 海底点云滤波
- 可以参考这篇微信推送 [笔记丨多波束测深数据简单处理（声线跟踪+坐标转换）](https://mp.weixin.qq.com/s/uopvvRfChe-lT3MKV3yVUg)

### 微信推送目录
**1. 实验要求**

**2. 技术原理**

  2.1. 多波束系统
  
  2.2. 声线跟踪计算
  
（1） Snell法则

（2） 层内常声速跟踪

（3） 层内常梯度声线跟踪
    
  2.3. GNSS高程与Heave数据融合
  
  2.4. 坐标归位转换
  
（1） 求取波束脚印在理想换能器坐标系下坐标  

（2） 求取换能器、GNSS在理想船体坐标系下坐标

（3） 求取波束脚印与GNSS在理想船体坐标系下的坐标差

（4） 求取波束脚印在地理坐标系下的坐标
    
2.5. 结果数据滤波

**3. 实验内容**

  3.1. 数据预处理与准备
  
  3.2. 波束脚印声线跟踪
  
  3.3. 计算波束脚印在地理坐标系下坐标
  
  3.4. 数据滤波与粗差剔除
  
  3.5. 结果点云三维可视化

**4. 实验心得**

## 处理结果预览
![未滤波三维图1](https://user-images.githubusercontent.com/55226358/227261659-98959b37-96f6-40ed-9d5b-66ffb424715d.png)
![滤波后三维图1](https://user-images.githubusercontent.com/55226358/227261774-2df50aac-0577-4888-a7ee-2c448e8ce77e.png)


## 欢迎关注公众号【Akex】
![image](https://user-images.githubusercontent.com/55226358/227260968-d5fe3591-b752-4554-b815-194df4d3bcb2.png)

