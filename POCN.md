# POCN(投影)
## 1. 通用

$$
\forall\alpha,\beta\in\mathrm{Exp}\Rightarrow \alpha+\beta\in \mathrm{Exp}\\
\psi_X(0)=B\\
\psi_X(\alpha+1)=\psi_X(\alpha)*\omega\\
\psi_X(h(Y))=\psi_X(\alpha \rightarrow h(\psi_Y(\alpha))fp.) ,\lnot(isProjection(h(Y),X)\lor\exist\gamma(\gamma<X\land f(\psi_\gamma(g(X)))=h(X)))
\\
\psi_X(\alpha)=sup\Set{\psi_X(\beta)\mid \beta \in \alpha\land(\lnot \exist \mu(\alpha=\mu+1))},isProjection(\alpha,X),\alpha\in\mathrm{Exp}\\
$$
## 2. n阶投影

记$n-P$为$n$阶投影的类。
记$0-P$为$\Pi_0$。
$$
\psi_{n-P\,\mathrm{aft}\alpha}(0)=(n-1)-P\,\mathrm{aft}\alpha \\
isProjection(\alpha,X)\iff X\in n-P\land\exist\beta((\exist m(m<n,\beta\in m-P\cap (m+1)-P\,\mathrm{aft}\,X \land\alpha=h(\beta)))\land(\lnot \exist\gamma(\gamma<X\land f(\psi_\gamma(g(\beta)))=h(\beta))))
$$
## 3. 向上投影

记 $ S_n=n \mathrm{th} (1,0)-P,\sigma \alpha =\beta \mathrm{th} (\#,\mu @ 1,\nu+1@ 0)-P, \theta \alpha =\beta \mathrm{th} (\#,\mu+1@ 1,\nu @ 0)-P ,\alpha=\beta\mathrm{th} (\#,\mu @ 1,\nu @ 0)-P $
$$
\psi_{\sigma^b\theta^aS_n}(0)=\begin{cases}
\sigma^{b-1}\theta^aS_{\sigma^b\theta^aS_{n-1}+1} &n>1\land isSucc(n)\land isSucc(b)\\
\sigma^{\theta^aS_{n-1}+1}\theta^{a-1}S&n>1\land isSucc(n)\land isSucc(a)\land b=0\\
\sigma^{b-1}\theta^aS &n=1\land isSucc(n)\land isSucc(b)\\
\sigma\theta^{a-1}S&n=1\land isSucc(n)\land isSucc(a)\land b=0\\
S_{n-1}&n>1\land isSucc(n)\land a,b=0\\
1&n=1 a,b=0
\end{cases}
$$
$$
isProjection(\alpha,X)\iff ... %未完待续
$$