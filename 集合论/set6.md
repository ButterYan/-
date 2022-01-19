## 第十章    开集与闭集

由于本章包含大量第九章证明的内容，因此，在学习本章前，请先阅读第九章。

> 定义10.1：设 $X$ 为研究的点集全集， $A\subset X$ ， 若 $A=A^{\circ}$ ，则称 $A$ 为开集。 引理：球形邻域和方邻域都是开集。

证：假设 $U_{x}$ 为 $x$ 的 $\delta$ 邻域，取其中任意一点 $z:(z_{1},z_{2},...z_{n})$ ， $U=\left\{ (y_{1},y_{2},...y_{n})|\sqrt{\sum_{i=1}^{n}{(x_{i}-y_{i})^{2}}}<\delta \right\}$ ，令 $\delta_{1}=\frac{\delta-\sqrt{\sum_{i=1}^{n}{(x_{i}-z_{i})^{2}}}}{2}$ ，我们可以取 $z$ 的 $\delta_{1}$ 邻域 $U_{z}$ ，显然， $U_{z}\subset U_{x}$ ，从而 $z$ 是 $U_{x}$ 的内点， $U_{x}$ 就是开集了。对于方邻域，也可以构造出类似的邻域，证明类似。

我们已经给出了开集的概念，接下来我们讨论关于邻域的本质问题，首先回忆一下定义9.1.1：设 $(X,\Im)$ 是拓扑空间, $x\in X$ ， $U$是 $X$ 的一个子集，满足: 存在一 个开集 $V\in \Im$ 使得 $x\in V\subset U$ ，则称 $U$ 为 $x$的一个邻域。

前面说过，邻域的本质是开集，我们发现根据上述定义，如果 $U_{x}$ 是 $x$ 的一个邻域，满足某种前面讨论过的性质，那么必存在一个它的开邻域$V$ 也满足这个性质，再加上下面的定理，我们可以充分理解邻域的本质了。

> 定理10.1：设 $X$ 为研究的点集全集， 若 $x\in U\subset X$ ，且 $U$ 为开集，则 $U$ 是点 $x$ 的邻域。

证：根据定义9.1.1， $x\in U\subset U$ ，得证。

> 定义10.2：设 $X$ 为研究的点集全集， $A\subset X$ ， 若 $A^{c}$ 是开集，则称 $A$ 为闭集。 定理10.2：设 $X$ 为研究的点集全集， $A\subset X$ ，$A$ 为闭集 $\Leftrightarrow A=\bar{A}$ 。

证：若 $A$ 为闭集 $\Leftrightarrow$ $A^{c}$ 为开集 $\Leftrightarrow A^{c}=(A^{c})^{\circ}$ $\Leftrightarrow A=A^{\circ}\cup \partial A$ $\Leftrightarrow A=\bar{A}$ 。

注：本条定理可以看作闭集的第二定义。

> 定理10.3：设 $X$ 为研究的点集全集， $A\subset X$ ，若 $A$ 包含所有的极限点，则$A$ 为闭集。

证： $A^{'}\subset A$ ，则有 $\bar{A}=A^{'}\cup A\subset A$ 。由定理10.2，得证。

