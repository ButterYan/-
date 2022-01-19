### **第九章    点集中点的分类**

> 定义9.1.1（拓扑学中的邻域）：设 $(X,\Im)$ 是拓扑空间, $x\in X$ ， $U$是 $X$ 的一个子集，满足: 存在一 个开集 $V\in \Im$ 使得 $x\in V\subset U$ ，则称 $U$ 为 $x$的一个邻域。 定义9.1.2（分析中的球形邻域）：设 $x:(x_{1},x_{2},...x_{n})$ 为欧式空间 $R^{n}$ 中一点，令 $U=\left\{ (y_{1},y_{2},...y_{n})|\sqrt{\sum_{i=1}^{n}{(x_{i}-y_{i})^{2}}}<\delta \right\}$ ，则称 $U$ 为点 $x$ 的 $\delta$ 球形邻域。 定义9.1.3（分析中的方形邻域）：设 $x:(x_{1},x_{2},...x_{n})$ 为欧式空间 $R^{n}$ 中一点，令 $U=\left\{ (y_{1},y_{2},...y_{n})|max(\left|x_{i}-y_{i}  \right|)<\delta \right\}$ ，则称 $U$ 为点 $x$ 的 $\delta$ 方形邻域。

​       在分析与拓扑中定义了不同的邻域，个人认为，邻域的本质是开集，拓扑中的邻域中真正奇效的概念是开集 $V$ ，鉴于点集的性质在多数教材中没有详细介绍，笔者试图通过集合的概念给出系统的论述。我们首先设 $X$ 为研究的点集全集， $A\subset X$，在此基础上研究点集的分类。第一分类法，将 $X$ 上的点分成内点，边界点，外点；第二分类法，将 $X$ 上的点分成聚点，孤立点，外点。其中外点不是我们主要关注的对象，另外两类点统称相关点（我独创的概念），接下来分别证明两种分类法能够完成分类（下文称分类的正当性），每一类别的点与 $A$ 的关系，以及两种分类之间的关系。

> 定义9.2：设 $X$ 为研究的点集全集， $A\subset X$ ， $A$ 的补集记作 $A^{c}$ ，对于点 $x\in X$ ： （1）若存在 $x$ 的邻域 $U_{x}$ ，满足 $U_{x}\subset A$ ，则称 $x$ 为 $A$ 的内点；$A$ 的内点构成的集合称为 $A$ 的内部，记作 $A^{\circ}$ 。 （2）若任意 $x$ 的邻域 $U_{x}$ ，满足 $U_{x}\cap A\ne \Phi$ 且 $U_{x}\cap A^{c}\ne \Phi$ ，则称 $x$ 为 $A$ 的边界点；$A$ 的边界点构成的集合称为 $A$ 的边界，记作 $\partial A$ 。 （3）若存在 $x$的邻域 $U_{x}$ ，满足 $U_{x}\cap A=\Phi$ ，则称 $x$ 为 $A$ 的外点；$A$ 的外点构成的集合称为 $A$ 的外部。 （4）若任意 $x$ 的邻域 $U_{x}$ ， $U_{x}\cap A\ne \Phi$ ，则称 $x$ 为 $A$ 的相关点，相关点构成的集合记作 $Rel(A)$ 。 定理9.1：设 $X$ 为研究的点集全集， $A\subset X$ ， $A$ 的补集记作 $A^{c}$ ，对于点 $x\in X$： （1）若$x$ 为 $A$ 的内点，则 $x$ 是 $A^{c}$ 的外点。 （2）若$x$ 为 $A$ 的外点，则 $x$ 是 $A^{c}$ 的内点。 （3）若$x$ 为 $A$ 的边界点，则 $x$ 是 $A^{c}$ 的边界点。

证：先证明 $U_{x}\subset A\Leftrightarrow$ $U_{x}\cap A^{c}=\Phi$ ：由于 $U_{x}\subset A$ ，$\forall a\in U_{x}$ ，都有 $a\in A$ ， $a\notin A^{c}$ ， $\Rightarrow$ 得证；由于 $U_{x}\cap A^{c}=\Phi$ ，$\forall a\in U_{x}$ ， $a\notin A^{c}$ ，$a\in A$ ， $\Leftarrow$ 得证。由此证明：

（1）由定义与上述结论，存在 $x$ 的邻域 $U_{x}$ ，满足 $U_{x}\cap A^{c}=\Phi$ ，恰好符合 $A^{c}$ 的外点的定义，得证。

（2）由定义与上述结论，存在 $x$ 的邻域 $U_{x}$ ，满足 $U_{x}\subset A^{c}$ ，恰好符合 $A^{c}$ 的内点的定义，得证。

