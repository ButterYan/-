# Gamma与Beta函数

对于Gamma函数，我们首先考虑一族积分：$\int_0^{+\infty}x^{\alpha-1}e^{-x}dx$ 。随着 $\alpha$ 的变化，积分的特性也发生变化，为了检验这个积分的敛散性，我们可以把积分区间分成 $[0,1]$ 和 $[1,+\infty)$ 两部分。即 $\int_0^{+\infty}x^{\alpha-1}e^{-x}dx=\int_0^1x^{\alpha-1}e^{-x}dx+\int_1^{+\infty}x^{\alpha-1}e^{-x}dx$ 。

注意到当 $\alpha<1$ 时，$\underset{x\rightarrow 0^+}{\lim} x^{\alpha-1}e^{-x}=\infty$ ，此时区间 $[0,1]$ 上是瑕积分。我们首先讨论它的敛散性：

当 $\alpha<0$ 时，$\int_0^1x^{\alpha-1}e^{-x}dx\ge\int_0^1x^{\alpha-1}e^{-1}dx=\frac{1}{\alpha e}x^\alpha|^1_0=\frac{1}{\alpha e}(1-\underset{x\rightarrow 0^+}{\lim} x^\alpha)$ ；由于极限 $\underset{x\rightarrow 0^+}{\lim} x^\alpha$ 不收敛，此时积分无意义。

当 $\alpha=0$ 时，$\int_0^1x^{\alpha-1}e^{-x}dx\ge\int_0^1x^{-1}e^{-1}dx=\frac{1}{e}\ln x|^1_0=-\frac{1}{e}\underset{x\rightarrow 0^+}{\lim}\ln x$ ；由于极限 $ \underset{x\rightarrow 0^+}{\lim}\ln x$不收敛，此时积分无意义。

当 $\alpha>0$ 时，$\int_0^1x^{\alpha-1}e^{-x}dx\le\int_0^1x^{\alpha-1}dx=\frac{1}{\alpha} x^\alpha|^1_0 =\frac{1}{\alpha}$ 。

此外，我们容易证明， $[1,+\infty)$ 上的积分总收敛，事实上，由泰勒展开，对任意正整数 $M$ 都存在$e^x>\frac{x^{\alpha+M}}{(\alpha+M)!}$ ，因此 $\int_1^{+\infty}x^{\alpha-1}e^{-x}dx\le \int_1^{+\infty}x^{\alpha-1}\frac{(\alpha+M)!}{x^{\alpha+M}}dx=(\alpha+M)!\int_1^{+\infty}x^{-M-1}dx=\frac{(\alpha+M)!}{M}$

由此，我们确定了这族积分当且仅当 $\alpha>0$ 时有意义，由此给出Gamma函数的定义。

定义1：$\Gamma(\alpha)=\int_0^{\infty}x^{\alpha-1}e^{-x}dx(\alpha>0)$ 称为Gamma函数。

定埋1：（1）$\Gamma(1)=1$ ;（2）$\Gamma(\alpha+1)=\alpha\Gamma(\alpha)$;（3）当 $\alpha$ 是正整数时，$\Gamma(\alpha)=(\alpha-1)!$。

证：（1）显然。（2）$\Gamma(\alpha+1)=\int_0^{\infty}x^{\alpha}e^{-x}dx=[-x^\alpha e^{-x}]_0^\infty-\int_0^{\infty}-\alpha x^{\alpha-1}e^{-x}dx=\alpha\int_0^{\infty}x^{\alpha-1}e^{-x}dx=\alpha\Gamma(\alpha)$ 。（3）结合（1）和（2），显然易得。

不难看出，Gamma函数是阶乘的推广。

引理1：$\int_{-\infty}^{+\infty}e^{-x^2}dx=\sqrt{\pi}$

证：设 $I=\int_{-\infty}^{+\infty}e^{-x^2}dx$ ，于是 $I^2=\int_{-\infty}^{+\infty}e^{-x^2}dx\int_{-\infty}^{+\infty}e^{-y^2}dy=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}e^{-x^2-y^2}dxdy=\int_{0}^{2\pi}\int_{0}^{+\infty}re^{-r^2}drd\theta=\pi$ 。于是 $I=\sqrt{\pi}$ 。

