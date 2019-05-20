# textClassify-keras
## 模型
### 1 FastText
FastText 在论文 [Bag of Tricks for Efficient Text Classification](https://arxiv.org/pdf/1607.01759.pdf) 中被提出。
#### 1.1 论文的描述
<p align="center">
  <img src="image/FastText.png">
</p>

1. Using a look-up table, **bags of n-gram** convert to **word representations**.
2. Word representations are **averaged** into a text representation, which is a hidden variable.
3. Text representation is in turn fed to a **linear classifier**.
4. Using the **softmax** function to compute the probability distribution over the predefined classes.（使用softmax函数计算预定义类的概率分布）

#### 1.2 此处的实现
FastText 的网络结构：
test