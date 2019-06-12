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


## 3. 从传递熵中抽取系数矩阵
---
（1）用法
coef(object, ...)

（2）参数







参考
1. https://cran.r-project.org/web/packages/RTransferEntropy/vignettes/transfer-entropy.html
2. https://cran.r-project.org/web/packages/RTransferEntropy/RTransferEntropy.pdf
