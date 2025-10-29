# 神经网络与深度学习题库（无乱码版）

## 一、单选题
### 1. 神经网络输入层的主要作用是？
- [ ] A. 对数据进行非线性变换
- [ ] B. 对数据进行归一化处理
- [ ] C. 接收外部输入的数据
- [ ] D. 对数据进行降维处理

<button onclick="check('q1','C')">提交答案</button>
<div id="ans-q1"></div>


### 2. 卷积神经网络（CNN）最突出的特点是？
- [ ] A. 使用全连接层提取全局特征
- [ ] B. 通过卷积操作提取局部特征
- [ ] C. 使用递归结构处理序列数据
- [ ] D. 采用强化学习方式训练

<button onclick="check('q2','B')">提交答案</button>
<div id="ans-q2"></div>


### 3. 激活函数的作用是？
- [ ] A. 计算神经元之间的权重
- [ ] B. 引入非线性，使模型能拟合复杂函数
- [ ] C. 减少模型训练时间
- [ ] D. 提高模型精度

<button onclick="check('q3','B')">提交答案</button>
<div id="ans-q3"></div>


### 4. 适用于分类任务的损失函数是？
- [ ] A. 均方误差（MSE）
- [ ] B. 交叉熵损失
- [ ] C. 三重态损耗
- [ ] D. 铰链损耗

<button onclick="check('q4','B')">提交答案</button>
<div id="ans-q4"></div>


## 二、多选题
### 5. 神经网络的基本组成部分包括？
- [ ] A. 输入层
- [ ] B. 隐藏层
- [ ] C. 输出层
- [ ] D. 激活函数
- [ ] E. 数据库

<button onclick="checkMulti('q5',['A','B','C','D'])">提交答案</button>
<div id="ans-q5"></div>


### 6. 深度学习相较于传统机器学习的优势是？
- [ ] A. 自动提取特征
- [ ] B. 依赖人工特征工程
- [ ] C. 处理高维数据能力强
- [ ] D. 对数据量需求较低
- [ ] E. 模型泛化能力更强

<button onclick="checkMulti('q6',['A','C','E'])">提交答案</button>
<div id="ans-q6"></div>


## 三、判断题
### 7. 神经网络隐藏层数越多，表达能力一定越强。
- [ ] 正确
- [ ] 错误

<button onclick="check('q7','错误')">提交答案</button>
<div id="ans-q7"></div>


### 8. 卷积神经网络（CNN）主要用于处理图像数据。
- [ ] 正确
- [ ] 错误

<button onclick="check('q8','正确')">提交答案</button>
<div id="ans-q8"></div>


## 四、填空题
### 9. 神经网络的基本组成单元是______，它由输入、权重、偏置、求和函数和______等部分构成。
<input type="text" id="fill9" style="width:300px">
<button onclick="checkFill('fill9','神经元,激活函数')">提交答案</button>
<div id="ans-fill9"></div>


### 10. 卷积神经网络主要包括卷积层、______和全连接层三个核心部分。
<input type="text" id="fill10" style="width:300px">
<button onclick="checkFill('fill10','池化层')">提交答案</button>
<div id="ans-fill10"></div>


## 五、论述题
### 11. 简述神经网络与深度学习的关系。
<details>
  <summary>查看答案</summary>
  神经网络是深度学习的基础，深度学习是神经网络的深化发展。深度学习通过构建多层神经网络，实现自动特征提取，处理更复杂的数据。
</details>


### 12. 说明CNN在图像识别中的优势。
<details>
  <summary>查看答案</summary>
  1. 局部感知：通过卷积核提取局部特征；2. 权值共享：减少参数数量；3. 池化层：增强对图像变换的鲁棒性。
</details>


<script>
// 单选题/判断题判分
function check(id, correct) {
  const options = document.querySelectorAll(`[id^="${id}"] + label`);
  let selected = null;
  options.forEach(option => {
    if (option.previousElementSibling.checked) {
      selected = option.textContent.trim().split('.')[0];
    }
  });
  const ansDiv = document.getElementById(`ans-${id}`);
  if (!selected) {
    ansDiv.innerHTML = "请先选择选项";
    return;
  }
  if (selected === correct) {
    ansDiv.innerHTML = "✅ 正确";
    ansDiv.style.color = "green";
  } else {
    ansDiv.innerHTML = `❌ 错误，正确答案是${correct}`;
    ansDiv.style.color = "red";
  }
}

// 多选题判分
function checkMulti(id, correct) {
  const options = document.querySelectorAll(`[name="${id}"]:checked`);
  const selected = Array.from(options).map(el => el.nextElementSibling.textContent.trim().split('.')[0]);
  const ansDiv = document.getElementById(`ans-${id}`);
  if (selected.length === 0) {
    ansDiv.innerHTML = "请至少选择一项";
    return;
  }
  const isCorrect = selected.sort().join(',') === correct.sort().join(',');
  if (isCorrect) {
    ansDiv.innerHTML = "✅ 正确";
    ansDiv.style.color = "green";
  } else {
    ansDiv.innerHTML = `❌ 错误，正确答案是${correct.join(',')}`;
    ansDiv.style.color = "red";
  }
}

// 填空题判分
function checkFill(id, correct) {
  const input = document.getElementById(id);
  const ans = input.value.trim();
  const ansDiv = document.getElementById(`ans-${id}`);
  if (!ans) {
    ansDiv.innerHTML = "请输入答案";
    return;
  }
  if (ans.toLowerCase() === correct.toLowerCase()) {
    ansDiv.innerHTML = "✅ 正确";
    ansDiv.style.color = "green";
  } else {
    ansDiv.innerHTML = `❌ 错误，正确答案是${correct}`;
    ansDiv.style.color = "red";
  }
}
</script>