（3）由于 $A=(A^{c})^{c}$ ，根据定义，显然得证。

​       我们前面证明的集合关系，给出了另一种一种内点与外电的定义方法，定义9.1是基于集合 $A$ 本身定义的，而这里是基于补集 $A^{c}$ 定义的；我们因而可以用 $(A^{c})^{\circ}$ 表示 $A$ 的外部。

> 推论9.1：设 $X$ 为研究的点集全集， $A\subset X$ ， $A^{\circ}\subset A$ ， $(A^{c})^{\circ}\subset A^{c}$ 。

证：设 $x\in A^{\circ}$ ，由内点定义有 $x\in U_{x}\subset A$ ，即得证，外点集同理可得。

> 定理9.2（第一分类法的正当性）：设 $X$ 为研究的点集全集， $A\subset X$ ， 对于点 $x\in X$ ， $x$ 必是内点、边界点、外点中的一种，即 $X=A^{\circ}\cup\partial A\cup(A^{c})^{\circ}$ ， $A^{\circ}\cap\partial A=\Phi$ ， $A^{\circ}\cap(A^{c})^{\circ}=\Phi$ ， $\partial A\cap(A^{c})^{\circ}=\Phi$ 。

证：先假设 $x$ 既不是内点，也不是外点，结合以上给出的两种定义，有任意 $x$ 的邻域 $U_{x}$，都有 $U_{x}\cap A\ne \Phi$ 和 $U_{x}\cap A^{c}\ne \Phi$ ，恰好满足边界点的定义，证得了，任何点都至少包含于这三种点当中的一种，接下来证明它不能同时属于两种。假设 $x\in \partial A$ ，由定义有$U_{x}\cap A\ne \Phi$ 且 $U_{x}\cap A^{c}\ne \Phi$ ，与 $x$ 是内点和外点的定义是矛盾的，因而有$A^{\circ}\cap\partial A=\Phi$ ， $\partial A\cap(A^{c})^{\circ}=\Phi$ ；最后再假设 $x\in A^{\circ}\cap(A^{c})^{\circ}$ ，则存在邻域 $U_{x}$ ，使得 $U_{x}\cap A=\Phi$ ， $U_{x}\cap A^{c}=\Phi$ ，从而推出 $U_{x}=\Phi$ ，与邻域定义矛盾，从而 $A^{\circ}\cap(A^{c})^{\circ}=\Phi$ 。

> 定理9.3：设 $X$ 为研究的点集全集， $A\subset X$ ： （1）$Rel(A)=A^{\circ}\cup\partial A$ 。 （2） $A\subset Rel(A)$ 。

证：（1）我们先假设 $x\in Rel(A)$ ，但 $x\notin \partial A$ ，由定义有$U_{x}\cap A\ne \Phi$ 且 $U_{x}\cap A^{c}= \Phi$ ，那么 $U_{x}\cap A^{c}=U_{x}$ ，即 $U_{x}\subset A$ ，$x\in A^{\circ}$ ，也就证出了 $Rel(A)\subset A^{\circ}\cup\partial A$ 。假设 $x\in A^{\circ}$ ，由定义知 $U_{x}\subset A$ ， $U_{x}\cap A\ne \Phi$ ，得 $x\in Rel(A)$ ；若 $x\in \partial A$ ，由定义也有$U_{x}\cap A\ne \Phi$ ，得 $x\in Rel(A)$ ，故得证。

（2）显然 $Rel(A)^{c}=(A^{c})^{\circ}\subset A^{c}$ ，有补集的性质，得证。

> 推论9.2：设 $X$ 为研究的点集全集， $A\subset X$ ，$Rel(A)\cup (A^{c})^{\circ}=X$ ， $Rel(A^{c})\cup A^{\circ}=X$ 。

证明：由定理9.3（1），显然。

> 定义9.3：设 $X$ 为研究的点集全集， $A\subset X$ ， 对于点 $x\in X$： （1）若任何 $x$ 的邻域 $U_{x}$ ， $(U_{x}-\left\{ x \right\})\cap A\ne \Phi$ ，则称 $x$ 为 $A$ 的聚点，聚点构成的集合称作导集，记作 $A^{'}$ 。 （2）若 $x\in A$ ， $x\notin A^{'}$，则称 $x$ 为 $A$ 的孤立点。 定理9.4（第二分类法的正当性）：设 $X$ 为研究的点集全集， $A\subset X$ ， 对于点 $x\in Rel(A)$，有 $x$ 不是聚点就是孤立点。

