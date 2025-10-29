# 《导论.doc》神经网络与深度学习题库（修复交互版）
所有选项可点击、填空框可输入，提交后仅显示当前题答案。

## 一、单选题（点击选项后提交）
### 1. 在神经网络中，输入层的主要作用是什么？
<div style="margin: 10px 0; padding-left: 20px;">
  <!-- 修复：input的id与label的for严格对应，name每题唯一 -->
  <input type="radio" name="single1" id="s1-C" value="C"> <label for="s1-C">A、对数据进行非线性变换</label><br>
  <input type="radio" name="single1" id="s1-B" value="B"> <label for="s1-B">B、对数据进行归一化处理</label><br>
  <input type="radio" name="single1" id="s1-A" value="A"> <label for="s1-A">C、接收外部输入的数据</label><br>
  <input type="radio" name="single1" id="s1-D" value="D"> <label for="s1-D">D、对数据进行降维处理</label>
</div>
<button onclick="checkSingle('single1', 's1-A', '解析：输入层是神经网络的第一层，其主要职责是接收外部输入的数据，如图像的像素值、文本的词向量等，为后续的处理提供原始信息。')">提交答案</button>
<div id="res-single1" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 2. 下列哪一项是卷积神经网络（CNN）最突出的特点？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single2" id="s2-A" value="A"> <label for="s2-A">A、使用全连接层进行全局特征提取</label><br>
  <input type="radio" name="single2" id="s2-B" value="B"> <label for="s2-B">B、通过卷积操作提取局部特征</label><br>
  <input type="radio" name="single2" id="s2-C" value="C"> <label for="s2-C">C、使用递归结构处理序列数据</label><br>
  <input type="radio" name="single2" id="s2-D" value="D"> <label for="s2-D">D、采用强化学习方式进行训练</label>
</div>
<button onclick="checkSingle('single2', 's2-B', '解析：卷积神经网络通过卷积操作提取数据的局部特征，特别适用于图像识别等任务，是其区别于全连接神经网络的核心特点。')">提交答案</button>
<div id="res-single2" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 3. 在神经网络中，激活函数的作用是什么？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single3" id="s3-A" value="A"> <label for="s3-A">A、计算神经元之间的权重</label><br>
  <input type="radio" name="single3" id="s3-B" value="B"> <label for="s3-B">B、引入非线性，使模型能拟合复杂函数</label><br>
  <input type="radio" name="single3" id="s3-C" value="C"> <label for="s3-C">C、减少模型的训练时间</label><br>
  <input type="radio" name="single3" id="s3-D" value="D"> <label for="s3-D">D、提高模型的精度</label>
</div>
<button onclick="checkSingle('single3', 's3-B', '解析：激活函数是神经网络中引入非线性的关键组件，使得模型能够拟合复杂的数据分布和函数关系。')">提交答案</button>
<div id="res-single3" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 4. 下列哪种损失函数适用于分类任务？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="single4" id="s4-A" value="A"> <label for="s4-A">A、均方误差（MSE）</label><br>
  <input type="radio" name="single4" id="s4-B" value="B"> <label for="s4-B">B、交叉熵损失</label><br>
  <input type="radio" name="single4" id="s4-C" value="C"> <label for="s4-C">C、Triplet Loss</label><br>
  <input type="radio" name="single4" id="s4-D" value="D"> <label for="s4-D">D、Hinge Loss</label>
</div>
<button onclick="checkSingle('single4', 's4-B', '解析：交叉熵损失函数常用于分类任务，因为它能够衡量预测概率分布与真实分布之间的差异，从而指导模型优化。')">提交答案</button>
<div id="res-single4" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


## 二、多选题（可多选，点击选项后提交）
### 5. 下列哪些是神经网络的基本组成部分？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi5" id="m5-A" value="A"> <label for="m5-A">A、输入层</label><br>
  <input type="checkbox" name="multi5" id="m5-B" value="B"> <label for="m5-B">B、隐藏层</label><br>
  <input type="checkbox" name="multi5" id="m5-C" value="C"> <label for="m5-C">C、输出层</label><br>
  <input type="checkbox" name="multi5" id="m5-D" value="D"> <label for="m5-D">D、激活函数</label><br>
  <input type="checkbox" name="multi5" id="m5-E" value="E"> <label for="m5-E">E、数据库</label>
