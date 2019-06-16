## 传递熵    
**传递熵**是用来测量两个随机过程的信息传递量。在已知Y的过去值和X的过去值的情况下，来减少Y值未来的不确定度，传递熵常常被用于估计社交网络中的社交影响。
两个随机过程X,Y，如果用**Shannon‘s entropy**来刻度信息量，表示为H(X)，用H(X|Y)表示为**conditional Shannon's entropy**那么传递熵**transfer entropy**可以被表示如下：

<img src="http://chart.googleapis.com/chart?cht=tx&chl= T_{X->Y}=H(Y_t|Y_{t-1:t-L})-H(Y_t|Y_{t-1:t-L}, X_{t-1:t-L})" style="border:none;">

此时，**transfer entropy**等价于一个特定的**partial mutual information**：
<img src="http://chart.googleapis.com/chart?cht=tx&chl= T_{m->n}=I(A_m,B_n|A_n)" style="border:none;">

需要说明的是：对**向量自回归的情况**，transfer entropy与**Grange causality**
等价，因此当Grange causality假设不满足的时候，transfer entropy就可以展现优势了，比如非线性信号。本质上来说，传递熵其实就是一个条件分布带来的探测到
时间序列间的不对称性，这个信息由Y到X和由X到Y是不对称，这种不对称就带来了，驱动和响应的关系的建立。

discussion of discretising stock price: [6][20]            
There is a large number of estimators of entropy, for details please see Refs. [56][60].       
使用Schurmann-Grassberger来估计entropy，Schurmann-Grassberger是一个Bayesian parametric procedure,假设样本来自Dirichlet distribution。










