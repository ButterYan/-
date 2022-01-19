### **第六章    集合的基数**

>  定义6.1：设 $A$ ， $B$ 是两个集合，如果存在一个从 $A$ 到 $B$ 的双射，则称集合 $A$ 与 $B$ 对等，记作 $A\sim B$ 。 定理6.1：集合的对等满足：（1） $A\sim A$ （自反性）。 （2）若 $A\sim B$ ，则 $B\sim A$ （对称性）。 （3）若 $A\sim B$ ， $B\sim C$ ，则 $A\sim C$ （传递性）。

证：（1）定义 $f:A\sim A$ ， $f(x)=x$ ，显然是双射。

（2）若 $f:A\sim B$ 是双射，由定理5.5， $f^{-1}$ 是双射。

（3）若 $f:A\sim B$ ， $g:B\sim C$ 都是双射，由定理5.6（3）， $g\circ f$ 是双射。

例6.1：设 $N^{+}$ 代表非零自然数集， $E$ 代表正偶数集，我们定义映射 $f:N^{+}\rightarrow E$ ， $f(x)=2x$ 。这是一个双射，显示两集合是对等的。但是 $E\subset N^{+}$ ，这显示了无限集的元素个数可以和它的真子集一样“多”。

>  定理6.2：设指标集族 $\left\{ A_{\alpha}|\alpha\in D \right\}$ 与 $\left\{ B_{\alpha}|\alpha\in D \right\}$ ，对于 $\alpha\ne \beta$ 都有 $A_{a}\cap A_{\beta}=\Phi$ ， $B_{a}\cap B_{\beta}=\Phi$ ，且 $\forall \alpha\in D$ ， $A_{\alpha}\sim B_{\alpha}$ ，则 $\underset{\alpha\in D}{\bigcup}A_{\alpha}\sim \underset{\alpha\in D}{\bigcup} B_{\alpha}$。

证：显然映射 $f_{\alpha}:A_{\alpha}\rightarrow B_{\alpha}$ 是双射，定义映射 $f:\underset{\alpha\in D}{\bigcup}A_{\alpha}\rightarrow \underset{\alpha\in D}{\bigcup}B_{\alpha}$ ， $f(x)=f_{\alpha}(x),x\in A_{\alpha}$ 。设 $y\in \underset{\alpha\in D}{\bigcup}B_{\alpha}$ ， $\exists \alpha$ 使得 $y\in B_{\alpha}$ ，由此 $\exists x\in A_{\alpha}$ ， $y=f(x)$ ，因此是满射；设 $x_{1}\ne x_{2}$ 且 $x_{1}, x_{2}\in \underset{\alpha\in D}{\bigcup}A_{\alpha}$ ，若 $x_{1}, x_{2}$ 属于同一个集合 $A_{\alpha}$ ，那么对于双射 $f_{\alpha}$ ，显然 $f(x_{1})\ne f(x_{2})$ ，若 $x_{1}, x_{2}$ 属于不同集合，由 $B_{a}\cap B_{\beta}=\emptyset$ ，显然 $f(x_{1})\ne f(x_{2})$，因而是单射。因此， $f$ 是双射，两集合对等。

>  定理6.3（F·Bernstein定理）：对于集合 $A，B$ ，有 $A_{0}\subset A$ ， $B_{0}\subset B$ ， $A_{0}\sim B$ ， $B_{0}\sim A$ ，则 $A\sim B$ 。

证：设 $f:A\rightarrow B_{0}$， $g:B\rightarrow A_{0}$ ，令 $A-A_{0}=A_{1}$ ， $B_{1}=f(A_{1})$ ， $A_{2}=g(B_{1})$ ，$B_{2}=f(A_{2})$ ， $A_{3}=g(B_{2})\cdots$ $B_{n}=f(A_{n})$ ， $A_{n+1}=g(B_{n})\cdots$显然 $A_{n}\sim B_{n}$ ，由定理6.2，有 $\underset{n=1}{\overset{\infty}{\bigcup}}A_{n}\sim \underset{n=1}{\overset{\infty}{\bigcup}}B_{n}$。由映射 $g$ 知， $B\sim A_{0}$ ， $B_{n}\sim A_{n+1}$ 。故 $B\setminus\underset{n=1}{\overset{\infty}{\bigcup}}B_{n}\sim A_{0}\setminus\underset{n=1}{\overset{\infty}{\bigcup}}A_{n+1}=A_{0}\setminus\underset{n=2}{\overset{\infty}{\bigcup}}A_{n}= A\setminus\underset{n=1}{\overset{\infty}{\bigcup}}A_{n}$ 。由定理6.2，