证：由定义可知， $x$ 不会既是聚点又是孤立点；那么我们假设 $x\notin A^{'}$ ，由定义得任存在 $x$ 的邻域 $U_{x}$ ， $(U_{x}-\left\{ x \right\})\cap A\ne \Phi$， $U_{x}\cap A\ne \Phi$ ，从而得 $\left\{ x \right\}\cap A\ne \Phi$ ，自然地，$x\in A$， $x$ 是$A$ 的孤立点，得证。

> 定理9.5（有争议）：设 $X$ 为研究的点集全集， $A\subset X$ ： （1）内点都是聚点。 （2）孤立点都是边界点。

证：（1）设 $x$ 是内点，则存在邻域 $U_{x1}\subset A$ ，对于任何邻域 $U_{x}$ ，由于 $(U_{x}-\left\{ x \right\})\cap U_{x1}\ne \Phi$ ， $(U_{x}-\left\{ x \right\})\cap U_{x1}\subset (U_{x}-\left\{ x \right\})\cap A$ ，得 $(U_{x}-\left\{ x \right\})\cap A\ne \Phi$ ，从而是聚点。

（2）设 $x$ 是孤立点，则任何 $x$ 的邻域 $U_{x}$ ， $(U_{x}-\left\{ x \right\})\cap A=\Phi$ ，$\left\{ x \right\}\cap A=\left\{ x \right\}\ne\Phi$ ，得 $U_{x}\cap A\ne\Phi$ ；由补集公式得， $(U_{x}-\left\{ x \right\})\cap A^{c}=U_{x}-\left\{ x \right\}\ne \Phi$ ，即 $U_{x}\cap A^{c}\ne \Phi$ ，满足边界点定义。

注：上述结论在拓扑空间中需要添加条件： $\left\{ x \right\}$ 不是一个邻域（开集）才能够成立，本文的探讨都默认这一条件。

> 定义9.4：设 $X$ 为研究的点集全集， $A\subset X$ ， $A^{'}\cup A$ 称为 $A$ 的闭包，记作 $\bar{A}$ 。 定理9.5：设 $X$ 为研究的点集全集， $A\subset X$ ， $\bar{A}=Rel(A)$ 。

证：设 $x\in Rel(A)$ ，则 $x\in A^{'}$ 或 $x$ 是孤立点，显然若是孤立点，则 $x\in A$ ，因此， $Rel(A)\subset \bar{A}$ 。再假设 $x\in \bar{A}$ ，则$x\in A^{'}$ 或 $x\in A$ ，结合定理9.3（2），易得 $\bar{A}\subset Rel(A)$ ，由此得证。

​       这样，我们就证明了闭包与相关点集的等价性，上述所有关于 $Rel(A)$ 的性质关于 $\bar{A}$ 同样成立，最重要的还是补集性质： $\bar{A}^{c}=(A^{c})^{\circ}$ ，请读者深入理解，这个性质将在下一章的证明中配合定理3.3被反复用到。

> 例9.1：定义二维欧式空间中的集合 $E_{1}=\left\{ (0,0) \right\}\cup \left\{ (x,y)|x^{2}+y^{2}>1 \right\}$ ，其内部：$\left\{ (x,y)|x^{2}+y^{2}>1 \right\}$ ，边界： $\left\{ (x,y)|x^{2}+y^{2}=1 \right\}\cup\left\{ (0,0) \right\}$ ，外部 ：$\left\{ (x,y)|0<x^{2}+y^{2}<1 \right\}$ ，闭包： $\left\{ (x,y)|x^{2}+y^{2}\geq1 \right\}\cup\left\{ (0,0) \right\}$ ，聚点： $\left\{ (x,y)|x^{2}+y^{2}\geq1 \right\}$ ，孤立点： $\left\{ (0,0) \right\}$ 。$E_{2}=\left\{ (x,y)|x^{2}+y^{2}\geq1 \right\}\cup\left\{ (0,0) \right\}$，如将集合 $E_{1}$ 换为 $E_{2}$ 上述结论完全不变，请读者自行验证。

总结：本章，我们采用了另外一种顺序阐述了点的分类体系，设 $X$ 为研究的点集全集， $A\subset X$ ， 将点分成两大类，一类是外点，一类称为相关点，定理9.5告诉我们相关点的集合与闭包是等价的，以后的讨论将只使用闭包，外点不是我们研究 $A$ 时感兴趣的点，而闭包中的点是我们感兴趣的，由此衍生出两大分类法。第一类将闭包分成内点和边界点，这一类分发使得 $A$ 与 $A^{c}$ 产生了对称性（定理9.1），同时内点一定是属于 $A$ 的，而边界点不见得属于 $A$ 。第二类将闭包分成了聚点和边界点，在特定条件下，聚点包含了全部的内点，同时边界点包含了全部的孤立点。下文将在分类的基础上探讨开集和闭集的性质。