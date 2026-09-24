![](./Notations.md#1 Ordinal Notations) 
# PrSS
# 1.定义
PrSS是序数记号中序列记号中的自然数序列中的阶差型记号。极限表达式为$0,1,2,\dots,n$
该记号在标准型下满足字典序比较
$$
PrSS:\mathcal O\\
Zero=()\\
(a_1,a_2,...,a_n)\oplus(b_1,b_2,...,b_m)=(a_1,a_2,...,a_n,b_1,b_2,...,b_m)\\
\forall a\in Exp\setminus Zero\to a_1=0\\
\forall n\in\mathbb{N}\to {i}_{i\in n}\in Exp\\
\forall a\in Exp(\exist b(a=b\oplus (0)))\Leftrightarrow a\in Succ,Prec(a)=b\\
Limit=Exp\setminus (Succ\cup Zero)\\
\forall a\in Succ\in\mathbb{N}\to Prec(a)\in Exp\\
\forall a\in Limit\forall n\in\mathbb{N}\to a[n]\in Exp\\
a[0]=\{a_i\}_{i\in len(a)\setminus0}\oplus(a_{len(a)}-1)\\
a[n+1]=a[n]\oplus\{a_i\}_{i\in len(a)\setminus n}\oplus(a_{len(a)}-1),\exist n \in len(a)(n-min\Set{i\mid a_{len(a)}>a_{len(a)-i}})
$$