$A=(A\setminus\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})\cup\underset{n=1}{\overset{\infty}{\bigcup}}A_{n}\sim (B\setminus\underset{n=1}{\overset{\infty}{\bigcup}}B_{n})\cup \underset{n=1}{\overset{\infty}{\bigcup}}B_{n}=B$ 。即 $A\sim B$ 。

由此，我们可以推出集合对等的夹逼性质：

>  定理6.4：若 $A\subset B\subset C$ ， $A\sim C$ ，则 $A\sim B\sim C$ 。

证：由于 $C\sim A\subset B$ ， $B\sim B\subset C$ ，由定理6.3， $B\sim C$ ，再由传递性， $A\sim B\sim C$ 。

随后，我们可以引出基数的概念。

>  定义6.2：若两个集合 $A,B$ 对等，则称他们有相同的基数，记作 $\bar{\bar{A}}=\bar{\bar{B}}$ 。

注：集合的基数也称为势

>  定理6.5：（1） $\bar{\bar{A}}=\bar{\bar{A}}$ （自反性）。 （2）若 $\bar{\bar{A}}=\bar{\bar{B}}$ ，则 $\bar{\bar{B}}=\bar{\bar{A}}$ （对称性）。 （3）若 $\bar{\bar{A}}=\bar{\bar{B}}$ ， $\bar{\bar{B}}=\bar{\bar{C}}$ ，则 $\bar{\bar{A}}=\bar{\bar{C}}$ （传递性）。

证：由定理6.1，显然可得。

>  定义6.3：对于集合 $A,B$，若有 $B_{0}\subset B$ ， $A\sim B_{0}$ ，则称 $A$ 的基数小于等于 $B$ 的基数，记作 $\bar{\bar{A}}\leq\bar{\bar{B}}$ 。若 $\bar{\bar{A}}\leq\bar{\bar{B}}$ 且$A$ 与 $B$不对等，则称称 $A$ 的基数小于 $B$ 的基数，记作 $\bar{\bar{A}}<\bar{\bar{B}}$ 。 定理6.6：对于集合 $A,B$， $\bar{\bar{A}}<\bar{\bar{B}}$ ， $\bar{\bar{A}}=\bar{\bar{B}}$ ， $\bar{\bar{A}}>\bar{\bar{B}}$ 中的任意两个不会同时成立。

证：由定义6.3可知，若 $\bar{\bar{A}}=\bar{\bar{B}}$ ，$A$ 与 $B$ 对等，另外两个不会成立；假设， $\bar{\bar{A}}<\bar{\bar{B}}$ 与 $\bar{\bar{A}}>\bar{\bar{B}}$ 同时成立，则有 $B_{0}\subset B$ ，$A\sim B_{0}$ ，$A_{0}\subset A$ ，$B\sim A_{0}$ ，使用定理6.3得出 $\bar{\bar{A}}=\bar{\bar{B}}$ ，显然矛盾，证毕。

注：我们并不能断定任给两个集合都能讲两者基数的关将锁定在以上三种之内，因为我们还没有证，基数的关系不可能不属于以上三种的任意一种，在目前数学体系下，无法完成这个证明，可能与哥德尔不完备定理有关，但在Zermelo选择公理下，我们可以证明它。

### **第七章    可列集**

>  定义7.1：含有有限个元素的集合称为有限集，基数定义为其元素的个数；与自然数集对等的集合称为可列集，基数定义为 $\aleph_{0}$ ；含有无限个元素且与自然数集不对等的集合称为不可数集；含有有限个元素的集合与可列集统称为至多可数集。

注：可列集也可称可数集，可列集 $A$ 可以表示为 $\left\{ a_{n} \right\}$ 。

>  定理7.1：任何无限集必包含一个可列子集。

证：设 $A$ 为无限集，在其中任取一元素记为 $a_{1}$ ， $A_{1}=A\setminus\left\{ a_{1} \right\}$ 仍为无限集，再在 $A_{1}$ 任取一元素记为$a_{2}$ ，记 $A_{2}=A_{1}\setminus\left\{ a_{2} \right\}$，依次取下去，得一序列 $\left\{ a_{n} \right\}$ ，显然这是一可列集合，且为 $A$ 的子集，得证。