</div>
<button onclick="checkMulti('multi5', ['m5-A','m5-B','m5-C','m5-D'], '解析：神经网络的基本组成部分包括输入层、隐藏层、输出层以及激活函数，它们共同构成神经网络的结构和功能基础。')">提交答案</button>
<div id="res-multi5" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 6. 下列哪些是深度学习相较于传统机器学习的优势？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi6" id="m6-A" value="A"> <label for="m6-A">A、自动提取特征</label><br>
  <input type="checkbox" name="multi6" id="m6-B" value="B"> <label for="m6-B">B、依赖人工特征工程</label><br>
  <input type="checkbox" name="multi6" id="m6-C" value="C"> <label for="m6-C">C、处理高维数据能力强</label><br>
  <input type="checkbox" name="multi6" id="m6-D" value="D"> <label for="m6-D">D、对数据量需求较低</label><br>
  <input type="checkbox" name="multi6" id="m6-E" value="E"> <label for="m6-E">E、模型泛化能力更强</label>
</div>
<button onclick="checkMulti('multi6', ['m6-A','m6-C','m6-E'], '解析：深度学习能够自动提取特征，处理高维数据，并且在大规模数据集上表现出更强的泛化能力，这是其相较于传统机器学习的主要优势。')">提交答案</button>
<div id="res-multi6" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 7. 下列哪些是神经网络中常用的优化器？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi7" id="m7-A" value="A"> <label for="m7-A">A、SGD</label><br>
  <input type="checkbox" name="multi7" id="m7-B" value="B"> <label for="m7-B">B、Adam</label><br>
  <input type="checkbox" name="multi7" id="m7-C" value="C"> <label for="m7-C">C、RMSProp</label><br>
  <input type="checkbox" name="multi7" id="m7-D" value="D"> <label for="m7-D">D、LSTM</label><br>
  <input type="checkbox" name="multi7" id="m7-E" value="E"> <label for="m7-E">E、ResNet</label>
</div>
<button onclick="checkMulti('multi7', ['m7-A','m7-B','m7-C'], '解析：SGD、Adam 和 RMSProp 是常用的优化器，用于在训练过程中调整神经网络的参数，以最小化损失函数。')">提交答案</button>
<div id="res-multi7" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 8. 下列哪些是深度学习在计算机视觉中的典型应用？
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="checkbox" name="multi8" id="m8-A" value="A"> <label for="m8-A">A、图像分类</label><br>
  <input type="checkbox" name="multi8" id="m8-B" value="B"> <label for="m8-B">B、目标检测</label><br>
  <input type="checkbox" name="multi8" id="m8-C" value="C"> <label for="m8-C">C、语音识别</label><br>
  <input type="checkbox" name="multi8" id="m8-D" value="D"> <label for="m8-D">D、图像分割</label><br>
  <input type="checkbox" name="multi8" id="m8-E" value="E"> <label for="m8-E">E、自然语言处理</label>
</div>
<button onclick="checkMulti('multi8', ['m8-A','m8-B','m8-D'], '解析：图像分类、目标检测和图像分割是深度学习在计算机视觉中的典型应用，而语音识别和自然语言处理则更多应用于NLP领域。')">提交答案</button>
<div id="res-multi8" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


## 三、判断题（点击选项后提交）
### 9. 神经网络的隐藏层数越多，模型的表达能力一定越强。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge9" id="j9-T" value="正确"> <label for="j9-T">正确</label><br>
  <input type="radio" name="judge9" id="j9-F" value="错误"> <label for="j9-F">错误</label>
</div>
<button onclick="checkSingle('judge9', 'j9-F', '解析：虽然增加隐藏层数可以提升模型的表达能力，但过多的层数可能导致训练困难、过拟合等问题，并不一定带来更好的性能。')">提交答案</button>
<div id="res-judge9" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 10. 卷积神经网络（CNN）主要用于处理图像数据。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge10" id="j10-T" value="正确"> <label for="j10-T">正确</label><br>
  <input type="radio" name="judge10" id="j10-F" value="错误"> <label for="j10-F">错误</label>
</div>
<button onclick="checkSingle('judge10', 'j10-T', '解析：CNN 的设计初衷是为了处理图像数据，通过卷积操作提取局部特征，因此在图像识别、目标检测等领域广泛应用。')">提交答案</button>
<div id="res-judge10" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 11. 反向传播算法是神经网络训练的核心算法之一。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge11" id="j11-T" value="正确"> <label for="j11-T">正确</label><br>
  <input type="radio" name="judge11" id="j11-F" value="错误"> <label for="j11-F">错误</label>
