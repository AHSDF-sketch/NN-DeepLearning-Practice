# 神经网络与深度学习题库（完全正常版）

## 一、单选题（点击选项可选中，提交显结果）
### 1. 神经网络输入层的主要作用是？
- <input type="radio" name="q1" id="q1-A"> <label for="q1-A">A. 对数据进行非线性变换</label><br>
- <input type="radio" name="q1" id="q1-B"> <label for="q1-B">B. 对数据进行归一化处理</label><br>
- <input type="radio" name="q1" id="q1-C"> <label for="q1-C">C. 接收外部输入的数据</label><br>
- <input type="radio" name="q1" id="q1-D"> <label for="q1-D">D. 对数据进行降维处理</label><br>
<button onclick="checkSingle('q1', 'q1-C')">提交答案</button>
<div id="ans-q1"></div>


### 2. 卷积神经网络（CNN）最突出的特点是？
- <input type="radio" name="q2" id="q2-A"> <label for="q2-A">A. 使用全连接层提取全局特征</label><br>
- <input type="radio" name="q2" id="q2-B"> <label for="q2-B">B. 通过卷积操作提取局部特征</label><br>
- <input type="radio" name="q2" id="q2-C"> <label for="q2-C">C. 使用递归结构处理序列数据</label><br>
- <input type="radio" name="q2" id="q2-D"> <label for="q2-D">D. 采用强化学习方式训练</label><br>
<button onclick="checkSingle('q2', 'q2-B')">提交答案</button>
<div id="ans-q2"></div>


## 二、多选题（点击选项可多选，提交显结果）
### 3. 神经网络的基本组成部分包括？
- <input type="checkbox" name="q3" id="q3-A"> <label for="q3-A">A. 输入层</label><br>
- <input type="checkbox" name="q3" id="q3-B"> <label for="q3-B">B. 隐藏层</label><br>
- <input type="checkbox" name="q3" id="q3-C"> <label for="q3-C">C. 输出层</label><br>
- <input type="checkbox" name="q3" id="q3-D"> <label for="q3-D">D. 激活函数</label><br>
- <input type="checkbox" name="q3" id="q3-E"> <label for="q3-E">E. 数据库</label><br>
<button onclick="checkMulti('q3', ['q3-A','q3-B','q3-C','q3-D'])">提交答案</button>
<div id="ans-q3"></div>


## 三、判断题（点击选项可选中，提交显结果）
### 4. 神经网络隐藏层数越多，表达能力一定越强。
- <input type="radio" name="q4" id="q4-T"> <label for="q4-T">正确</label><br>
- <input type="radio" name="q4" id="q4-F"> <label for="q4-F">错误</label><br>
<button onclick="checkSingle('q4', 'q4-F')">提交答案</button>
<div id="ans-q4"></div>


## 四、填空题（输入后提交，显结果）
### 5. 神经网络的基本组成单元是______，它由输入、权重、偏置、求和函数和______等部分构成。
<input type="text" id="fill5" style="width:300px">
<button onclick="checkFill('fill5', '神经元,激活函数')">提交答案</button>
<div id="ans-fill5"></div>


## 五、论述题（点击展开答案，无乱码）
### 6. 简述神经网络与深度学习的关系。
<details>
  <summary>查看答案</summary>
  神经网络是深度学习的基础，深度学习是神经网络的深化发展。深度学习通过构建多层神经网络，实现自动特征提取，能处理更复杂的数据模式。
</details>


### 7. 说明CNN在图像识别中的优势。
<details>
  <summary>查看答案</summary>
  1. 局部感知：通过卷积核提取图像局部特征（如边缘、纹理）；<br>
  2. 权值共享：大幅减少参数数量，降低过拟合风险；<br>
  3. 池化层：压缩特征维度，增强对图像平移、缩放的鲁棒性。
</details>


<script>
// 单选题/判断题判分函数
function checkSingle(id, correctId) {
  const selected = document.querySelector(`input[name="${id}"]:checked`);
  const ansDiv = document.getElementById(`ans-${id}`);
  if (!selected) {
    ansDiv.innerHTML = "请先选择选项";
    return;
  }
  if (selected.id === correctId) {
    ansDiv.innerHTML = "✅ 正确";
    ansDiv.style.color = "green";
  } else {
    const correctLabel = document.querySelector(`label[for="${correctId}"]`).textContent;
    ansDiv.innerHTML = `❌ 错误，正确答案是${correctLabel}`;
    ansDiv.style.color = "red";
  }
}

// 多选题判分函数
function checkMulti(id, correctIds) {
  const selected = Array.from(document.querySelectorAll(`input[name="${id}"]:checked`)).map(el => el.id);
  const ansDiv = document.getElementById(`ans-${id}`);
  if (selected.length === 0) {
    ansDiv.innerHTML = "请至少选择一项";
    return;
  }
  const isCorrect = JSON.stringify(selected.sort()) === JSON.stringify(correctIds.sort());
  const correctLabels = correctIds.map(id => document.querySelector(`label[for="${id}"]`).textContent).join("、");
  if (isCorrect) {
    ansDiv.innerHTML = "✅ 正确";
    ansDiv.style.color = "green";
  } else {
    ansDiv.innerHTML = `❌ 错误，正确答案是${correctLabels}`;
    ansDiv.style.color = "red";
  }
}

// 填空题判分函数
function checkFill(id, correctAnswer) {
  const input = document.getElementById(id);
  const ans = input.value.trim();
  const ansDiv = document.getElementById(`ans-${id}`);
  if (!ans) {
    ansDiv.innerHTML = "请输入答案";
    return;
  }
  if (ans.toLowerCase() === correctAnswer.toLowerCase()) {
    ansDiv.innerHTML = "✅ 正确";
    ansDiv.style.color = "green";
  } else {
    ansDiv.innerHTML = `❌ 错误，正确答案是${correctAnswer}`;
    ansDiv.style.color = "red";
  }
}
</script>
