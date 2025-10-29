# 《导论.doc》神经网络与深度学习题库（完美交互+视觉反馈版）
✅ 选项点击变浅蓝（选中反馈） | ✅ 正确显绿色/错误显红色 | ✅ 论述题无乱码 | ✅ 解析清晰可见

<!-- 核心样式：解决选中无反馈问题 -->
<style>
/* 单选/多选选中后，选项文字变浅蓝（直观反馈） */
input[type="radio"]:checked + label,
input[type="checkbox"]:checked + label {
  color: #1a73e8;
  font-weight: 500;
}
/* 选项按钮和文字对齐 */
input[type="radio"], input[type="checkbox"] {
  margin-right: 8px;
  vertical-align: middle;
}
label {
  vertical-align: middle;
  cursor: pointer;
}
/* 提交按钮样式 */
button {
  padding: 6px 12px;
  background: #1a73e8;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}
button:hover {
  background: #1557b0;
}
/* 结果区域样式 */
.res-div {
  margin: 10px 0;
  padding: 8px;
  background: #f5f5f5;
  border-radius: 4px;
}
</style>

## 一、单选题（点击选项变浅蓝，提交显结果）
### 1. 在神经网络中，输入层的主要作用是什么？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single1" id="s1-A"> <label for="s1-A">A、对数据进行非线性变换</label><br>
  <input type="radio" name="single1" id="s1-B"> <label for="s1-B">B、对数据进行归一化处理</label><br>
  <input type="radio" name="single1" id="s1-C"> <label for="s1-C">C、接收外部输入的数据</label><br>
  <input type="radio" name="single1" id="s1-D"> <label for="s1-D">D、对数据进行降维处理</label>
</div>
<button onclick="checkSingle('single1', 's1-C', '解析：输入层是神经网络的第一层，核心作用是接收外部输入数据（如图像像素、文本向量），为后续处理提供原始信息。')">提交答案</button>
<div id="res-single1" class="res-div"></div>


### 2. 下列哪一项是卷积神经网络（CNN）最突出的特点？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single2" id="s2-A"> <label for="s2-A">A、使用全连接层进行全局特征提取</label><br>
  <input type="radio" name="single2" id="s2-B"> <label for="s2-B">B、通过卷积操作提取局部特征</label><br>
  <input type="radio" name="single2" id="s2-C"> <label for="s2-C">C、使用递归结构处理序列数据</label><br>
  <input type="radio" name="single2" id="s2-D"> <label for="s2-D">D、采用强化学习方式进行训练</label>
</div>
<button onclick="checkSingle('single2', 's2-B', '解析：CNN的核心特点是通过卷积操作提取局部特征（如图像的边缘、纹理），结合权值共享减少参数，适配空间结构数据。')">提交答案</button>
<div id="res-single2" class="res-div"></div>


### 3. 在神经网络中，激活函数的作用是什么？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single3" id="s3-A"> <label for="s3-A">A、计算神经元之间的权重</label><br>
  <input type="radio" name="single3" id="s3-B"> <label for="s3-B">B、引入非线性，使模型能拟合复杂函数</label><br>
  <input type="radio" name="single3" id="s3-C"> <label for="s3-C">C、减少模型的训练时间</label><br>
  <input type="radio" name="single3" id="s3-D"> <label for="s3-D">D、提高模型的精度</label>
</div>
<button onclick="checkSingle('single3', 's3-B', '解析：激活函数是引入非线性的关键，若无激活函数，无论多少层神经网络都是线性模型，无法拟合复杂数据分布。')">提交答案</button>
<div id="res-single3" class="res-div"></div>


### 4. 下列哪种损失函数适用于分类任务？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single4" id="s4-A"> <label for="s4-A">A、均方误差（MSE）</label><br>
  <input type="radio" name="single4" id="s4-B"> <label for="s4-B">B、交叉熵损失</label><br>
  <input type="radio" name="single4" id="s4-C"> <label for="s4-C">C、三重态损耗（Triplet Loss）</label><br>
  <input type="radio" name="single4" id="s4-D"> <label for="s4-D">D、铰链损耗（Hinge Loss）</label>
</div>
<button onclick="checkSingle('single4', 's4-B', '解析：交叉熵损失能衡量预测概率分布与真实标签分布的差异，是分类任务（如多类别识别）的常用损失函数。')">提交答案</button>
<div id="res-single4" class="res-div"></div>


## 二、多选题（点击选项变浅蓝，提交显结果）
### 5. 下列哪些是神经网络的基本组成部分？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi5" id="m5-A"> <label for="m5-A">A、输入层</label><br>
  <input type="checkbox" name="multi5" id="m5-B"> <label for="m5-B">B、隐藏层</label><br>
  <input type="checkbox" name="multi5" id="m5-C"> <label for="m5-C">C、输出层</label><br>
  <input type="checkbox" name="multi5" id="m5-D"> <label for="m5-D">D、激活函数</label><br>
  <input type="checkbox" name="multi5" id="m5-E"> <label for="m5-E">E、数据库</label>
</div>
<button onclick="checkMulti('multi5', ['m5-A','m5-B','m5-C','m5-D'], '解析：神经网络的基本结构包括输入层（接收数据）、隐藏层（特征处理）、输出层（输出结果），激活函数引入非线性，数据库不属于网络组成。')">提交答案</button>
<div id="res-multi5" class="res-div"></div>


### 6. 下列哪些是深度学习相较于传统机器学习的优势？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi6" id="m6-A"> <label for="m6-A">A、自动提取特征</label><br>
  <input type="checkbox" name="multi6" id="m6-B"> <label for="m6-B">B、依赖人工特征工程</label><br>
  <input type="checkbox" name="multi6" id="m6-C"> <label for="m6-C">C、处理高维数据能力强</label><br>
  <input type="checkbox" name="multi6" id="m6-D"> <label for="m6-D">D、对数据量需求较低</label><br>
  <input type="checkbox" name="multi6" id="m6-E"> <label for="m6-E">E、模型泛化能力更强</label>
</div>
<button onclick="checkMulti('multi6', ['m6-A','m6-C','m6-E'], '解析：深度学习无需人工设计特征（自动提取），能处理图像、文本等高维数据，大规模数据下泛化能力优于传统方法；但依赖大量数据，B、D是传统机器学习特点。')">提交答案</button>
<div id="res-multi6" class="res-div"></div>


### 7. 下列哪些是神经网络中常用的优化器？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi7" id="m7-A"> <label for="m7-A">A、SGD（随机梯度下降）</label><br>
  <input type="checkbox" name="multi7" id="m7-B"> <label for="m7-B">B、Adam</label><br>
  <input type="checkbox" name="multi7" id="m7-C"> <label for="m7-C">C、RMSProp</label><br>
  <input type="checkbox" name="multi7" id="m7-D"> <label for="m7-D">D、LSTM（循环神经网络结构）</label><br>
  <input type="checkbox" name="multi7" id="m7-E"> <label for="m7-E">E、ResNet（深度残差网络模型）</label>
</div>
<button onclick="checkMulti('multi7', ['m7-A','m7-B','m7-C'], '解析：SGD、Adam、RMSProp是常用优化器，用于更新网络参数；LSTM是网络结构，ResNet是具体模型，均不属于优化器。')">提交答案</button>
<div id="res-multi7" class="res-div"></div>


### 8. 下列哪些是深度学习在计算机视觉中的典型应用？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi8" id="m8-A"> <label for="m8-A">A、图像分类</label><br>
  <input type="checkbox" name="multi8" id="m8-B"> <label for="m8-B">B、目标检测</label><br>
  <input type="checkbox" name="multi8" id="m8-C"> <label for="m8-C">C、语音识别（NLP领域）</label><br>
  <input type="checkbox" name="multi8" id="m8-D"> <label for="m8-D">D、图像分割</label><br>
  <input type="checkbox" name="multi8" id="m8-E"> <label for="m8-E">E、自然语言处理（NLP领域）</label>
</div>
<button onclick="checkMulti('multi8', ['m8-A','m8-B','m8-D'], '解析：图像分类、目标检测、图像分割是计算机视觉核心应用；语音识别、自然语言处理属于NLP领域，与计算机视觉无关。')">提交答案</button>
<div id="res-multi8" class="res-div"></div>


## 三、判断题（点击选项变浅蓝，提交显结果）
### 9. 神经网络的隐藏层数越多，模型的表达能力一定越强。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge9" id="j9-T"> <label for="j9-T">正确</label><br>
  <input type="radio" name="judge9" id="j9-F"> <label for="j9-F">错误</label>
</div>
<button onclick="checkSingle('judge9', 'j9-F', '解析：过多隐藏层会导致训练困难（梯度消失）、过拟合，反而降低性能，并非层数越多表达能力越强。')">提交答案</button>
<div id="res-judge9" class="res-div"></div>


### 10. 卷积神经网络（CNN）主要用于处理图像数据。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge10" id="j10-T"> <label for="j10-T">正确</label><br>
  <input type="radio" name="judge10" id="j10-F"> <label for="j10-F">错误</label>
</div>
<button onclick="checkSingle('judge10', 'j10-T', '解析：CNN设计初衷是处理图像（保留空间结构），通过卷积提取局部特征，广泛用于图像识别、目标检测等任务。')">提交答案</button>
<div id="res-judge10" class="res-div"></div>


### 11. 反向传播算法是神经网络训练的核心算法之一。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge11" id="j11-T"> <label for="j11-T">正确</label><br>
  <input type="radio" name="judge11" id="j11-F"> <label for="j11-F">错误</label>
</div>
<button onclick="checkSingle('judge11', 'j11-T', '解析：反向传播通过链式求导计算梯度，指导参数更新，是训练多层神经网络的核心技术，无反向传播则无法优化深层模型。')">提交答案</button>
<div id="res-judge11" class="res-div"></div>


### 12. 深度学习模型在小规模数据集上的表现通常优于传统机器学习模型。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge12" id="j12-T"> <label for="j12-T">正确</label><br>
  <input type="radio" name="judge12" id="j12-F"> <label for="j12-F">错误</label>
</div>
<button onclick="checkSingle('judge12', 'j12-F', '解析：深度学习需大量数据拟合复杂参数，小规模数据下易过拟合；传统机器学习（如SVM、决策树）对数据量要求低，表现更优。')">提交答案</button>
<div id="res-judge12" class="res-div"></div>


### 22. 梯度下降法总是能找到全局最优解。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge22" id="j22-T"> <label for="j22-T">正确</label><br>
  <input type="radio" name="judge22" id="j22-F"> <label for="j22-F">错误</label>
</div>
<button onclick="checkSingle('judge22', 'j22-F', '解析：梯度下降易陷入局部最优解（如损失函数非凸），仅在凸函数中能保证找到全局最优，无法“总是”找到。')">提交答案</button>
<div id="res-judge22" class="res-div"></div>


### 23. 梯度方向是函数值变化最快的方向。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge23" id="j23-T"> <label for="j23-T">正确</label><br>
  <input type="radio" name="judge23" id="j23-F"> <label for="j23-F">错误</label>
</div>
<button onclick="checkSingle('judge23', 'j23-T', '解析：数学上，梯度是函数在某点的方向导数最大值方向，即函数值上升最快的方向，梯度下降沿反方向（下降最快）更新参数。')">提交答案</button>
<div id="res-judge23" class="res-div"></div>


## 四、填空题（输入后提交，显结果）
### 13. 神经网络的基本组成单元是______，它由输入、权重、偏置、求和函数和______等部分构成。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill13" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="答案用逗号分隔，如“神经元,激活函数”">
</div>
<button onclick="checkFill('fill13', '神经元,激活函数', '解析：神经元是神经网络的基本单元，结构包含输入、权重（调节输入重要性）、偏置（调整激活阈值）、求和函数（计算加权和）、激活函数（引入非线性）。')">提交答案</button>
<div id="res-fill13" class="res-div"></div>


### 14. 卷积神经网络（CNN）主要包括卷积层、______和全连接层三个核心部分。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill14" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="填写单个答案，如“池化层”">
</div>
<button onclick="checkFill('fill14', '池化层', '解析：CNN核心结构分工：卷积层（提取局部特征）、池化层（压缩特征维度，增强鲁棒性）、全连接层（整合特征并分类）。')">提交答案</button>
<div id="res-fill14" class="res-div"></div>


### 15. 在神经网络中，______函数用于衡量预测值与真实值之间的差距，常见的有均方误差和______损失。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill15" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="答案用逗号分隔，如“损失,交叉熵”">
</div>
<button onclick="checkFill('fill15', '损失,交叉熵', '解析：损失函数是模型优化的目标，均方误差常用于回归任务，交叉熵损失常用于分类任务，两者均用于量化预测与真实值的差距。')">提交答案</button>
<div id="res-fill15" class="res-div"></div>


### 16. 反向传播算法通过计算损失函数相对于参数的______，指导神经网络的参数更新。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill16" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="填写单个答案，如“梯度”">
</div>
<button onclick="checkFill('fill16', '梯度', '解析：反向传播的核心是“梯度计算”——通过链式求导得到损失对每个参数的梯度，再沿梯度反方向更新参数，实现损失最小化。')">提交答案</button>
<div id="res-fill16" class="res-div"></div>


## 五、论述题（点击展开，无乱码）
### 17. 请简述神经网络与深度学习的关系。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong style="color: #2ca02c;">答案</strong>：神经网络是深度学习的基础，深度学习是神经网络的“深度化”发展。<br>
    具体来说：①神经网络提供结构框架（输入层、隐藏层、输出层+激活函数）；②深度学习通过增加隐藏层数量（构建“深度神经网络”），结合卷积、循环等特殊结构，解决了传统浅层神经网络无法处理高维复杂数据的问题，实现自动特征提取和复杂模式识别，是当前AI领域的核心技术。<br><br>
    <strong style="color: #1a73e8;">解析</strong>：传统神经网络（2-3层）仅能处理简单线性问题，深度学习（10层以上）通过“深度”突破表达能力限制，在图像、语音、文本等领域实现技术突破。
  </div>
</details>


### 18. 请说明卷积神经网络（CNN）在图像识别中的优势。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong style="color: #2ca02c;">答案</strong>：CNN在图像识别中有三大核心优势：<br>
    1. 局部感知野：卷积核仅关注图像局部区域，符合人类视觉“先识别局部再整合全局”的逻辑，能有效提取边缘、纹理等基础特征；<br>
    2. 权值共享：同一卷积核在图像不同位置使用相同权重，大幅减少参数数量（如1000x1000图像用5x5卷积核，参数从百万级降为25个），降低过拟合和计算成本；<br>
    3. 池化层作用：通过最大池化/平均池化压缩特征维度，增强模型对图像平移、缩放、旋转的鲁棒性（如“猫”的图像即使位置偏移，仍能识别）。<br><br>
    <strong style="color: #1a73e8;">解析</strong>：传统全连接网络将图像拉平为一维向量，丢失空间信息且参数冗余，CNN保留二维结构，是图像识别任务的“最优选择”。
  </div>
</details>


### 19. 请解释什么是激活函数及其在神经网络中的作用。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong style="color: #2ca02c;">答案</strong>：<br>
    定义：激活函数是定义在神经网络神经元上的非线性函数，输入为神经元的“加权和+偏置”，输出为神经元的最终激活值。<br>
    核心作用：引入非线性变换——若没有激活函数，无论神经网络有多少层，整体输出都是输入的线性组合（线性模型），无法拟合异或、图像分类等非线性问题；通过激活函数（如ReLU、sigmoid），模型能学习复杂的数据分布和函数关系。<br><br>
    <strong style="color: #1a73e8;">解析</strong>：例如“异或问题”，线性模型无法区分（输出为直线），但通过sigmoid激活函数的非线性，两层神经网络即可正确分类，可见激活函数是神经网络“拟合复杂问题”的关键。
  </div>
</details>


### 20. 请简述反向传播算法的原理。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong style="color: #2ca02c;">答案</strong>：反向传播算法是训练多层神经网络的“误差反馈机制”，核心原理分两步：<br>
    1. 前向传播：输入数据从输入层传入，经隐藏层各神经元的“加权和+激活函数”计算，最终从输出层得到预测值，同时计算预测值与真实值的损失（如交叉熵、均方误差）；<br>
    2. 反向传播：从输出层开始，利用链式求导法则计算“损失函数相对于每个参数（权重、偏置）的梯度”——输出层梯度直接由损失函数求导得到，隐藏层梯度依赖后一层的梯度（“误差反向传递”），最后沿梯度反方向更新参数（梯度下降），最小化损失。<br><br>
    <strong style="color: #1a73e8;">解析</strong>：反向传播的本质是“链式求导的工程实现”，解决了多层神经网络参数难以优化的问题，是深度学习能落地的“核心基石”。
  </div>
</details>


### 21. 请简述梯度下降法的基本思想。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong style="color: #2ca02c;">答案</strong>：梯度下降法是一种“迭代式优化算法”，基本思想可概括为“沿下坡最快的方向走，逐步靠近最低点”：<br>
    1. 初始化参数：随机设定神经网络的权重、偏置等参数；<br>
    2. 计算梯度：通过前向传播得到损失，再通过反向传播计算损失函数在当前参数处的梯度（梯度方向是函数值上升最快的方向）；<br>
    3. 更新参数：沿梯度反方向（函数值下降最快的方向）调整参数，更新公式为“新参数 = 旧参数 - 学习率×梯度”（学习率控制步长，避免步过大震荡、步过小训练慢）；<br>
    4. 迭代收敛：重复“计算梯度→更新参数”的过程，直到损失函数值不再下降（收敛），得到最优参数。<br><br>
    <strong style="color: #1a73e8;">解析</strong>：梯度下降是“最简单但最有效”的优化方法，衍生出SGD（随机梯度下降）、Adam等变种，但核心思想均为“沿梯度反方向迭代优化”。
  </div>
</details>


<!-- 修复后无语法错误的判分脚本 -->
<script>
// 单选题/判断题判分（正确绿/错误红，带解析）
function checkSingle(questionName, correctId, explanation) {
  // 定位选中的选项
  const selected = document.querySelector(`input[name="${questionName}"][type="radio"]:checked`);
  const resDiv = document.getElementById(`res-${questionName}`);

  // 未选择时提示
  if (!selected) {
    resDiv.innerHTML = "<span style='color: #ff7f0e;'>⚠️ 请先选择一个选项再提交！</span>";
    return;
  }

  // 正确/错误结果（绿色/红色）
  if (selected.id === correctId) {
    resDiv.innerHTML = `<span style='color: #2ca02c;'>✅ 回答正确！</span><br><span style='color: #666;'>${explanation}</span>`;
  } else {
    const correctLabel = document.querySelector(`label[for="${correctId}"]`).textContent;
    resDiv.innerHTML = `<span style='color: #d62728;'>❌ 回答错误！</span><br><span style='color: #666;'>正确答案：${correctLabel}<br>${explanation}</span>`;
  }
}

// 多选题判分（正确绿/错误红，带解析）
function checkMulti(questionName, correctIds, explanation) {
  // 定位所有选中的选项
  const selected = Array.from(
    document.querySelectorAll(`input[name="${questionName}"][type="checkbox"]:checked`)
  ).map(el => el.id);
  const resDiv = document.getElementById(`res-${questionName}`);

  // 未选择时提示
  if (selected.length === 0) {
    resDiv.innerHTML = "<span style='color: #ff7f0e;'>⚠️ 请至少选择一个选项再提交！</span>";
    return;
  }

  // 排序对比（避免选择顺序影响结果）
  const isCorrect = JSON.stringify(selected.sort()) === JSON.stringify(correctIds.sort());
  const correctLabels = correctIds.map(id => document.querySelector(`label[for="${id}"]`).textContent).join("、");

  // 正确/错误结果
  if (isCorrect) {
    resDiv.innerHTML = `<span style='color: #2ca02c;'>✅ 回答正确！</span><br><span style='color: #666;'>${explanation}</span>`;
  } else {
    resDiv.innerHTML = `<span style='color: #d62728;'>❌ 回答错误！</span><br><span style='color: #666;'>正确答案：${correctLabels}<br>${explanation}</span>`;
  }
}

// 填空题判分（正确绿/错误红，带解析）
function checkFill(inputId, correctAnswer, explanation) {
  const inputEl = document.getElementById(inputId);
  const userAnswer = inputEl.value.trim();
  const resDiv = document.getElementById(`res-${inputId}`);

  // 未填写时提示
  if (!userAnswer) {
    resDiv.innerHTML = "<span style='color: #ff7f0e;'>⚠️ 请先填写答案再提交！</span>";
    return;
  }

  // 忽略空格和大小写（兼容输入格式）
  const normalize = str => str.replace(/\s+/g, '').toLowerCase();
  if (normalize(userAnswer) === normalize(correctAnswer)) {
    resDiv.innerHTML = `<span style='color: #2ca02c;'>✅ 回答正确！</span><br><span style='color: #666;'>${explanation}</span>`;
  } else {
    resDiv.innerHTML = `<span style='color: #d62728;'>❌ 回答错误！</span><br><span style='color: #666;'>正确答案：${correctAnswer}<br>${explanation}</span>`;
  }
}
</script>