</div>
<button onclick="checkSingle('judge11', 'j11-T', '解析：反向传播算法通过计算损失函数相对于参数的梯度，指导神经网络的参数更新，是训练多层神经网络的关键技术。')">提交答案</button>
<div id="res-judge11" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 12. 深度学习模型在小规模数据集上的表现通常优于传统机器学习模型。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge12" id="j12-T" value="正确"> <label for="j12-T">正确</label><br>
  <input type="radio" name="judge12" id="j12-F" value="错误"> <label for="j12-F">错误</label>
</div>
<button onclick="checkSingle('judge12', 'j12-F', '解析：深度学习模型通常需要大量数据才能发挥其优势，在小规模数据集上容易过拟合，表现可能不如传统机器学习模型。')">提交答案</button>
<div id="res-judge12" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 22. 梯度下降法总是能找到全局最优解。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge22" id="j22-T" value="正确"> <label for="j22-T">正确</label><br>
  <input type="radio" name="judge22" id="j22-F" value="错误"> <label for="j22-F">错误</label>
</div>
<button onclick="checkSingle('judge22', 'j22-F', '解析：梯度下降法可能陷入局部最优解，无法保证找到全局最优解。')">提交答案</button>
<div id="res-judge22" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 23. 梯度方向是函数值变化最快的方向。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="radio" name="judge23" id="j23-T" value="正确"> <label for="j23-T">正确</label><br>
  <input type="radio" name="judge23" id="j23-F" value="错误"> <label for="j23-F">错误</label>
</div>
<button onclick="checkSingle('judge23', 'j23-T', '解析：梯度方向是函数在某一点上变化最快的方向，梯度下降法正是利用这一点进行参数更新。')">提交答案</button>
<div id="res-judge23" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


## 四、填空题（可输入文本，提交后显答案）
### 13. 神经网络的基本组成单元是______，它由输入、权重、偏置、求和函数和______等部分构成。
<div style="margin: 10px 0; padding-left: 20px;">
  <!-- 修复：输入框可点击，id唯一 -->
  <input type="text" id="fill13" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="答案用逗号分隔，如“xx, xx”">
</div>
<button onclick="checkFill('fill13', '神经元,激活函数', '解析：神经元是神经网络的基本组成单元，其结构包括输入、权重、偏置、求和函数和激活函数，用于模拟生物神经元的功能。')">提交答案</button>
<div id="res-fill13" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 14. 卷积神经网络（CNN）主要包括卷积层、______和全连接层三个核心部分。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill14" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="填写单个答案">
</div>
<button onclick="checkFill('fill14', '池化层', '解析：CNN 的基本结构包括卷积层、池化层和全连接层，分别用于特征提取、特征压缩和最终分类。')">提交答案</button>
<div id="res-fill14" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 15. 在神经网络中，______函数用于衡量预测值与真实值之间的差距，常见的有均方误差和______损失。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill15" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="答案用逗号分隔，如“xx, xx”">
</div>
<button onclick="checkFill('fill15', '损失,交叉熵', '解析：损失函数用于量化模型预测与真实值之间的差距，是训练神经网络的重要指标。')">提交答案</button>
<div id="res-fill15" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


### 16. 反向传播算法通过计算损失函数相对于参数的______，指导神经网络的参数更新。
<div style="margin: 10px 0; padding-left: 20px;">
  <input type="text" id="fill16" style="width: 400px; padding: 6px; border: 1px solid #ccc;" placeholder="填写单个答案">
</div>
<button onclick="checkFill('fill16', '梯度', '解析：反向传播算法利用梯度下降法，根据损失函数的梯度调整神经网络的参数，以最小化误差。')">提交答案</button>
<div id="res-fill16" style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;"></div>


## 五、论述题（点击查看答案）
### 17. 请简述神经网络与深度学习的关系。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong>答案</strong>：神经网络是深度学习的基础，深度学习则是神经网络的进一步发展。深度学习通过构建多层神经网络，实现了对数据的自动特征提取和复杂模式识别，是当前人工智能领域的重要技术。<br><br>
    <strong>解析</strong>：神经网络为深度学习提供了结构基础，而深度学习则通过增加网络深度和引入新技术，提升了模型的表达能力和应用效果。
  </div>
</details>


### 18. 请说明卷积神经网络（CNN）在图像识别中的优势。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong>答案</strong>：CNN 通过卷积操作提取图像的局部特征，结合池化层进行特征压缩，能够高效地处理高维图像数据，同时减少参数数量，提高模型的泛化能力。<br><br>
    <strong>解析</strong>：CNN 的局部感受野和权值共享机制使其在图像识别任务中表现优异，尤其适合处理具有空间结构的数据。
  </div>
</details>


