### **第四章    集列的极限**

>  定义4.1：对于集列 $\left\{ A_{n} \right\}$ ，若 $\forall i$ ，都有 $A_{i}\subset A_{i+1}$ ，则称 $\left\{ A_{n} \right\}$ 是单调递增的集列；若 $\forall i$ ，都有 $A_{i+1}\subset A_{i}$ ，则称 $\left\{ A_{n} \right\}$ 是单调递减的集列。

例4.1： $\underset{n=1}{\overset{\infty}{\bigcup}}[\frac{1}{n},1-\frac{1}{n}]=(0,1)$ ， $\underset{n=1}{\overset{\infty}{\bigcap}}[n,+\infty)=\emptyset$ 。

本节我们考虑集列的极限集，通过例4.1，我们发现，单调集列的极限比较容易刻画，单调递减的集列的极限可以定义为它们的无穷交，单调递增的集列的极限可以定义为它们的无穷并；并且，容易发现，对于任意集列 $\{A_{n}\}$，都有 $B_{n}=\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}$ 是单调递减的集列，$C_{n}=\underset{j=n}{\overset{\infty}{\bigcap}}A_{j}$ 是单调递增的集列。据此，我们产生了上极限与下极限的定义：

>  定义4.2：对于集列 $\left\{ A_{n} \right\}$ ，称$\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}$ 为集列 $\left\{ A_{n} \right\}$ 的上极限，记作 $\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ ；$\underset{n=1}{\overset{\infty}{\bigcup}}\underset{j=n}{\overset{\infty}{\bigcap}}A_{j}$ 为集列 $\left\{ A_{n} \right\}$ 的下极限，记作 $\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ 。

下面我们通过一个定理来研究上下极限的本质：

>  定理4.1：对于集列 $\left\{ A_{n} \right\}$ ， （1）$x\in\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}\Leftrightarrow \forall m$，都有 $n>m$ ，使得 $x\in A_{n}$ 。 （2）$x\in\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}\Leftrightarrow \exists m$ ，当 $n>m$时，总有 $x\in A_{n}$ 。

证：（1）$\Rightarrow$ ：若 $x\in\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ ，则 $x\in\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}$ ，则 $\forall n$ ，都有 $x\in\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}$ ，因此 $x\in\underset{j=m}{\overset{\infty}{\bigcup}}A_{j}$ ，因此必存在 $n>m$ ，使得 $x\in A_{n}$ 。 $\Leftarrow$ ：若存在 $n>m$ ，使得 $x\in A_{n}$ ，则意味着 $x\in\underset{j=m}{\overset{\infty}{\bigcup}}A_{j}$ ，由于对任意 $m$ 都成立，则有 $x\in\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}=\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ 。

（2）$\Rightarrow$ ：若 $x\in\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ ，则 $x\in\underset{n=1}{\overset{\infty}{\bigcup}}\underset{j=n}{\overset{\infty}{\bigcap}}A_{j}$ ，则 $\exists n$ ，都有 $x\in\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}$ ，因此 $x\in\underset{j=m}{\overset{\infty}{\bigcup}}A_{j}$ ，因此必存在 $n>m$ ，使得 $x\in A_{n}$ 。 $\Leftarrow$ ：若存在 $n>m$ ，使得 $x\in A_{n}$ ，则意味着 $x\in\underset{j=m}{\overset{\infty}{\bigcup}}A_{j}$ ，由于对任意 $m$ 都成立，则有 $x\in\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}=\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ 。

与数学分析中数列的上下极限类似，上极限描集中的元素是属于原集列的任意子列的元素，或属于集列中无限个集合的元素；下极限描述的元素是仅仅不属于集列中有限个集合的元素。因此，显然地有 $\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}\subset\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ 。由此，我们给出极限集存在的定义：

>  定义4.3：若对于集列 $\left\{ A_{n} \right\}$， $\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ ，则称它是收敛集列，定义它的极限为 $\lim \limits_{n \rightarrow \infty}{A_{n}}=\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}$ 。

下面我们说明在此定义下单调集列的极限与我们期望的情形是一样的：