例1：

注：后半的推导可以用来证明正态分布密度函数的积分为 $1$ 。

定理2：$\Gamma(\frac{1}{2})=\sqrt \pi$ 。

证：$\Gamma(\frac{1}{2})=\int_0^{\infty}x^{-\frac{1}{2}}e^{-x}dx=\int_0^{\infty}2e^{-x}dx^{\frac{1}{2}}=2\int_0^{\infty}e^{-t^2}dt=\int_{-\infty}^{+\infty}e^{-t^2}dt$ 。下面我们来求这个积分的值，设 $I=\Gamma(\frac{1}{2})=\int_{-\infty}^{+\infty}e^{-t^2}dt$ ，于是 $I^2=[\int_{-\infty}^{+\infty}e^{-t^2}dt]^2=\int_{-\infty}^{+\infty}e^{-x^2}dx\int_{-\infty}^{+\infty}e^{-y^2}dy=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}e^{-x^2-y^2}dxdy$ 

$=\int_{0}^{2\pi}\int_{0}^{+\infty}re^{-r^2}drd\theta=\pi$ ，于是 $\Gamma(\frac 1 2)=\sqrt\pi$ 。





例1：设 $\lambda>0$ ，则 $\int_0^{\infty}x^{\alpha-1}e^{-\lambda x}dx=\int_0^{\infty}\frac 1 \lambda x^{\alpha-1}e^{-\lambda x}d\lambda x=\int_0^{\infty}\frac 1 {\lambda^\alpha} t^{\alpha-1}e^{-t}dt=\frac{\Gamma(\alpha)}{\lambda^\alpha}$ 。

有了上面的铺垫，我们定义伽马分布：

定义2：设 $\alpha,\lambda>0$ ，分布密度函数为 $f(x)=\begin{cases}\frac{\lambda^\alpha}{\Gamma(\alpha)}x^{\alpha-1}e^{-\lambda x}&x\ge 0\\0&x<0\end{cases}$ 的分布称为伽马分布，$\alpha$ 称为形状参数，$\lambda$ 称为尺度参数。

定理3：设 $X$ 服从以 $\alpha,\lambda$ 为参数的伽马分布，则 $E(X^k)=\dfrac{(\alpha+k-1)\cdots(\alpha)}{\lambda^k}$ ；特别地，$E(X)=\frac{\alpha}{\lambda}$ ，$E(X^2)=\frac{\alpha(\alpha+1)}{\lambda^2}$ 。

证：$E(X^k)=\int_0^{\infty}\frac{\lambda^\alpha}{\Gamma(\alpha)}x^{\alpha+k-1}e^{-\lambda x}dx$ ，由例1的结论，原式 $=\frac{\lambda^\alpha}{\Gamma(\alpha)}\frac{\Gamma(\alpha+k)}{\lambda^{\alpha+k}}=\frac{(\alpha+k-1)!}{\lambda^k(\alpha-1)!}=\frac{(\alpha+k-1)\cdots(\alpha)}{\lambda^k}$  。

下面，我们知道 $Var(X)=E(X^2)-[E(x)]^2$ ，代入立即可得：

定理4：设 $X$ 服从以 $\alpha,\lambda$ 为参数的伽马分布，则 $Var(X)=\frac{\alpha}{\lambda^2}$ 。

$\phi(t)=E(e^{ixt})=\int\dfrac{\lambda^\alpha}{\Gamma(\alpha)}x^{\alpha-1}e^{-\lambda x}e^{ixt}dx=$

下面，我们继续考虑贝塔分布：

定义3：$B(a,b)=\int_0^1x^{a-1}(1-x)^{b-1}dx(a,b>0)$ 称为贝塔函数。

定理5：（1）$B(a,b)=B(b,a)$ 。（2）$B(a,b)=\dfrac{\Gamma(a)\Gamma(b)}{\Gamma(a+b)}$

#### Legendre公式

