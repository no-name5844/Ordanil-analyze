# Notations
## 1 Ordinal Notations
### 1.1 定义
$$
\mathcal{O}=(Exp,Zero,Succ,Limit,Prec,FS)\\
Zero\in Exp
Succ \subset Exp\\
Limit \subset Exp\\
Prec: Succ\to Exp\\
FS: Limit*\omega\to Exp\\
Exp=Zero\cup Succ\cup Limit\\
Limit=\Set{\alpha\in Exp\mid\alpha\not\in Zero\cup Succ}\\
FS(\alpha,n)\text{记作}\alpha[n],<\alpha[i]>_{i\in\omega}\text{基本列}\\
\mathcal{F}:Exp \leftrightarrow A \subset On\\
\mathcal{F}(Zero)=0\\
\mathcal{F}(\alpha)=\mathcal{F}(Prec(\alpha))+1,\alpha\in Succ\\
\mathcal{F}(\alpha)=sup\Set{\mathcal{F}(FS(\alpha,i))\mid{i\in\omega}}\alpha\in Limit\land(\forall n\in\omega\forall m\in n)(\mathcal{F}(FS(\alpha,n))>\mathcal{F}(FS(\alpha,m)))  \\
$$
## 2 Large Number Notations
### 2.1 定义
$$
\mathcal{N}=(Exp,FS)\\
\mathbb{N} \subset Exp\\
FS: Exp\to Exp\\
\mathcal{F}:Exp \to \mathbb{N}\\
\mathcal{F}(\alpha)=\alpha,\alpha\in \mathbb{N}\
\mathcal{F}(\alpha)=\mathcal{F}(FS(\alpha)),\alpha\in Exp-\mathbb{N} \\
$$