>  定理4.2：若集列 $\left\{ A_{n} \right\}$  单调递减，则 $\lim \limits_{n \rightarrow \infty}{A_{n}}=\underset{n=1}{\overset{\infty}{\bigcap}}A_{n}$ ；若集列 $\left\{ A_{n} \right\}$ 单调递增，则 $\lim \limits_{n \rightarrow \infty}{A_{n}}=\underset{n=1}{\overset{\infty}{\bigcup}}A_{n}$ 。

证：若集列 $\left\{ A_{n} \right\}$单调递减，则 $\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}=\underset{n=1}{\overset{\infty}{\bigcap}}A_{n}$ ， $\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=\underset{n=1}{\overset{\infty}{\bigcup}}\underset{j=n}{\overset{\infty}{\bigcap}}A_{j} =\underset{n=1}{\overset{\infty}{\bigcup}}\underset{j=1}{\overset{\infty}{\bigcap}}A_{j}= \underset{n=1}{\overset{\infty}{\bigcap}}A_{n}$ 。若集列 $\left\{ A_{n} \right\}$单调递增，则 $\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=n}{\overset{\infty}{\bigcup}}A_{j}=\underset{n=1}{\overset{\infty}{\bigcap}}\underset{j=1}{\overset{\infty}{\bigcup}}A_{j}=\underset{n=1}{\overset{\infty}{\bigcup}}A_{n}$ ， $\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=\underset{n=1}{\overset{\infty}{\bigcup}}\underset{j=n}{\overset{\infty}{\bigcap}}A_{j}=\underset{n=1}{\overset{\infty}{\bigcup}}A_{n}$ 。

### **第五章    映射与双射**

>  定义5.1：设 $A,B$ 为两个非空集合，若有一个对应法则 $f$ ，使得 $\forall x\in A$ ，有**唯一**一个 $y\in B$ 与之对应，则称 $f$ 为从 $A$ 到 $B$ 的映射记作 $f：A\rightarrow B$ ，对应元素的关系写作 $y=f(x)$ ，集合 $A$ 称为 $f$ 的定义域，记作 $D(f)$ ， $f(A)=\left\{ f(x)|x\in A \right\}$ 是 $f$ 的值域，记作 $R(f)$ 。

注：定义域的英文是Domain，值域是Range。只有 $R(f)\subset B$ ，不一定有 $R(f)=B$ 。

>  定义5.2：若 $A_{1}\subset A$ ，集合 $f(A_{1})=\left\{ f(x)|x\in A_{1} \right\}$ 称为 $A_{1}$ 的像集。若$B_{1}\subset B$ ，集合 $f^{-1}(B_{1})=\left\{ x\in A|f(x)\in B_{1} \right\}$ 称为 $B_{1}$ 的原像集。

例5.1：设 $X$ 是集合，从 $X\times X$ 到 $X$ 的映射 $f$ 称为运算，如 $X=R$ 时，令 $f(x,y)=x+y$ 或 $f(x,y)=xy$ 即为 $R$ 上的加法和或乘法运算。进一步地，如果有 $f(x,y)=f(y,x)$ 恒成立，则称运算满足交换律；如果 $f(f(x,y),z)=f(x,f(y,z))$ 恒成立，则称运算满足结合律。上述的加法与乘法运算满足交换律和结合律。

>  定义5.3：对于$f：A\rightarrow B$，若 $B$ 是数集，则 $f$ 称作泛函；若 $A,B$ 都是数集，则 $f$ 称作函数。

例5.2：设 $S$ 是全集，$A\subset S$ ，定义从 $S$ 到 $\{0,1\}$ 的函数 $1_{A}(x)=\begin{cases}1\quad x\in A\\0\quad x\notin A\end{cases}$ ，称为集合 $A$ 的示性函数。显然这是泛函，当 $S$ 是数集时，这是函数。并且 $1_{A\cap B}=min\{1_{A},1_{B}\}=1_{A}1_{B}$ ，$1_{A^{c}}=1-1_{A}$ ，$1_{A\setminus B}=min\{1_{A},1-1_{B}\}=1_{A}(1-1_{B})$ ，$1_{A\cup B}=max\{1_{A},1_{B}\}=1-min\{1-1_{A},1-1_{B}\}+1-(1-1_{A})(1-1_{B})=1_{A}+1_{B}-1_{A}1_{B}$ ， $1_{A\triangle B}=max\{min\{1_{A},1-1_{B}\},min\{1-1_{A},1_{B}\}\}$ $=1_{A}(1-1_{B})+(1-1_{A})1_{B}-1_{A}(1-1_{B})(1-1_{A})1_{B}=1_{A}+1_{B}-21_{A}1_{B}$ 。 若 $\overline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=A$，则$\overline{\lim} \limits_{n \rightarrow \infty}1_{A_{n}}(x)=1_{A}(x)$ ；若 $\underline{\lim} \limits_{n \rightarrow \infty}{A_{n}}=A$，则$\underline{\lim} \limits_{n \rightarrow \infty}1_{A_{n}}(x)=1_{A}(x)$ ；若 $\lim \limits_{n \rightarrow \infty}{A_{n}}=A$，则$\lim \limits_{n \rightarrow \infty}1_{A_{n}}(x)=1_{A}(x)$ 。

