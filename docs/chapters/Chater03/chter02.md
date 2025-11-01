# 第03章：池化操作 - 第2部分
## 3.4 池化操作的分类
### 核心内容：每种池化的逻辑、步骤与PPT示例（输入均为4×4矩阵：[[3,6,1,4],[4,7,7,8],[2,2,1,2],[2,4,3,4]]，k=2，s=2）  
| 池化类型               | 具体内容                                                  | 图示文字解释                                           |
|------------------------|--------------------------------------------------------------------------|------------------------------------------------------------------------------|
| 1. 最大池化（Max Pooling） | 定义：将输入矩阵划分为若干矩形区域，每个子区域取最大值；<br>PPT示例：<br>输入4×4矩阵→划分为4个2×2窗口→输出2×2矩阵：[[7,8],[4,4]]；<br>PPT图示：含动态GIF演示过程 |<img width="1623" height="853" alt="image" src="https://github.com/user-attachments/assets/6a361538-2ad8-40b7-bb31-988f5bcbde10" />|
| 2. 平均池化（Average Pooling） | 定义：对局部接受域中所有值求平均值；<br>PPT示例：<br>同上述输入→输出2×2矩阵：[[5,5],[2.5,2.5]] |<img width="1415" height="863" alt="image" src="https://github.com/user-attachments/assets/0adf9873-3834-40a1-8b42-04cb32843d28" />|
| 3. 随机池化（Stochastic Pooling） | 定义（PPT原文）：ICLR2013 Zeiler提出，按Feature Map元素概率随机选择（概率与数值正相关）；<br>计算步骤（PPT原文）：<br>1. 元素÷窗口总和→概率矩阵；<br>2. 按概率随机选方格；<br>3. 池化值为选中方格值；<br>PPT示例：<br>输入4×4→概率矩阵（如窗口1：3→0.15、6→0.30、4→0.20、7→0.35）→输出2×2矩阵：[[5,5],[2.5,2.5]] |<img width="1706" height="864" alt="image" src="https://github.com/user-attachments/assets/dbfd1469-8233-40b1-8316-f130ce8b2333" />|
| 4. 组合池化（Combined Pooling） | 定义（PPT原文）：结合最大池化与均值池化优势，分Add、Cat两种策略；<br>PPT代码片段：<br>def add_avgmax_pool2d(x, output_size=1):<br>  x_avg = F.adaptive_avg_pool2d(x, output_size)<br>  x_max = F.adaptive_max_pool2d(x, output_size)<br>  return 0.5 * (x_avg + x_max)<br>def cat_avgmax_pool2d(x, output_size=1):<br>  x_avg = F.adaptive_avg_pool2d(x, output_size)<br>  x_max = F.adaptive_max_pool2d(x, output_size)<br>  return torch.cat([x_avg, x_max], 1)<br>PPT示例：<br>Add策略输出：[[6,6.5],[3.25,3.25]]；<br>Cat策略输出：[[7,8,5,5],[4,4,2.5,2.5]] |<img width="1775" height="684" alt="image" src="https://github.com/user-attachments/assets/023a04c3-46e9-47f0-a7ff-147bf4e93d4a" />|


## 3.5 4种池化类型对比
### 核心内容：各类型特点  
| 池化类型               | 总结特点                                                        |
|------------------------|--------------------------------------------------------------------------|
| 最大池化               | 减小卷积层参数误差造成的估计均值偏移，更多保留纹理信息，关注重要局部特征   |
| 平均池化               | 减小邻域大小受限造成的估计值方差增大，更多保留背景信息，关注全局特征       |
| 随机池化               | 介于两者之间；按数值赋概率、按概率采样；平均意义近似平均池化，局部服从最大池化准则 |
| 组合池化               | 结合两种或多种经典池化逻辑，吸收每种池化优点                               |


### ➡️ 跳转至下一部分  
理解分类后，点击学习池化应用与总结：  
**[第03章：池化操作 - 第3部分](chter02.md)**
