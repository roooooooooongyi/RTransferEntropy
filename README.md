# RTransferEntropy
学习RTransferEntropy
通过Shannon和Renyi的**传递熵**来测度时间序列的信息流。
## 1. 高效的计算两个时间序列之间的传递熵
---
（1）用法
calc_ete(x, y, lx = 1, ly = 1, q = 0.1, entropy = "Shannon",
shuffles = 100, type = "quantiles", quantiles = c(5, 95),
bins = NULL, limits = NULL, burn = 50, seed = NULL)

（2）参数



## 2. 计算两个时间序列之间的传递熵
---
（1）用法
calc_te(x, y, lx = 1, ly = 1, q = 0.1, entropy = "Shannon",
shuffles = 100, type = "quantiles", quantiles = c(5, 95),
bins = NULL, limits = NULL, burn = 50, seed = NULL)


（2）参数


## 3. 估计两个时间序列的Shannon和Renyi传递熵
---
（1）用法
transfer_entropy(x, y, lx = 1, ly = 1, q = 0.1,
entropy = "Shannon", shuffles = 100, type = "quantiles",
quantiles = c(5, 95), bins = NULL, limits = NULL, nboot = 300,
burn = 50, quiet = NULL, seed = NULL)


（2）参数



## 4. 从传递熵中抽取系数矩阵
---
（1）用法
coef(object, ...)

（2）参数

## 5. 判断一个对象是否是传递熵对象（transfer_entropy）

即判断一个对象是否是calc_ete()或者calc_te（）返回的结果

---
（1）用法
is.transfer_entropy(x)

（2）参数

## 6. 打印传递熵对象（transfer_entropy）的结果
---
（1）用法
print(x, digits = 4, boot = TRUE, probs = c(0, 0.25, 0.5, 0.75, 1), ...)

（2）参数


## 7. 设置是否隐藏计算过程
---
（1）用法
set_quiet(quiet)

（2）参数

## 8. transfer_entropy对象的总结结果（R语言的老套路）
---
（1）用法
summary(object, digits = 4, probs = c(0,
0.25, 0.5, 0.75, 1), ...)

（2）参数




stocks 股票数据集
A dataset containing the daily stock returns for 10 stocks and the S&P 500 market returns for the
time-period 2000-01-04 until 2017-12-29

---
（1）用法
set_quiet(quiet)

（2）参数








参考
1. https://cran.r-project.org/web/packages/RTransferEntropy/vignettes/transfer-entropy.html
2. https://cran.r-project.org/web/packages/RTransferEntropy/RTransferEntropy.pdf