>  定义5.4：对于$f：A\rightarrow B$，若 $\forall y\in B$ ，都有 $x\in A$ ，满足 $f(x)=y$ ，则称 $f$ 是满射。若 $\forall x_{1}\ne x_{2}$ ，都有 $f(x_{1})\ne f(x_{2})$ ，则称 $f$ 是单射。若 $f$ 既是满射又是单射，则称 $f$ 是双射。

注：满射也可以理解为 $R(f)=B$ ，单射理解为 $\forall y\in B$ ，$f^{-1}(y)$ 至多有一个元素，双射建立了两个集合的一一对应。

>  定理5.1：对于映射 $f：A\rightarrow B$ ， $f(A_{1}\cup A_{2})=f(A_{1})\cup f(A_{2})$

证：由于 $A_{1},A_{2}\subset A_{1}\cup A_{2}$ ，有 $f(A_{1}),f(A_{2})\subset f(A_{1}\cup A_{2})$ ，从而有 $f(A_{1})\cup f(A_{2})\subset f(A_{1}\cup A_{2})$ 。若 $y\in f(A_{1}\cup A_{2})$ ，则 $\exists x\in A_{1}\cup A_{2}$ ，使得 $y=f(x)$ ，故 $x\in A_{1}$ 或 $x\in A_{2}$ ，从而 $y\in f(A_{1})$ 或 $y\in f(A_{2})$ ，因此证得了 $f(A_{1}\cup A_{2})\subset f(A_{1})\cup f(A_{2})$ 。综上， $f(A_{1}\cup A_{2})=f(A_{1})\cup f(A_{2})$ 。

>  定理5.2：对于映射 $f：A\rightarrow B$ ， $f(A_{1}\cap A_{2}) \subset f(A_{1})\cap f(A_{2})$ ，若 $f$ 是单射，则有 $f(A_{1}\cap A_{2}) =f(A_{1})\cap f(A_{2})$ 。

证：由于 $ A_{1}\cap A_{2}\subset A_{1},A_{2}$ ，有 $f(A_{1}\cap A_{2})\subset f(A_{1}),f(A_{2})$ ，从而有 $f(A_{1}\cap A_{2})\subset f(A_{1})\cap f(A_{2})$ 。若 $f$ 是单射，设 $y\in f(A_{1})\cap f(A_{2})$ ，则 $\exists x$ ，使得 $y=f(x)$ ，并且 $x\in A_{1}$ 且 $x\in A_{2}$ ，即 $x\in A_{1}\cap A_{2}$ ，从而 $y\in f(A_{1}\cap A_{2})$ ，因此证得了 $f(A_{1})\cap f(A_{2})\subset f(A_{1}\cap A_{2})  $ 。综上， $f(A_{1}\cap A_{2})=f(A_{1})\cap f(A_{2})$ 。

注：定理5.1和5.2将两个集合的交并推广为若干指标集仍成立，证：类似。

>  定理5.3：对于映射 $f：A\rightarrow B$， （1） $A_{1}\subset f^{-1}(f(A_{1}))$ ，当 $f$ 是单射时， $A_{1}=f^{-1}(f(A_{1}))$ 。 （2） $f(f^{-1}(B_{1}))\subset B_{1}$ ，当 $f$ 是满射时， $f(f^{-1}(B_{1}))= B_{1}$ 。