注：由此可知，在无限集中，可列集合的基数为最小。

>  定理7.2：可列集的子集至多可列。

证：设 $A$ 为可列集，表示为 $\left\{ a_{n} \right\}$ ，若它的子集不是有限集，则为它的子列构成的集合，即 $\left\{ a_{n_{k}} \right\}$ ，必为可列集。

>  定理7.3：若 $A$ 为有限集，$B$ 为可列集，则： （1） $A\cup B$ 是可列集。 （2） $B\setminus A$ 是可列集。

证：（1）易得 $(A\cup B)\setminus B\subset A$ ，从而 $A\cup B\setminus B$ 只包含 $A$ 中的有限个元素，从而 $A\cup B=\left\{b_{n} \right\}\cup\left\{a_{1},a_{2},\cdots,a_{k} \right\}$ ，我们只需令 $c_{i}=a_{i}(i\leq k)$ ， $c_{i}=b_{i+k}(i> k)$ ，那么 $A\cup B=\left\{ c_{i} \right\}$ 为可列集。

（2）显然， $B\setminus A\subset B$ ，由定理7.2，它至多可列；再假设他是有限集， $B\setminus(B\setminus A)\subset A$ ， $B\setminus(B\setminus A)$ 是有限集，由此 $B=B\setminus(B\setminus A)\cup B\setminus A$ 也是有限集，与 $B$ 为可列集矛盾，故 $A\cup B$ 为可列集。

>  定理7.4：当各集合的交集都含有有限个元素时： （1）有限个有限集的的并是有限集。 （2）可列个有限集的并是可列集。 （3）有限个可列集的并是可列集。 （4）可列个可列集的并是可列集。 

证：（1）显然。