> 定理10.4：(1) 若 $ A\subset B$ ，则 $A^{\circ}\subset B^{\circ}$ *，*$\bar{A}\subset \bar{B}$ 。 （2） $(A\cap B)^{\circ} =A^{\circ}\cap B^{\circ}$ ， ![ \bar{A}\cup\bar{B} = \overline{A\cup B}](https://www.zhihu.com/equation?tex=%20%5Cbar%7BA%7D%5Ccup%5Cbar%7BB%7D%20%3D%20%5Coverline%7BA%5Ccup%20B%7D) \bar{A}\cup\bar{B} = \bar{A\cup B} 。

证：（1）设 $x\in A^{\circ}$ ，则存在邻域 $U_{x}$ ，满足 $U_{x}\subset A \subset B$ ，从而 $x\in B^{\circ}$ ，即 $A^{\circ}\subset B^{\circ}$ 。由 $ A\subset B$ ，利用定理3.2（1）得 $B^{c}\subset A^{c}$ ，再利用刚才证明的结论有： $(B^{c})^{\circ}\subset (A^{c})^{\circ}$ ，再次利用定理3.2（1）得 $\bar{A}\subset \bar{B}$ 。

（2）设 $x\in (A\cap B)^{\circ} $ ，则存在邻域 $U_{x}$ ，满足 $U_{x}\subset A\cap B$ ，从而 $U_{x}\subset A$ 且 $U_{x}\subset B$ ，由此， $x\in A^{\circ}\cap B^{\circ}$ ， $(A\cap B)^{\circ} \subset A^{\circ}\cap B^{\circ}$ ；若 $x\in A^{\circ}\cap B^{\circ}$ ，则存在邻域 $U_{x}$ ，满足 $U_{x}\subset A$ 且 $U_{x}\subset B$ ，从而 $U_{x}\subset A\cap B$ ， $x\in (A\cap B)^{\circ} $ ， $A^{\circ}\cap B^{\circ}\subset (A\cap B)^{\circ}$ ；综上， $(A\cap B)^{\circ} =A^{\circ}\cap B^{\circ}$ 。

由定理3.4，有 ![ \bar{A}\cup\bar{B} =(\bar{A}^{c}\cap \bar{B}^{c})^c=[(A^{c})^{\circ}\cap (B^{c})^{\circ}]^c](https://www.zhihu.com/equation?tex=%20%5Cbar%7BA%7D%5Ccup%5Cbar%7BB%7D%20%3D(%5Cbar%7BA%7D%5E%7Bc%7D%5Ccap%20%5Cbar%7BB%7D%5E%7Bc%7D)%5Ec%3D%5B(A%5E%7Bc%7D)%5E%7B%5Ccirc%7D%5Ccap%20(B%5E%7Bc%7D)%5E%7B%5Ccirc%7D%5D%5Ec) \bar{A}\cup\bar{B} =\bar{A}^{c}\cap \bar{B}^{c}=(A^{c})^{\circ}\cap (B^{c})^{\circ} ，再由前述定理，得 ![[(A^{c})^{\circ}\cap (B^{c})^{\circ}]^c=[(A^{c}\cap B^{c})^{\circ}]^c=\overline{(A^{c}\cap B^{c})^c}=\overline{A\cup B}](https://www.zhihu.com/equation?tex=%5B(A%5E%7Bc%7D)%5E%7B%5Ccirc%7D%5Ccap%20(B%5E%7Bc%7D)%5E%7B%5Ccirc%7D%5D%5Ec%3D%5B(A%5E%7Bc%7D%5Ccap%20B%5E%7Bc%7D)%5E%7B%5Ccirc%7D%5D%5Ec%3D%5Coverline%7B(A%5E%7Bc%7D%5Ccap%20B%5E%7Bc%7D)%5Ec%7D%3D%5Coverline%7BA%5Ccup%20B%7D)(A^{c})^{\circ}\cap (B^{c})^{\circ}=(A^{c}\cap B^{c})^{\circ}=\bar{(A^{c}\cap B^{c})^c}=\bar{A\cup B} 。

> 定理10.5：关于开集，有以下结论： （1）空集和全集是开集。 （2）任意多个开集的并集是开集。 （3）有限多个开集的交集是开集。

证：（1）由于 $\Phi^{\circ}\subset \Phi$ ，显然有 $\Phi^{\circ}=\Phi$ ，故空集是开集。设 $X$ 是全集，任意 $x\in X$ ，显然有 $U_{x}\subset X$ ，故全集也是开集。

（2）设 $A=\bigcup_{i=1}^{\infty}A_{i}$ ，则任意 $x\in A$ ， $U_{x}\subset A_{j}\subset A$ ，因而 $A=A^{\circ}$ ，得证。

（3）设 $A,B$ 是开集， $(A\cap B)^{\circ} =A^{\circ}\cap B^{\circ}=A\cap B$ ，集合的交满足结合律，因此用数学归纳法即可得证。

> 例11.1： $\bigcap_{n=1}^{\infty}(-\frac{1}{n},1+\frac{1}{n})=[0,1]$ ，是闭集，任意多个开集的交未必是开集。 定理10.6：关于闭集，有以下结论： （1）空集和全集是闭集。 （2）任意多个闭集的交集是闭集。 （3）有限多个闭集的并集是闭集。

证：（1）由定理10.5（1）立即可得。

（2）设 $A=\bigcap_{i=1}^{\infty}A_{i}$ ，由定理3.5，由 $A^{c}=\bigcup_{i=1}^{\infty}A_{i}^{c}$ ，显然 $A_{i}^{c}$ 是开集，由定理10.5（2）， $A^{c}$ 是开集，从而 $A$ 是闭集。

（3）设 $A=\bigcup_{i=1}^{n}A_{i} $ ，由定理3.5，由 $A^{c}=\bigcap_{i=1}^{n}A_{i}^{c}$ ，显然 $A_{i}^{c}$ 是开集，由定理10.5（3）， $A^{c}$ 是开集，从而 $A$ 是闭集。

> 例10.2： $\bigcup_{n=1}^{\infty}[\frac{1}{n},1-\frac{1}{n}]=(0,1)$ ，是开集，任意多个闭集的并未必是闭集。 定理10.7：若 $A$ 是开集， $B$ 是闭集，则 $A-B$ 是开集， $B-A$ 是闭集。

证： $A-B=A\cap B^{c}$ ，由闭集定义得 $B^{c}$ 是开集，再由定理10.5（3）得证，同理可证另外一命题。

> 定理10.8：（1）$A^{\circ}$ 是开集，并且是 $A$ 所包含的最大的开子集。 （2） $\bar{A}$ 是闭集， 并且是包含 $A$ 的最小的闭集。

证：（1）设 $A$ 所包含的所有开集构成的子集族为 $\Im$ ，设 $ U ⊂ A $ 是 $A$ 中的开集，则

$∀ x ∈ U$ ， $ x ∈ U ⊂ A$ ， 则 $x$ 也是 $A$ 的内点， $x\in A^{\circ}$ ，于是 $ U\subset A^{\circ}$ ，因此， $\bigcup_{U\in\Im}^{}U\subset A^{\circ}$ 。反之， $\forall x\in A^{\circ}$ ，存在开集 $U$ ，满足 $ x ∈ U ⊂ A$ ，于是  $x\in \bigcup_{U\in\Im}^{}U$， 即有 $A^{\circ}\subset \bigcup_{U\in\Im}^{}U$ ，综上，$A^{\circ}$ 是 $A$ 所包含的所有开集的并集，当然也是开集，并且是$A$所包含的最大的开子集。

（2）考虑$\bar{A}^{c}=(A^{c})^{\circ}$，由（1）结论， $(A^{c})^{\circ}$ 是开集，因此，$\bar{A}$ 是闭集。设 $V$ 是闭集，且 $A\subset V$ ，则 $V^{c}$ 是开集， $V^{c}\subset A^{c}$ 。由（1），$(A^{c})^{\circ}$ 是$A^{c}$ 所包含的最大的开子集，因此，$\bar{A}$ 是包含 $A$ 的最小的闭集。

> 推论10.1： $(A^{\circ})^{\circ}=A^{\circ}$ ， $\bar{\bar{A}}=\bar{A}$ 。

证：由定理10.8，和开集，并集定义显然。

> 定理10.7：设 $X$ 为研究的点集全集， 若 $A\subset X$ ，且 $A$ 非空，则： (1) $∂A ⊂ A ⇔ A $ 是闭集。 (2) $A ∩ ∂A = \Phi⇔ A $ 是开集。 (3) $∂A = \Phi⇔ A$既是开集又是闭集。

证：（1）由于 $A^{\circ}\subset A$ ， $∂A ⊂ A ⇔ A=\partial A\cup A^{\circ}=\bar{A} \Leftrightarrow A$ 是闭集。

（2） $A ∩ ∂A = \Phi⇔ A =A^{\circ}\Leftrightarrow A$ 是开集。

（3）显然满足（1）和（2）的条件，故既是开集又是闭集。

> 推论10.2：欧式空间上的单点集是闭集。

证：容易验证定理10.7（1）的条件成立。

> 例10.3：定义二维欧式空间中的集合$E_{1}=\left\{ (0,0) \right\}\cup \left\{ (x,y)|x^{2}+y^{2}>1 \right\}$， $E_{2}=\left\{ (x,y)|x^{2}+y^{2}\geq1 \right\}\cup\left\{ (0,0) \right\}$，他们的边界都是$\left\{ (x,y)|x^{2}+y^{2}=1 \right\}\cup\left\{ (0,0) \right\}$，容易验证 $E_{1}$ 不满足定理10.7（1）（2），既不是开集，也不是闭集。而 $E_{2}$ 满足（1），是闭集。

## 第十二章    紧集与连通集

> 定义11.1：设 $X$ 为研究的点集全集， $A\subset X$ ， 若 $\left\{ O_{\alpha}|\alpha\in E \right\}$ 是 $X$ 上的一个开集族，若 $A\in \bigcup_{\alpha\in E}^{}O_{\alpha}$ ，则称 $\left\{ O_{\alpha}|\alpha\in E \right\}$ 是 $A$ 的一个开覆盖，若集合 $E$ 中有有限个元素，则称 $\left\{ O_{\alpha}|\alpha\in E \right\}$ 是 $A$ 的一个有限开覆盖。 定义11.2：设 $X$ 为研究的点集全集， $A\subset X$ ，若 $A$ 的任意开覆盖都有有限子覆盖，则称 $A$ 是紧集。 定理11.1：设 $A\subset R^{n}$ ，则 $A$ 是紧集 $\Leftrightarrow$ $A$ 是有界闭集。

证：将以原点 $O$ 为中心，半径为 $r$ 的求形邻域记作 $U(O,r)$ ，显然集族 $\left\{ U(O,k)|k\in N\right\}$ 构成了 $A$ 的一个开覆盖，若$A$ 是紧集，则存在有限开覆盖使得 $A\subset \bigcup_{i=1}^{n}U(O,k_{i})$ ，则有 $A$ 中的所有点与原点的欧式距离小于 $max\{k_{i}\}$ ，从而 $A$ 有界。

再假设 $A$ 不是闭集，参考闭集定义（ $A=\bar{A}=A\cup $ $A^{'}$)，得到 $\exists x\in A^{'}$ ，有 $x\notin A$ ，那么再取 $\forall y\in A$ ，存在 $r_{x}$ ，使得 $U(x,r_{x})\cap U(y,r_{x})=\Phi$ 。由于 $A\subset \bigcup_{y\in A}^{}U(y,r_{x})$ ，由于 $A$ 是紧集，存在 $y_{1},y_{2},y_{3}...y_{n}$ ，满足 $A\subset \bigcup_{i=1}^{n}U(y_{i},r_{x})$ ，显然 $U(x,r_{x})\subset \bigcup_{i=1}^{n}U(y_{i},r_{x})$ ，与 $\forall y$ ，$U(x,r_{x})\cap U(y,r_{x})=\Phi$ 矛盾。从而 $A$ 是闭集， $\Rightarrow$ 得证。

$\Leftarrow$ 的证明请参考扩展阅读（1）中的有限覆盖定理，并在此基础上自行从一维推广到高维。

> 定义11.3：设 $A\subset X$ ， 若 $A$ 不能写成两个非空不相交开集的并，则称 $A$ 是连通集。 定义11.4：设 $X$ 为研究的点集全集， $A\subset R^{n}$ ， 若 $\forall x,y\in A$ ，都存在一条连续曲线满足， $h(a)=x$ ， $h(b)=y$ ，且 $\forall t\in [a,b]$ ，都有 $h(t)\in A$ ，则称 $A$ 为道路连通的。 定义11.5：道路连通的开集是区域。若 $A$ 是区域，那么 $\bar{A}$ 称为闭区域。 定义11.6：设 $A$ 是一个区域，若 $\forall x,y\in A$ ，都有 $tx+(1-t)y\in A(t\in[0,1]) $ ，则称 $A$ 是凸域。

由于文章性质，本章内容只给出数学分析的定义，拓扑学相关知识请自行阅读扩展阅读。拓扑学对开集闭集的体系构建过程是与本文不同的，他们将定理10.5作为开集的定义，本文是以研究集合的视角建立的体系，与之不同请大家理解。

## 扩展阅读：

（1）

[乌兰巴托海军：七大实数理论与互推](https://zhuanlan.zhihu.com/p/84625424)

（2）

[乌兰巴托海军：七大实数理论互推完整版](https://zhuanlan.zhihu.com/p/83426407)

（3）

[学弱猹：拓扑学Ⅱ|笔记整理（1）——拓扑基本概念及性质，连续](https://zhuanlan.zhihu.com/p/34986735)

（4）

[学弱猹：拓扑学Ⅱ|笔记整理（2）——乘积空间，拓扑基，分离公理](https://zhuanlan.zhihu.com/p/35050567)

（5）

[学弱猹：拓扑学Ⅱ|笔记整理（3）——可数公理，Urysohn可度量化定理](https://zhuanlan.zhihu.com/p/35125375)

（6）

[学弱猹：拓扑学Ⅱ|笔记整理（4）——紧致性，列紧性](https://zhuanlan.zhihu.com/p/35177017)

（7）

[学弱猹：拓扑学Ⅱ|笔记整理（5）——连通性](https://zhuanlan.zhihu.com/p/35864474)

（8）

[学弱猹：实分析Ⅱ|笔记整理（2）——开集，闭集等集合性质深化](https://zhuanlan.zhihu.com/p/34893497)