### 19. 请解释什么是激活函数及其在神经网络中的作用。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong>答案</strong>：激活函数是神经网络中引入非线性的关键组件，其作用是将神经元的线性输出转换为非线性输出，使模型能够拟合复杂的数据分布。<br><br>
    <strong>解析</strong>：如果没有激活函数，无论神经网络有多少层，其整体仍然是一个线性模型，无法处理复杂的数据模式。
  </div>
</details>


### 20. 请简述反向传播算法的原理。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong>答案</strong>：反向传播算法通过计算损失函数相对于网络参数的梯度，从输出层向输入层逐层传播误差，利用梯度下降法更新参数，以最小化损失函数。<br><br>
    <strong>解析</strong>：反向传播是训练多层神经网络的核心算法，它使得神经网络能够通过误差反馈不断优化自身的参数。
  </div>
</details>


### 21. 请简述梯度下降法的基本思想。
<details style="margin: 10px 0; padding: 8px; background: #f5f5f5; border-radius: 4px;">
  <summary style="cursor: pointer; font-weight: bold;">点击查看答案</summary>
  <div style="margin-top: 8px; padding-top: 8px; border-top: 1px dashed #ccc;">
    <strong>答案</strong>：梯度下降法的基本思想是通过计算损失函数的梯度，沿着梯度的反方向逐步更新参数，以最小化损失函数。<br><br>
    <strong>解析</strong>：梯度下降法的核心在于利用梯度信息指导参数更新，从而逐步逼近最优解。
  </div>
</details>


<!-- 核心判分函数（确保能定位到所有元素） -->
<script>
// 单选题/判断题判分（修复元素定位）
function checkSingle(questionName, correctId, explanation) {
  // 精准定位当前题的选中选项
  const selected = document.querySelector(`input[name="${questionName}"][type="radio"]:checked`);
  const resDiv = document.getElementById(`res-${questionName}`);
  
  if (!selected) {
    resDiv.innerHTML = "<span style='color: #ff7f0e;'>请先选择一个选项再提交！</span>";
    return;
  }
  
  // 对比选中选项的id与正确答案id
  if (selected.id === correctId) {
    resDiv.innerHTML = `<span style='color: #2ca02c;'>✅ 回答正确！</span><br>${explanation}`;
  } else {
    const correctLabel = document.querySelector(`label[for="${correctId}"]`).textContent;
    resDiv.innerHTML = `<span style='color: #d62728;'>❌ 回答错误！</span><br>正确答案：${correctLabel}<br>${explanation}`;
  }
}

// 多选题判分（修复多选逻辑）
function checkMulti(questionName, correctIds, explanation) {
  // 获取当前题所有选中的复选框
  const selected = Array.from(document.querySelectorAll(`input[name="${questionName}"][type="checkbox"]:checked`)).map(el => el.id);
  const resDiv = document.getElementById(`res-${questionName}`);
  
  if (selected.length === 0) {
    resDiv.innerHTML = "<span style='color: #ff7f0e;'>请至少选择一个选项再提交！</span>";
    return;
  }
  
  // 排序后对比（避免选择顺序影响结果）
  const isCorrect = JSON.stringify(selected.sort()) === JSON.stringify(correctIds.sort());
  const correctLabels = correctIds.map(id => document.querySelector(`label[for="${id}"]`).textContent).join("、");
  
  resDiv.innerHTML = isCorrect ? 
    `<span style='color: #2ca02c;'>✅ 回答正确！</span><br>${explanation}` : 
    `<span style='color: #d62728;'>❌ 回答错误！</span><br>正确答案：${correctLabels}<br>${explanation}`;
}

// 填空题判分（修复输入框取值）
function checkFill(inputId, correctAnswer, explanation) {
  // 精准定位当前题的输入框
  const inputEl = document.getElementById(inputId);
  const userAnswer = inputEl.value.trim();
  const resDiv = document.getElementById(`res-${inputId}`);
  
  if (!userAnswer) {
    resDiv.innerHTML = "<span style='color: #ff7f0e;'>请先填写答案再提交！</span>";
    return;
  }
  
  // 忽略空格和大小写，兼容多种输入格式
  const normalize = str => str.replace(/\s+/g, '').toLowerCase();
  if (normalize(userAnswer) === normalize(correctAnswer)) {
    resDiv.innerHTML = `<span style='color: #2ca02c;'>✅ 回答正确！</span><br>${explanation}`;
  } else {
    resDiv.innerHTML = `<span style='color: #d62728;'>❌ 回答错误！</span><br>正确答案：${correctAnswer}<br>${explanation}`;
  }
}
</script>
