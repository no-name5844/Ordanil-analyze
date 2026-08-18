# 1 zahin's weak-Veblen-like notation  (zahin的类弱veblen记号) by zahin
## 1.1 定义
是不封闭，是序数记号中的序列记号。极限表达式为$(0),(1@(0)),(1@(1@(0))),\dots$
该记号在标准型下满足字典序比较
对于 $ A= (a_1@b_1,a_2@b_2,\dots,a_n@b_n)$ 一定满足：
1. $a_i , b_i \in On.$
2. $b_i > b_{i+1}$
## 1.2 展开
## 1.2.1 expand 函数
对于$A=(0)$
$$
expand(A,n)=n\\
$$
对于$A=(0@b_1,\#)$
$$
expand(A,n)=(\#)\\
$$
对于$A=(\#,(a+1)@0)$
$$
expand(A,n)=\begin{cases}
(\#,a@0)+1 & n=0\\
(\#,a@0)^{expand(A,m)} & n=m+1
\end{cases}\\
$$
对于$A=(\#,(a+1)@(b+1))$
$$
expand(A,n)=\begin{cases}
(\#,a@(b+1))+1 & n=0\\
(\#,a@(b+1),expand(A,m)@b) & n=m+1
\end{cases}\\
$$
对于$A=(\#,(a+1)@b)(!\exists c(b=c+1))$
$$
expand(A,n)=(\#,a@b,1@expand(b,n))
$$
对于$A=(\#,a@b)(!\exists c(a=c+1))$
$$
expand(A,n)=(\#,expand(a,n)@b)
$$
# 1.3 compare 函数
对于$A=(a_1@i_1,a_2@i_2,\dots,a_n@i_n),B=(b_1@j_1,b_2@j_2,\dots,b_m@j_m)$
$$
is\_ equal(A,B)=\begin{cases}
true & a_1=b_1,i_1=j_1,n=m=1\\
false & a_1\neq b_1,i_1\neq j_1\\
false & n\neq m\\
false & i_1\neq j_1\\
false & a_1\neq b_1,i_1=j_1\\
is\_ equal((a_2@i_2,\dots,a_n@i_n),(b_2@j_2,\dots,b_m@j_m)) & n,m> 1\\
\end{cases}
$$
$$
is\_ greater(A,B)=\begin{cases}
true & i_1>j_1\\
true & a_1> b_1,i_1=j_1\\
true & n>m=1,a_1=b_1\\
false & i_1\le j_1\\
false & a_1\le b_1,i_1=j_1\\
false & n=1\ge m,a_1=b_1\\
is\_ greater((a_2@i_2,\dots,a_n@i_n),(b_2@j_2,\dots,b_m@j_m)) & n,m> 1\\
\end{cases}
$$
$$
compare(A,B)=\begin{cases}
1 & is\_ greater(A,B)\\
0 & is\_ equal(A,B)\\
-1 & \lnot (is\_ greater(A,B) \land is\_ equal(A,B))\\
\end{cases}\\
$$
