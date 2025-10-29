# 神经网络与深度学习交互式题库（23题）
> 说明：选选项/填答案后点“检查”，样式已适配GitHub Pages

<!-- 仅保留基础全局样式，避免复杂选择器 -->
<style>
/* 基础样式：确保所有平台兼容 */
body { font-family: Arial, sans-serif; max-width: 800px; margin: 0 auto; padding: 20px; }
.opt { margin: 10px 0; } /* 选项容器 */
.res { margin: 10px 0; padding: 8px; border-radius: 4px; } /* 结果容器 */
.btn { padding: 6px 12px; background: #0969da; color: white; border: none; border-radius: 4px; cursor: pointer; margin: 8px 0; }
.txt-input { padding: 6px; margin: 0 5px 8px 0; border: 1px solid #ddd; border-radius: 4px; }
.txtarea { width: 100%; min-height: 100px; padding: 8px; border: 1px solid #ddd; border-radius: 4px; margin: 8px 0; box-sizing: border-box; }
.correct { color: #1a7f37; font-weight: bold; }
.incorrect { color: #cf222e; font-weight: bold; }
</style>

## 一、单选题（可选择+检查）
### 1. 神经网络输入层的主要作用是？
<div class="opt">
  <input type="radio" name="q1" id="q1-A" value="A" style="margin-right: 8px;">
  <label for="q1-A">A. 对数据进行非线性变换</label>
</div>
<div class="opt">
  <input type="radio" name="q1" id="q1-B" value="B" style="margin-right: 8px;">
  <label for="q1-B">B. 对数据进行归一化处理</label>
</div>
<div class="opt">
  <input type="radio" name="q1" id="q1-C" value="C" style="margin-right: 8px;">
  <label for="q1-C">C. 接收外部输入的数据</label>
</div>
<div class="opt">
  <input type="radio" name="q1" id="q1-D" value="D" style="margin-right: 8px;">
  <label for="q1-D">D. 对数据进行降维处理</label>
</div>
<button class="btn" onclick="checkSingle('q1', 'C', 'q1-res')">检查答案</button>
<div id="q1-res" class="res"></div>


### 2. 卷积神经网络（CNN）最突出的特点是？
<div class="opt">
  <input type="radio" name="q2" id="q2-A" value="A" style="margin-right: 8px;">
  <label for="q2-A">A. 使用全连接层提取全局特征</label>
</div>
<div class="opt">
  <input type="radio" name="q2" id="q2-B" value="B" style="margin-right: 8px;">
  <label for="q2-B">B. 通过卷积操作提取局部特征</label>
</div>
<div class="opt">
  <input type="radio" name="q2" id="q2-C" value="C" style="margin-right: 8px;">
  <label for="q2-C">C. 使用递归结构处理序列数据</label>
</div>
<div class="opt">
  <input type="radio" name="q2" id="q2-D" value="D" style="margin-right: 8px;">
  <label for="q2-D">D. 采用强化学习方式训练</label>
</div>
<button class="btn" onclick="checkSingle('q2', 'B', 'q2-res')">检查答案</button>
<div id="q2-res" class="res"></div>


## 二、填空题（可填写+检查）
### 3. 神经网络的基本组成单元是______，它由输入、权重、偏置、求和函数和______等部分构成。
<br>
<input type="text" class="txt-input" id="fill3-1" placeholder="第一个空（如：神经元）" style="width: 200px;">
<input type="text" class="txt-input" id="fill3-2" placeholder="第二个空（如：激活函数）" style="width: 200px;">
<br>
<button class="btn" onclick="checkFill(['神经元','激活函数'], ['fill3-1','fill3-2'], 'fill3-res')">检查答案</button>
<div id="fill3-res" class="res"></div>


### 4. 卷积神经网络（CNN）主要包括卷积层、______和全连接层三个核心部分。
<br>
<input type="text" class="txt-input" id="fill4" placeholder="填写答案（如：池化层）" style="width: 300px;">
<br>
<button class="btn" onclick="checkFill(['池化层'], ['fill4'], 'fill4-res')">检查答案</button>
<div id="fill4-res" class="res"></div>


## 三、论述题（可填写+看参考）
### 5. 请简述神经网络与深度学习的关系。
<br>
<textarea class="txtarea" id="essay5" placeholder="请在此输入你的答案..."></textarea>
<br>
<details style="margin: 10px 0;">
  <summary style="cursor: pointer; color: #0969da; font-weight: 500;">点击查看参考答案</summary>
  <div style="margin: 10px 0 0 15px; line-height: 1.6;">
    1. 基础关系：神经网络是深度学习的“底层框架”，深度学习是神经网络的“深度化升级”；<br>
    2. 神经网络特点：包含输入层、隐藏层、输出层+激活函数，能解决简单非线性问题（如异或）；<br>
    3. 深度学习特点：通过增加隐藏层数量（构建深度网络），结合卷积、循环结构，实现“自动特征提取”，可处理图像、语音等复杂数据（如人脸识别）。
  </div>
</details>


## 四、交互脚本（极简逻辑，确保运行）
<script>
// 单选题检查：兼容所有浏览器
function checkSingle(qName, correctAns, resId) {
  const selected = document.querySelector(`input[name="${qName}"]:checked`);
  const resEl = document.getElementById(resId);
  
  if (!selected) {
    resEl.innerHTML = "请先选择一个选项！";
    resEl.style.background = "#fef2f2";
    return;
  }
  
  if (selected.value === correctAns) {
    resEl.innerHTML = `<span class="correct">✅ 回答正确！</span><br>解析：${getExp(qName)}`;
    resEl.style.background = "#f0fdf4";
  } else {
    resEl.innerHTML = `<span class="incorrect">❌ 回答错误！正确答案是 ${correctAns}</span><br>解析：${getExp(qName)}`;
    resEl.style.background = "#fef2f2";
  }
}

// 填空题检查：兼容大小写
function checkFill(correctArr, inputIds, resId) {
  const userAns = inputIds.map(id => document.getElementById(id).value.trim().toLowerCase());
  const correctLow = correctArr.map(a => a.toLowerCase());
  const resEl = document.getElementById(resId);
  
  if (userAns.includes("")) {
    resEl.innerHTML = "请填写所有空的答案！";
    resEl.style.background = "#fef2f2";
    return;
  }
  
  const allCorrect = userAns.every((a, i) => a === correctLow[i]);
  if (allCorrect) {
    resEl.innerHTML = `<span class="correct">✅ 回答正确！</span><br>正确答案：${correctArr.join("、")}`;
    resEl.style.background = "#f0fdf4";
  } else {
    resEl.innerHTML = `<span class="incorrect">❌ 回答错误！</span><br>正确答案：${correctArr.join("、")}`;
    resEl.style.background = "#fef2f2";
  }
}

// 解析库：极简定义
function getExp(qName) {
  const exps = {
    "q1": "输入层仅负责接收外部数据（如图像、文本），不做数据处理。",
    "q2": "CNN靠卷积核提取图像局部特征，权值共享减少参数，适配图像结构。"
  };
  return exps[qName] || "暂无解析";
}
</script>