（2）定义第 $k$ 个集合表示为 $A_{k}=\left\{ a_{n}^{(k)} \right\}$ ， $c_{m}$ 表示前 $m$ 个集合的元素个数和。令 $b_{i}=$ $a_{b_{i}-c_{m}}^{(m)}(c_{m} 

（3）设共有 $x$ 个集合，定义第 $k$ 个集合表示为 $A_{k}=\left\{ a_{n}^{(k)} \right\}$ ， $c_{m}$ 表示 $m$ 除以 $x$ 的余数， $d_{m}$ 表示 $m$ 除以 $x$ 的结果向下取整。令 $b_{i}=$$a_{d_{m}}^{(c_{m})}$ 。就有 $\underset{k=1}{\overset{\infty}{\bigcup}}A_{k}=\{ b_{i} \}$ 。

（4）设第 $p$ 个集合的第 $q$ 个元素记作 $a_{pq}$ ， $h=p+q$ ，按照 $h$ 从小到大排序， $h$ 相等时再按 $q$ 从小到大排序，就得到了一种所有元素的排序方式，再去掉重复元素，即得可列集。

注：若去掉交集有限的条件，（2）—（4）的结论变为至多可数。

>  定理7.5：（1）整数集是可列集。 （2）有理数集是可列集。 （3）$P_{n}$ 表示 $n$ 阶的整系数多项式全体，$P_{n}$ 是可列集。 （4）整系数多项式全体是可列集，进而全体代数数是可列集。

证：（1）显然整数集 $Z=N\cup\{ -1,-2,-3,\cdots,-n,\cdots \}$ ，显然二者都是可列集，由定理7.4（3），得证。

（2）集合 $Q=\underset{p=1}{\overset{\infty}{\bigcup}}\left\{ \frac{q}{p}|q\in Z \right\}$ ，由定理7.4（4）， $Q$ 为可列集。

（3）设 $k$ 为任意正整数，使用数学归纳法，当 $k=1$ 时，由（2）结论显然可列；设 $P_{n}$ 可列，则固定 $n+1$ 阶系数的 $n+1$ 阶整系数多项式可列，故 $P_{n+1}$ 为可列个 $P_{n}$ 的并，由定理7.4（4），得证。

（4）全体整系数多项式为 $\underset{n=1}{\overset{\infty}{\bigcup}}P_{n}$ ，是可列个可列集的并，由定理7.4（4），得证。

例7.1：下列元素构成的集合都是可列集：整系数多项式，有理系数多项式，代数数， $n$ 为欧式空间上的整数坐标点，$n$ 为欧式空间上的有理坐标点，分量为有理数的有限维向量。

>  定理7.6：若集合 $A_{1},A_{2},A_{3},\cdots,A_{k}$ 都是可列集，则 $A_{1}\times A_{2}\times A_{3}\times\cdots\times A_{k}$ 是可列集。

证：用数学归纳法，显然 $A_{1}$ 是可列集，假设 $A_{1}\times A_{2}\times A_{3}\times\cdots\times A_{n}$ 可列 ，那么在 $A_{1}\times A_{2}\times A_{3}\times\cdots\times A_{n}\times A_{n+1}$ 中。取定任一 $A_{n+1}$ 中的元素都是一个可列集，因此是可列个可列集的不交并；根据定理7.4（4），得证。

## **第八章    不可列集**

> 定理8.1：区间 $[0,1]$ 是不可列集。

证：假设是可列集，则 $[0,1]=\{a_{1},a_{2},\cdots,a_{n},\cdots\}$ 。我们将区间三等分，取其中一份，使得 $a_{1}\notin I_{1}$ ，再将 $ I_{1}$ 三等分，得到 $a_{2}\notin I_{2}$ ，这样一直做下去，得到一列区间列，有 $I_{1}\subset I_{2}\subset\cdots\subset I_{n}\subset\cdots$ 。显然区间长度趋于 $0$ ，由区间套定理，$\exists a\in [0,1]$ ，满足 $a\in\underset{i=1}{\overset{\infty}{\bigcap}}I_{i}$，但由于 $[0,1]$ 可列， $\exists m$ ，$a=a_{m}$ ，于是 $a\notin I_{m}$ ，矛盾，故不是可数集。

由此，我们可以找到一类基数比可列集大的无限集：

> 定义8.1：与区间 $[0,1]$ 对等的集合称为连续集，基数记为 $\aleph$ 。 定理8.2：设 $A$ 是无限集， $B$ 是至多可列集，则 $A\cup B\sim A$ 。 

证：假设 $A\cap B=\empty$ ，由于$A$ 是无限集，由定理7.1，存在可列集 $M\subset A$ ，由定理7.4， $M\sim M\cup B$ ，从而， $A\cup B=(A\setminus M)\cup(M\cup B)\sim (A\setminus M)\cup M=A$ 。若 $A\cap B\ne\emptyset$ ，则令 $C=(A\cup B)\setminus A$ ，有 $A\cup C=A\cup B$ 且 $A\cap C=\emptyset$ ，用前面结论即可证。

>  定理8.3：（1） $[0,1]\sim (0,1)$ 。 （2） $R\sim(0,1)$ 。 （3）任意含有无限个元素的区间的基数都是 $\aleph$ 。 （4）任意含有无限个元素的区间内无理数全体的基数是 $\aleph$ 。

证：（1）取 $A=(0,1)$ , $B=\left\{ 0,1 \right\}$ ，使用定理8.3即得。

（2）构造映射 $f：(0,1)\rightarrow R$ ， $f(x)=tan(πx-\frac{π}{2})$ ，不难验证这是一个双射，由此 $R\sim (0,1)$ ，得证。

（3）令 $f(x)=(b-a)x+a$ ，显然 $f$ 是从 $[0,1]$ 到 $[a,b]$ 的双射，也是从 $(0,1)$ 到 $(a,b)$ 的双射，而半开半闭区间 $(a,b)\subset [a,b)\subset [a,b]$ ，由定理6.4，基数也是 $\aleph$ ，由此，有界区间的情形得证。对于无界区间，有 $(a,a+1)\subset (a,+\infty)\subset (-\infty,+\infty)$ 。由定理6.4，得证。

（4）该区间内的有理数全体是至多可列的，由定理8.3，无理数全体与该区间对等，得证。

为了找到更多不可列集，我们通过进制的概念进一步研究区间 $(0,1)$ 。显然任何数 $a$ 都可以写成小数的形式，即 $a=\underset{n=1}{\overset{\infty}\sum}\frac{a_{n}}{10^{n}}$ ，其中 $a_{n}=0,1,\cdots,9$ ，因而 $10$ 进制可以表示 $(0,1)$ 上所有的数。我们把 $k$ 进制数全体记作 $B_{k}=\{\underset{n=1}{\overset{\infty}\sum}\frac{a_{n}}{k^{n}}|a_{n}=0,1,\cdots,9\}$ ，显然 $(0,1)\subset B_{k}$ ，但有些数会有两种表示，如 $0.5=0.4999\cdots$ ，但不难想象，至多有两种表示，于是 $B_{k}$ 可以与 $(0,2)$ 的子集建立双射，由定理6.4，$B_{k}$ 的基数为 $\aleph$ 。因此，我们可以用 $B_{k}$ 代表所有连续集进行分析。

>  定理8.4：（1）$R^{n}$ 的基数为 $\aleph$ ，即有限个连续集的直积仍是连续集。 （2）可列维的实向量全体的基数为 $\aleph$ ，即可列个连续集的直积仍是连续集。 （3） 有理数域上的可列维向量全体基数为 $\aleph$ ，即可列个可列集的直积是连续集。

证：（1）$R^{n}$ 中的一个元素可以表示为 $n$ 个小数，我们把每一个小数的第一位排列起来，再依次这样排列第二位、第三位 $\cdots$ ，即可得一个 $R_{n}$ 到 $R$ 的双射，得证。

（2）设第 $p$ 个分量的第 $q$ 位小数记作 $a_{pq}$ ， $h=p+q$ ，按照 $h$ 从小到大排序， $h$ 相等时再按 $q$ 从小到大排序，就得到了一种所有元素的排序方式，因而是连续集。

（3）我们将向量的每一位理解为小数，则每一位有可列种选择，而小数集 $B_{k}$ 有有限种选择，故基数不小于 $\aleph$ ；另一方面，可列个可列集的直积小于可列个连续集，故基数不大于 $\aleph$ ，综上，得证。

注：全体整系数多项式的基数为 $\aleph_{0}$ ，它不能够看作是可列个可列集的直积，因为任何整系数多项式都包含于有限个可列集的直积，而事实上，不包含于有限个可列集的元素更多，因而可列个可列集的直积的基数为 $\aleph$ 。

我们把用集合的基数用有限数想象以下，比如：二进制数就是可列位小数，每一位都有两种选择，因而可以表达为 $2^{\aleph_{0}}$ 。类似地，记 $n$ 为有限基数，无限集基数运算的结论可以记作：$\aleph_{0}=\aleph_{0}-n=\aleph_{0}+n$ ，$\aleph_{0}=n\aleph_{0}=\aleph_{0}\times \aleph_{0}=\aleph_{0}^{n}$ ；$n^{\aleph_{0}}=\aleph_{0}^{\aleph_{0}}=\aleph$ ，$\aleph=\aleph-\aleph_{0}=\aleph+\aleph_{0}$ ，$\aleph=n\aleph=\aleph_{0}\times\aleph$  ， $\aleph=\aleph^{\aleph_{0}}$ 。

那么一个问题出现了，还有没有基数更大的集合呢？答案是肯定的。我们前面将可列集作为指数得到了连续集，我们想，如果将连续集作为指数，得到的自然应该是基数更大的集合，下面我们借助定义1.8中幂集的概念来说明这个问题。

> 定理8.5（康托定理）：设 $A$ 是一个集合，那么 $P(A)$ 的势大于 $A$ 的势。

证：有限的情形由定理1.3显然。无限的情形我们用反证法，假设有映射 $f：A\rightarrow P(A)$ 是双射 ，首先假设 $\forall a\in A$ ，都有 $a\notin f(a)$ ，那么 $f^{-1}(A)=\emptyset$ ，不成立；其次，如果存在 $a\in A$ ，满足 $a\notin f(a)$ ，令 $B=\{a|a\notin f(a)\}$ ，易得 $f^{-1}(A)=\emptyset$ ，不成立；因此， $\forall a\in A$ ，都有 $a\in f(a)$ ，于是 $\forall a\in A$ ，发现必有 $f^{-1}(\{a\})=a$ ，于是 $P(A)$ 中的单元素集就已经用尽了 $A$ 中的所有元素，这不是双射，矛盾，因此得证。

定理8.1是康托定理对于可列集下的特例。定理8.5说明了不存在基数“最大”的集合，因为任何集合的幂集的基数都会更大。至此，我们通过幂集说明了无穷是一级一级递增，没有上限的。另一个问题便是两级之间，即一个无限集与它的幂集合之间有没有其它基数，更具体地，连续集与可列集之间还有没有其他基数，这称为连续统假设，目前为止既无法证实也无法证伪，是一个非常复杂的问题。