证：（1）设 $x\in A_{1}$ ，则 $y=f(x)\in f(A_{1})$ ，那么显然 $x\in f^{-1}(y)\subset f^{-1}(f(A_{1}))$ 。若$f$ 是单射，令 $x\in f^{-1}(f(A_{1}))$ ，则 $y\in f(A_{1})$ ，满足 $y=f(x)$ ，由于是单射，满足 $y=f(x)$ 的 $x$ 是唯一的，因此 $x\in A_{1}$ 。

（2）设 $y\in f(f^{-1}(B_{1}))$ ，则必存在 $x\in f^{-1}(B_{1})$ ，满足 $y=f(x)$ ，由于映射的性质，满足 $x= f^{-1}(y)$ 的 $y$ 是唯一的，总而 $y\in B_{1}$ 。若$f$ 是满射，令 $y\in B_{1}$ ，则 $\exists x\in f^{-1}(B_{1})$ ，显然 $y=f(x)$ ，因此 $y\in f(f^{-1}(B_{1}))$ 。

>  定理5.4：若 $A,B$ 是有限集，包含 $n$ 个元素，则对于映射 $f：A\rightarrow B$，有 $f$ 是单射 $\Leftrightarrow f$ 是双射 $\Leftrightarrow f$ 是满射。

证：若 $f$ 是单射，则 $f(A)$ 中的元素个数为 $n$ ，不然必存在 $f(x_{1})=f(x_{2})$ ；因此 $f(A)=B$ ，$f$ 是满射，进而是双射。若 $f$ 是满射，若有 $f(x_{1})=f(x_{2})$ ，则 $f(A)=f(A\setminus\{x_{1},x_{2}\})\cup \{f(x_{1})\}$ ，至多有 $n-1$ 个元素，与 $f$ 是满射矛盾，因此 $f$ 是单射，进而是双射。

注：上述结论对于无限集不成立，例如 $f：Z\rightarrow Z$ ，$f(x)=2x$ ，是一个单射，但不是满射。

>  定义5.5：若$f：A\rightarrow B$ 是双射，那么对于 $\forall b\in B$ ，都有唯一的 $a\in A$ ，使得 $f(a)=b$ ，则令 $f^{-1}(b)=a$ ，那么 $f^{-1}：B\rightarrow A$ ，称为 $f$ 的逆映射。 定理5.5：若$f：A\rightarrow B$ 不是双射，则 $f^{-1}$ 不是映射；若 $f$ 是双射，则 $f^{-1}$ 是双射。

证：若 $f$ 不是满射，$\exists y\in B$ ， $f^{-1}(\left\{ y \right\})=\emptyset$ ，若 $f$ 不是单射，$\exists y\in B$ ， $f^{-1}(\left\{ y \right\})=\left\{ x_{1},x_{2} \right\}$，其中 $y=f(x_{1})=f(x_{2})$ 。因而$f^{-1}$ 不是映射。相反地，若$f$ 是双射，则 $\forall y\in B$ ， $f^{-1}(\left\{ y \right\})=\left\{ x\right\}$，其中 $y=f(x)$ ，从而是映射，又 $f$ 是映射，因而 $f^{-1}(y_{1})\ne f^{-1}(y_{2})$ ，是单射，满射显然，因而双射得证。

>  定义5.6：设 $f：A\rightarrow B$ ， $g：B\rightarrow C$ ，可以由表达式 $g(f(x))$ 定义复合映射 $g\circ f：A\rightarrow C$ 。 定理5.6：对于映射$f：A\rightarrow B$ ， $g：B\rightarrow C$，与复合映射 $g\circ f：A\rightarrow C$ ，有： （1）若 $g,f$ 为单射，则 $g\circ f$ 为单射。 （2）若 $g,f$ 为满射，则 $g\circ f$ 为满射。 （3）若 $g,f$ 为双射，则 $g\circ f$ 为双射。

证：（1）若 $x_{1},x_{2}\in A$ ，由于$g,f$ 为单射，有 $f(x_{1})\ne f(x_{2})$ 和$g(f(x_{1}))\ne g(f(x_{2}))$ ，因而为单射。

（2）若 $z\in C$ ，由于 $g,f$ 为满射， $\exists y\in B$ ，使 $g(y)=z$ ，$\exists x\in A$ ，使 $f(x)=y$ ，此时 $z=g(f(x))$ ，因而是满射。

（3）根据（1）（2）结论直接可得。