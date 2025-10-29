# 神经网络与深度学习题库（23题·点击交互版）

<!-- 基础样式：确保显示和交互兼容 -->
<style>
.option { margin: 6px 0; cursor: pointer; }
input[type="radio"], input[type="checkbox"] { margin-right: 8px; vertical-align: middle; }
label { vertical-align: middle; cursor: pointer; }
.correct { color: #0f9d58; background: #e6f4ea; padding: 2px 4px; border-radius: 2px; }
.incorrect { color: #d93025; background: #fce8e6; padding: 2px 4px; border-radius: 2px; }
.explanation { margin: 5px 0 10px 20px; color: #5f6368; font-size: 0.9em; }
.fill-ans { margin: 5px 0; color: #1a73e8; }
details { margin: 10px 0; padding: 5px; background: #f5f5f5; border-radius: 4px; }
summary { cursor: pointer; font-weight: bold; }
</style>

## 一、单选题（4题）
### 1. 神经网络输入层的主要作用是？
- <div class="option">
  <input type="radio" name="s1" id="s1-A"> 
  <label for="s1-A" onclick="checkSingle('s1', 's1-C', 'exp1', '解析：输入层是神经网络的“数据入口”，仅接收外部原始数据，不参与数据变换。')">A. 对数据进行非线性变换</label>
</div>
- <div class="option">
  <input type="radio" name="s1" id="s1-B"> 
  <label for="s1-B" onclick="checkSingle('s1', 's1-C', 'exp1', '解析：输入层是神经网络的“数据入口”，仅接收外部原始数据，不参与数据变换。')">B. 对数据进行归一化处理</label>
</div>
- <div class="option">
  <input type="radio" name="s1" id="s1-C"> 
  <label for="s1-C" onclick="checkSingle('s1', 's1-C', 'exp1', '解析：输入层是神经网络的“数据入口”，仅接收外部原始数据，不参与数据变换。')">C. 接收外部输入的数据</label>
</div>
- <div class="option">
  <input type="radio" name="s1" id="s1-D"> 
  <label for="s1-D" onclick="checkSingle('s1', 's1-C', 'exp1', '解析：输入层是神经网络的“数据入口”，仅接收外部原始数据，不参与数据变换。')">D. 对数据进行降维处理</label>
</div>
<div class="explanation" id="exp1"></div>


### 2. 卷积神经网络（CNN）最突出的特点是？
- <div class="option">
  <input type="radio" name="s2" id="s2-A"> 
  <label for="s2-A" onclick="checkSingle('s2', 's2-B', 'exp2', '解析：CNN通过卷积核提取图像局部特征，结合权值共享减少参数，适配图像空间结构。')">A. 使用全连接层进行全局特征提取</label>
</div>
- <div class="option">
  <input type="radio" name="s2" id="s2-B"> 
  <label for="s2-B" onclick="checkSingle('s2', 's2-B', 'exp2', '解析：CNN通过卷积核提取图像局部特征，结合权值共享减少参数，适配图像空间结构。')">B. 通过卷积操作提取局部特征</label>
</div>
- <div class="option">
  <input type="radio" name="s2" id="s2-C"> 
  <label for="s2-C" onclick="checkSingle('s2', 's2-B', 'exp2', '解析：CNN通过卷积核提取图像局部特征，结合权值共享减少参数，适配图像空间结构。')">C. 使用递归结构处理序列数据</label>
</div>
- <div class="option">
  <input type="radio" name="s2" id="s2-D"> 
  <label for="s2-D" onclick="checkSingle('s2', 's2-B', 'exp2', '解析：CNN通过卷积核提取图像局部特征，结合权值共享减少参数，适配图像空间结构。')">D. 采用强化学习方式进行训练</label>
</div>
<div class="explanation" id="exp2"></div>


### 3. 激活函数在神经网络中的作用是？
- <div class="option">
  <input type="radio" name="s3" id="s3-A"> 
  <label for="s3-A" onclick="checkSingle('s3', 's3-B', 'exp3', '解析：无激活函数时神经网络是线性模型，激活函数通过非线性变换赋予复杂拟合能力。')">A. 计算神经元之间的权重</label>
</div>
- <div class="option">
  <input type="radio" name="s3" id="s3-B"> 
  <label for="s3-B" onclick="checkSingle('s3', 's3-B', 'exp3', '解析：无激活函数时神经网络是线性模型，激活函数通过非线性变换赋予复杂拟合能力。')">B. 引入非线性，使模型能拟合复杂函数</label>
</div>
- <div class="option">
  <input type="radio" name="s3" id="s3-C"> 
  <label for="s3-C" onclick="checkSingle('s3', 's3-B', 'exp3', '解析：无激活函数时神经网络是线性模型，激活函数通过非线性变换赋予复杂拟合能力。')">C. 减少模型的训练时间</label>
</div>
- <div class="option">
  <input type="radio" name="s3" id="s3-D"> 
  <label for="s3-D" onclick="checkSingle('s3', 's3-B', 'exp3', '解析：无激活函数时神经网络是线性模型，激活函数通过非线性变换赋予复杂拟合能力。')">D. 提高模型的精度</label>
</div>
<div class="explanation" id="exp3"></div>


### 4. 下列哪种损失函数适用于分类任务？
- <div class="option">
  <input type="radio" name="s4" id="s4-A"> 
  <label for="s4-A" onclick="checkSingle('s4', 's4-B', 'exp4', '解析：交叉熵损失衡量预测与真实标签的分布差异，是分类任务的首选损失函数。')">A. 均方误差（MSE）</label>
</div>
- <div class="option">
  <input type="radio" name="s4" id="s4-B"> 
  <label for="s4-B" onclick="checkSingle('s4', 's4-B', 'exp4', '解析：交叉熵损失衡量预测与真实标签的分布差异，是分类任务的首选损失函数。')">B. 交叉熵损失</label>
</div>
- <div class="option">
  <input type="radio" name="s4" id="s4-C"> 
  <label for="s4-C" onclick="checkSingle('s4', 's4-B', 'exp4', '解析：交叉熵损失衡量预测与真实标签的分布差异，是分类任务的首选损失函数。')">C. 三重态损耗（Triplet Loss）</label>
</div>
- <div class="option">
  <input type="radio" name="s4" id="s4-D"> 
  <label for="s4-D" onclick="checkSingle('s4', 's4-B', 'exp4', '解析：交叉熵损失衡量预测与真实标签的分布差异，是分类任务的首选损失函数。')">D. 铰链损耗（Hinge Loss）</label>
</div>
<div class="explanation" id="exp4"></div>


## 二、多选题（4题）
### 5. 神经网络的基本组成部分包括？
- <div class="option">
  <input type="checkbox" name="m5" id="m5-A"> 
  <label for="m5-A" onclick="checkMulti('m5', ['m5-A','m5-B','m5-C','m5-D'], 'exp5', '解析：输入层、隐藏层、输出层构成网络结构，激活函数引入非线性，数据库不属于网络组成。')">A. 输入层</label>
</div>
- <div class="option">
  <input type="checkbox" name="m5" id="m5-B"> 
  <label for="m5-B" onclick="checkMulti('m5', ['m5-A','m5-B','m5-C','m5-D'], 'exp5', '解析：输入层、隐藏层、输出层构成网络结构，激活函数引入非线性，数据库不属于网络组成。')">B. 隐藏层</label>
</div>
- <div class="option">
  <input type="checkbox" name="m5" id="m5-C"> 
  <label for="m5-C" onclick="checkMulti('m5', ['m5-A','m5-B','m5-C','m5-D'], 'exp5', '解析：输入层、隐藏层、输出层构成网络结构，激活函数引入非线性，数据库不属于网络组成。')">C. 输出层</label>
</div>
- <div class="option">
  <input type="checkbox" name="m5" id="m5-D"> 
  <label for="m5-D" onclick="checkMulti('m5', ['m5-A','m5-B','m5-C','m5-D'], 'exp5', '解析：输入层、隐藏层、输出层构成网络结构，激活函数引入非线性，数据库不属于网络组成。')">D. 激活函数</label>
</div>
- <div class="option">
  <input type="checkbox" name="m5" id="m5-E"> 
  <label for="m5-E" onclick="checkMulti('m5', ['m5-A','m5-B','m5-C','m5-D'], 'exp5', '解析：输入层、隐藏层、输出层构成网络结构，激活函数引入非线性，数据库不属于网络组成。')">E. 数据库</label>
</div>
<div class="explanation" id="exp5"></div>


### 6. 深度学习相较于传统机器学习的优势是？
- <div class="option">
  <input type="checkbox" name="m6" id="m6-A"> 
  <label for="m6-A" onclick="checkMulti('m6', ['m6-A','m6-C','m6-E'], 'exp6', '解析：深度学习自动提取特征、处理高维数据能力强，大规模数据下泛化能力更优。')">A. 自动提取特征</label>
</div>
- <div class="option">
  <input type="checkbox" name="m6" id="m6-B"> 
  <label for="m6-B" onclick="checkMulti('m6', ['m6-A','m6-C','m6-E'], 'exp6', '解析：深度学习自动提取特征、处理高维数据能力强，大规模数据下泛化能力更优。')">B. 依赖人工特征工程</label>
</div>
- <div class="option">
  <input type="checkbox" name="m6" id="m6-C"> 
  <label for="m6-C" onclick="checkMulti('m6', ['m6-A','m6-C','m6-E'], 'exp6', '解析：深度学习自动提取特征、处理高维数据能力强，大规模数据下泛化能力更优。')">C. 处理高维数据能力强</label>
</div>
- <div class="option">
  <input type="checkbox" name="m6" id="m6-D"> 
  <label for="m6-D" onclick="checkMulti('m6', ['m6-A','m6-C','m6-E'], 'exp6', '解析：深度学习自动提取特征、处理高维数据能力强，大规模数据下泛化能力更优。')">D. 对数据量需求较低</label>
</div>
- <div class="option">
  <input type="checkbox" name="m6" id="m6-E"> 
  <label for="m6-E" onclick="checkMulti('m6', ['m6-A','m6-C','m6-E'], 'exp6', '解析：深度学习自动提取特征、处理高维数据能力强，大规模数据下泛化能力更优。')">E. 模型泛化能力更强</label>
</div>
<div class="explanation" id="exp6"></div>


### 7. 神经网络中常用的优化器有？
- <div class="option">
  <input type="checkbox" name="m7" id="m7-A"> 
  <label for="m7-A" onclick="checkMulti('m7', ['m7-A','m7-B','m7-C'], 'exp7', '解析：SGD、Adam、RMSProp是参数优化算法，LSTM是网络结构，ResNet是模型。')">A. SGD</label>
</div>
- <div class="option">
  <input type="checkbox" name="m7" id="m7-B"> 
  <label for="m7-B" onclick="checkMulti('m7', ['m7-A','m7-B','m7-C'], 'exp7', '解析：SGD、Adam、RMSProp是参数优化算法，LSTM是网络结构，ResNet是模型。')">B. Adam</label>
</div>
- <div class="option">
  <input type="checkbox" name="m7" id="m7-C"> 
  <label for="m7-C" onclick="checkMulti('m7', ['m7-A','m7-B','m7-C'], 'exp7', '解析：SGD、Adam、RMSProp是参数优化算法，LSTM是网络结构，ResNet是模型。')">C. RMSProp</label>
</div>
- <div class="option">
  <input type="checkbox" name="m7" id="m7-D"> 
  <label for="m7-D" onclick="checkMulti('m7', ['m7-A','m7-B','m7-C'], 'exp7', '解析：SGD、Adam、RMSProp是参数优化算法，LSTM是网络结构，ResNet是模型。')">D. LSTM</label>
</div>
- <div class="option">
  <input type="checkbox" name="m7" id="m7-E"> 
  <label for="m7-E" onclick="checkMulti('m7', ['m7-A','m7-B','m7-C'], 'exp7', '解析：SGD、Adam、RMSProp是参数优化算法，LSTM是网络结构，ResNet是模型。')">E. ResNet</label>
</div>
<div class="explanation" id="exp7"></div>


### 8. 深度学习在计算机视觉中的典型应用有？
- <div class="option">
  <input type="checkbox" name="m8" id="m8-A"> 
  <label for="m8-A" onclick="checkMulti('m8', ['m8-A','m8-B','m8-D'], 'exp8', '解析：图像分类、目标检测、图像分割是计算机视觉任务，语音识别、NLP属于另一领域。')">A. 图像分类</label>
</div>
- <div class="option">
  <input type="checkbox" name="m8" id="m8-B"> 
  <label for="m8-B" onclick="checkMulti('m8', ['m8-A','m8-B','m8-D'], 'exp8', '解析：图像分类、目标检测、图像分割是计算机视觉任务，语音识别、NLP属于另一领域。')">B. 目标检测</label>
</div>
- <div class="option">
  <input type="checkbox" name="m8" id="m8-C"> 
  <label for="m8-C" onclick="checkMulti('m8', ['m8-A','m8-B','m8-D'], 'exp8', '解析：图像分类、目标检测、图像分割是计算机视觉任务，语音识别、NLP属于另一领域。')">C. 语音识别</label>
</div>
- <div class="option">
  <input type="checkbox" name="m8" id="m8-D"> 
  <label for="m8-D" onclick="checkMulti('m8', ['m8-A','m8-B','m8-D'], 'exp8', '解析：图像分类、目标检测、图像分割是计算机视觉任务，语音识别、NLP属于另一领域。')">D. 图像分割</label>
</div>
- <div class="option">
  <input type="checkbox" name="m8" id="m8-E"> 
  <label for="m8-E" onclick="checkMulti('m8', ['m8-A','m8-B','m8-D'], 'exp8', '解析：图像分类、目标检测、图像分割是计算机视觉任务，语音识别、NLP属于另一领域。')">E. 自然语言处理</label>
</div>
<div class="explanation" id="exp8"></div>


## 三、判断题（6题）
### 9. 神经网络的隐藏层数越多，模型的表达能力一定越强。
- <div class="option">
  <input type="radio" name="j9" id="j9-T"> 
  <label for="j9-T" onclick="checkSingle('j9', 'j9-F', 'exp9', '解析：过多隐藏层导致梯度消失、过拟合，表达能力需结合数据量和正则化。')">正确</label>
</div>
- <div class="option">
  <input type="radio" name="j9" id="j9-F"> 
  <label for="j9-F" onclick="checkSingle('j9', 'j9-F', 'exp9', '解析：过多隐藏层导致梯度消失、过拟合，表达能力需结合数据量和正则化。')">错误</label>
</div>
<div class="explanation" id="exp9"></div>


### 10. 卷积神经网络（CNN）主要用于处理图像数据。
- <div class="option">
  <input type="radio" name="j10" id="j10-T"> 
  <label for="j10-T" onclick="checkSingle('j10', 'j10-T', 'exp10', '解析：CNN的卷积+池化结构保留图像空间信息，是图像任务的主流模型。')">正确</label>
</div>
- <div class="option">
  <input type="radio" name="j10" id="j10-F"> 
  <label for="j10-F" onclick="checkSingle('j10', 'j10-T', 'exp10', '解析：CNN的卷积+池化结构保留图像空间信息，是图像任务的主流模型。')">错误</label>
</div>
<div class="explanation" id="exp10"></div>


### 11. 反向传播算法是神经网络训练的核心算法之一。
- <div class="option">
  <input type="radio" name="j11" id="j11-T"> 
  <label for="j11-T" onclick="checkSingle('j11', 'j11-T', 'exp11', '解析：反向传播通过链式求导计算梯度，指导参数更新，是深层网络训练的关键。')">正确</label>
</div>
- <div class="option">
  <input type="radio" name="j11" id="j11-F"> 
  <label for="j11-F" onclick="checkSingle('j11', 'j11-T', 'exp11', '解析：反向传播通过链式求导计算梯度，指导参数更新，是深层网络训练的关键。')">错误</label>
</div>
<div class="explanation" id="exp11"></div>


### 12. 深度学习模型在小规模数据集上的表现通常优于传统机器学习模型。
- <div class="option">
  <input type="radio" name="j12" id="j12-T"> 
  <label for="j12-T" onclick="checkSingle('j12', 'j12-F', 'exp12', '解析：深度学习需大量数据拟合参数，小规模数据下易过拟合，传统模型表现更优。')">正确</label>
</div>
- <div class="option">
  <input type="radio" name="j12" id="j12-F"> 
  <label for="j12-F" onclick="checkSingle('j12', 'j12-F', 'exp12', '解析：深度学习需大量数据拟合参数，小规模数据下易过拟合，传统模型表现更优。')">错误</label>
</div>
<div class="explanation" id="exp12"></div>


### 22. 梯度下降法总是能找到全局最优解。
- <div class="option">
  <input type="radio" name="j22" id="j22-T"> 
  <label for="j22-T" onclick="checkSingle('j22', 'j22-F', 'exp22', '解析：梯度下降易陷入局部最优，仅凸函数中能保证全局最优，实际任务多为非凸。')">正确</label>
</div>
- <div class="option">
  <input type="radio" name="j22" id="j22-F"> 
  <label for="j22-F" onclick="checkSingle('j22', 'j22-F', 'exp22', '解析：梯度下降易陷入局部最优，仅凸函数中能保证全局最优，实际任务多为非凸。')">错误</label>
</div>
<div class="explanation" id="exp22"></div>


### 23. 梯度方向是函数值变化最快的方向。
- <div class="option">
  <input type="radio" name="j23" id="j23-T"> 
  <label for="j23-T" onclick="checkSingle('j23', 'j23-T', 'exp23', '解析：梯度是函数上升最快的方向，梯度下降沿反方向实现函数值下降最快。')">正确</label>
</div>
- <div class="option">
  <input type="radio" name="j23" id="j23-F"> 
  <label for="j23-F" onclick="checkSingle('j23', 'j23-T', 'exp23', '解析：梯度是函数上升最快的方向，梯度下降沿反方向实现函数值下降最快。')">错误</label>
</div>
<div class="explanation" id="exp23"></div>


## 四、填空题（4题）
### 13. 神经网络的基本组成单元是______，它由输入、权重、偏置、求和函数和______等部分构成。
- <div class="option" onclick="showFill('exp13', '神经元,激活函数', '解析：神经元是基本单元，激活函数引入非线性。')">点击查看答案</div>
<div class="fill-ans" id="exp13"></div>


### 14. 卷积神经网络（CNN）主要包括卷积层、______和全连接层三个核心部分。
- <div class="option" onclick="showFill('exp14', '池化层', '解析：池化层压缩特征维度，增强模型鲁棒性。')">点击查看答案</div>
<div class="fill-ans" id="exp14"></div>


### 15. 在神经网络中，______函数用于衡量预测值与真实值之间的差距，常见的有均方误差和______损失。
- <div class="option" onclick="showFill('exp15', '损失,交叉熵', '解析：损失函数是优化目标，均方误差适用于回归，交叉熵适用于分类。')">点击查看答案</div>
<div class="fill-ans" id="exp15"></div>


### 16. 反向传播算法通过计算损失函数相对于参数的______，指导神经网络的参数更新。
- <div class="option" onclick="showFill('exp16', '梯度', '解析：梯度反映参数对损失的影响，是参数更新的依据。')">点击查看答案</div>
<div class="fill-ans" id="exp16"></div>


## 五、论述题（5题）
### 17. 请简述神经网络与深度学习的关系。
<details>
  <summary>点击查看答案</summary>
  <p>1. 神经网络是深度学习的基础：提供输入层、隐藏层、输出层+激活函数的基本结构，解决简单非线性问题；</p>
  <p>2. 深度学习是神经网络的升级：通过增加隐藏层数量（构建深度网络），结合卷积、循环等结构，实现自动特征提取，处理图像、语音等复杂数据；</p>
  <p>简言之，深度学习是“深度神经网络”的研究与应用，依赖神经网络的基础框架，同时突破其浅层局限。</p>
</details>


### 18. 请说明卷积神经网络（CNN）在图像识别中的优势。
<details>
  <summary>点击查看答案</summary>
  <p>1. 局部感知：卷积核仅关注图像局部区域（如3×3），符合人类视觉“先局部后全局”的逻辑，有效提取边缘、纹理等特征；</p>
  <p>2. 权值共享：同一卷积核在图像不同位置使用相同权重，大幅减少参数数量（如1000×1000图像参数从百万级降至几十），降低过拟合；</p>
  <p>3. 池化层作用：通过最大池化/平均池化压缩特征维度，增强模型对图像平移、缩放、旋转的鲁棒性（如猫的图像偏移后仍能识别）。</p>
</details>


### 19. 请解释什么是激活函数及其在神经网络中的作用。
<details>
  <summary>点击查看答案</summary>
  <p>定义：激活函数是神经元上的非线性函数，输入为“加权和+偏置”，输出为神经元的激活值；</p>
  <p>作用：引入非线性变换——无激活函数时，无论多少层神经网络都是线性模型（输出=输入线性组合），无法拟合异或、图像分类等非线性问题；激活函数（如ReLU、sigmoid）通过非线性处理，使模型能学习复杂数据分布，是神经网络“智能”的核心。</p>
</details>


### 20. 请简述反向传播算法的原理。
<details>
  <summary>点击查看答案</summary>
  <p>1. 前向传播：输入数据从输入层传入，经隐藏层“加权和+激活函数”计算，从输出层得到预测值，同时计算预测与真实值的损失（如交叉熵）；</p>
  <p>2. 反向传播：从输出层开始，用链式求导法则计算“损失对每个参数（权重、偏置）的梯度”——输出层梯度直接由损失函数求导得到，隐藏层梯度依赖后一层梯度（误差反向传递）；</p>
  <p>3. 参数更新：沿梯度反方向更新参数（梯度下降），最小化损失；</p>
  <p>核心：通过“误差反馈+梯度计算”，解决多层网络参数难以优化的问题。</p>
</details>


### 21. 请简述梯度下降法的基本思想。
<details>
  <summary>点击查看答案</summary>
  <p>1. 核心思想：沿损失函数下降最快的方向，迭代逼近最小值；</p>
  <p>步骤：①初始化参数（随机设定权重、偏置）；②计算梯度（前向传播得损失，反向传播算损失对参数的梯度，梯度是损失上升最快的方向）；③更新参数（新参数=旧参数-学习率×梯度，学习率控制步长，避免震荡或过慢）；④迭代收敛（重复②③，直到损失不再下降）；</p>
  <p>定位：深度学习中参数优化的基础算法，衍生出SGD、Adam等变种，但核心逻辑一致。</p>
</details>


<!-- 交互脚本：简化适配MD渲染 -->
<script>
// 单选题/判断题：点击选项显对错+解析
function checkSingle(radioName, correctId, expId, expText) {
  // 清除同题样式
  document.querySelectorAll(`input[name="${radioName}"] + label`).forEach(el => {
    el.classList.remove('correct', 'incorrect');
  });
  // 标记当前选项
  const currentLabel = document.querySelector(`label[for="${event.target.id}"]`);
  if (event.target.id === correctId) {
    currentLabel.classList.add('correct');
  } else {
    currentLabel.classList.add('incorrect');
  }
  // 显示解析
  document.getElementById(expId).textContent = expText;
}

// 多选题：点击选项显对错+解析
function checkMulti(checkboxName, correctIds, expId, expText) {
  const currentId = event.target.id;
  const currentLabel = document.querySelector(`label[for="${currentId}"]`);
  // 标记当前选项
  if (correctIds.includes(currentId)) {
    currentLabel.classList.add('correct');
    currentLabel.classList.remove('incorrect');
  } else {
    currentLabel.classList.add('incorrect');
    currentLabel.classList.remove('correct');
  }
  // 显示解析
  document.getElementById(expId).textContent = expText;
}

// 填空题：点击显答案+解析
function showFill(expId, answer, expText) {
  document.getElementById(expId).textContent = `答案：${answer} | ${expText}`;
}
</script>
