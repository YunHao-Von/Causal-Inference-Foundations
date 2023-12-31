# Module2 因果推断假设  
假设海拔和温度的联合密度为$p(a,t)$，则该联合密度的两种表达式如下：  
$$p(a,t) = p(a|t)p(t) =p(t|a)p(a) \tag{1}$$  
第一个式子定义了一个$T → A$的因式分解。第二个分解师对应了一个$A→ T$的因式分解。  
如何确定真正的因果关系呢？  
如果干预A能够改变T，但是对T的干预没有改变A，因此合理的倾向于把$A→ T$作为一个因果结构的描述。  
如果$A→ T$是正确的因果结构，那么：  
+ 原则上可以对A进行局部干预，改变$p(a)$而不改变$p(t|a)$。  
+ $p(a)$和$p(t|a)$是自治的、模块化的或者不变的机制或者世界上的物体。  

在因果分解$p(a,t)=p(t|a)p(a)$中，我们期望条件概率密度$p(t|a)$不提供关于边缘密度函数$p(a)$的信息。


$$A:=N_A \\ T:=f_T(A,N_T)$$
$N_T$和$N_A$是统计独立的噪声，且二者不相关。  
#### 独立机制：系统变量的因果生成过程由互不知晓或者互不影响的自主模块组成。