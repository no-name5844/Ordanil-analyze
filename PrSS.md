# PrSS
# 1.定义
PrSS是序数记号中序列记号中的自然数序列中的阶差型记号。极限表达式为$0,1,2,\dots,n$
该记号在标准型下满足字典序比较
对于$A=(a_1,a_2,...,a_n)$一定满足:
  1. $a_i \in \mathbb{N}$
  2. $a_{i+1} - a_i \le 1$ 
  3. $a_1 = 0$
  4. $a_{i+1} - a_i = 0 \Rightarrow a_{i+2} - a_{i+1} \le 0$
   
对于$A=(a_1,a_2,...,a_n)$ 中的元素 $a_i$ 有 :
  1. 列标为$i$
  2. $i th A=a_i$
# 2.展开
## 2.1 辅助函数
1. $ (a_1,a_2,\dots,a_n)\oplus(b_1,b_2,\dots,b_n)=(a_1,a_2,\dots,a_n,b_1,b_2,\dots,b_n)$
2. $A \bigoplus^n_{i=a} f(i)=(A \bigoplus^{n-1}_{i=a} f(i)) \oplus f(n)$
## 2.2 expand 函数
对于$A=()$中:
$$
expand(A,m)=()\\
$$
对于$A=(a_1,a_2,...,a_n,0)$中:<!-- A is Successor -->
$$
expand(A,m)=(a_1,a_2,...,a_n)\\
$$
对于$A=(a_1,a_2,...,a_n)$以上不满足时:
  - 设 $br=max\{n-i\mid a_(n-i)<a_n\}$ 即从右到左的寻找比a_n小的第一个元素的列标。$L=n-br$ 
  $$
  G=(a_1,a_2,...,a_{br-1})\\
  B=(a_{br},...,a_{n-1})\\
  expand(A,m)=G(\bigoplus^m_{i=0} B)
  $$

