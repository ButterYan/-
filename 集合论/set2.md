### **第二章    集合的并、交运算**

>  定义2.1：对于集合 $A$ 和 $B$ ， $\{ x|x\in A$ 或 $x\in B\}$ 称为 $A$ 与 $B$ 的并集记作 $A\cup B$ ，$\{ x|x\in A$ 且 $x\in B\}$ 称为 $A$ 与 $B$ 的交集记作 $A\cap B$ 。 定理2.1（幂等律）： $A\cup A=A$ ， $A\cap A=A$ 。

证：由定义2.1，显然。

>  定理2.2（交换律）： $A\cup B=B\cup A$ ， $A\cap B=B\cap A$ 。

证： $A\cup B=$ $\{ x|x\in A$ 或 $x\in B\}=\{ x|x\in B$ 或 $x\in A\}=B\cup A$ 。

>  定理2.3（结合律）： $(A\cup B)\cup C=A\cup (B\cup C）$, $(A\cap B)\cap C=A\cap (B\cap C)$ 。

证： $(A\cap B)\cap C=$ $\{ x|x\in A\cap B$ 且 $x\in C\} =\{ x|x\in A$ 且 $x\in B$ 且 $x\in C\} =\{ x|x\in A$ 且 $x\in B\cap C\} =A\cap (B\cap C）$。

$(A\cap B)\cap C=\{ x|x\in A\cup B$ 或 $x\in C\} =\{ x|x\in A$ 或 $x\in B$ 或 $x\in C\} =\{ x|x\in A$ 或 $x\in B\cup C\} =A\cup (B\cup C）$。

>  定理2.4：对于集合 $A$ ， $B$ ， $A\cap B\subset A\subset A\cup B$ ， $A\cap B\subset B\subset A\cup B$ 。 证：若 $x\in A\cap B$ ，则 $x\in A$ 且 $x\in B$ ，从而 $x\in A$ ，根据子集的定义可得 $A\cap B\subset A$ 。若 $x\in A$ ，则显然 $x\in A$ 或 $x\in B$ 必成立，从而 $A\subset A\cup B$ 。同理可证另一关系式。 定理2.5（分配律）： $A\cap (B\cup C)=(A\cap B)\cup(A\cap C)$， $A\cup (B\cap C)=(A\cup B)\cap (A\cup C)$ 。

证：若 $x\in A\cap (B\cup C)$ ，则 $x\in A$ 且 $x\in B\cup C$ 。由此可得 $x\in A\cap B$ 或 $x\in A\cap C$ ，即 $x\in(A\cap B)\cup(A\cap C)$ ，从而 $A\cap (B\cup C)\subset(A\cap B)\cup(A\cap C)$ 。若 $x\in (A\cap B)\cup(A\cap C)$ ，则 $x\in A\cap B$ 或 $x\in A\cap C$ 。由此可得$x\in A$ 且 $x\in B\cup C$，因此 $(A\cap B)\cup(A\cap C)\subset A\cap (B\cup C)$ 。综上， $A\cap (B\cup C)=(A\cap B)\cup(A\cap C)$ 得证。

若 $x\in A\cup (B\cap C)$ ，则 $x\in A$ 或 $x\in B\cap C$ 。若 $x\in A$ ，则 $x\in (A\cup B)\cap (A\cup C)$ ；若 $x\in  B\cap C$ ，则 $x\in A\cup B$ 且 $x\in A\cup C$ ，从而， $x\in (A\cup B)\cap (A\cup C)$ 。若 $x\in (A\cup B)\cap (A\cup C)$ ，则 $x\in A\cup B$ 且 $x\in A\cup C$ 。由此可得$x\in A$ 或$x\in B\cap C$，因此 $x\in A\cup (B\cap C)$ 。综上， $A\cup (B\cap C)=(A\cup B)\cap (A\cup C)$ 得证。

>  定义2.2：设 $D$ 是非空集合，对 $D$ 中所有元素 $\alpha$ ，都有一个指标集 $A_{\alpha}$ 与之对应，则这些指标集组成的集合称为以 $D$ 为指标集的集族，记作 $\left\{ A_{\alpha}|\alpha\in D \right\}$ ，简称 $\left\{ A_{\alpha} \right\}$ 。

例2.1：若 $D$ 为自然数集，则 $\left\{ A_{\alpha} \right\}$ 为集列（ $A_{1},A_{2},...,A_{n},...$ ）。

>  定义2.3：对于集族 $\left\{ A_{\alpha} \right\}$ ，若存在 $\alpha$ ，使得 $x\in A_{\alpha}$ ，则称 $x\in\underset{\alpha\in D}{\bigcup}A_{\alpha}$ ，即 $\underset{\alpha\in D}{\bigcup}A_{\alpha}=\{x|\exist \alpha\in D,x\in A_{\alpha}\}$ ；若任意 $\alpha$ ，满足 $x\in A_{\alpha}$ ，则称 $x\in\underset{\alpha\in D}{\bigcap}A_{\alpha}$ ，即 $\underset{\alpha\in D}{\bigcap}A_{\alpha}=\{x|\forall \alpha\in D,x\in A_{\alpha}\}$ 。

由上述无穷交、并的定义，下面结论显然：

>  定理2.6：对于集族 $A_{n}$ 和集合 $B$ ，有： （1）若 $\forall \alpha\in D$ ，有 $B\subset A_{\alpha}$ ，则 $B\subset \underset{\alpha\in D}{\bigcap} A_{\alpha}$ 。 （2）若 $\forall \alpha\in D$ ，有 $A_{\alpha}\subset B$ ，则 $\underset{\alpha\in D}{\bigcup}A_{\alpha}\subset B$ 。

证：（1）若 $x\in B$ ，则 $\forall \alpha\in D$ ， $x\in A_{\alpha}$ ，由无穷交的定义， $x\in \underset{\alpha\in D}{\bigcap} A_{\alpha}$ ，得证。

（2）若 $x\in \underset{\alpha\in D}{\bigcup} A_{\alpha}$ ，由无穷并的定义 ，$\exists \alpha$ ，使得 $x\in A_{\alpha}$ ，由 $A_{\alpha}\subset B$，得 $x\in B$ ，得证。

>  定理2.7：对于一列集合 $A_{n}$ 和集合 $B$ ， （1） $B\cap (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})=\underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cap B)$ ， $B\cup(\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})=\underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cup B)$ 。 （2） $B\cap (\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})=\underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cap B)$ ， $B\cup (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})=\underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cup B)$ 。

证：（1）若 $x\in B\cap (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})$ ，则 $x\in B$ 且 $x\in \underset{n=1}{\overset{\infty}{\bigcup}}A_{n}$ ，则 $\exists n$ ， $x\in A_{n}$ ，故 $x\in A_{n}\cap B$ ，由此 $x\in \underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cap B)$ ，从而 $B\cap (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})\subset\underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cap B)$ 。若 $x\in \underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cap B)$ ，则 $\exists n$，使得 $x\in A_{n}\cap B$ ，从而 $x\in A_{n}$ 且 $x\in B$ ，因此 $x\in B\cap (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})$ ，由此 $\underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cap B)\subset B\cap (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})$ 。综上， $B\cap (\underset{n=1}{\overset{\infty}{\bigcup}}A_{n})=\underset{n=1}{\overset{\infty}{\bigcup}}(A_{n}\cap B)$ 成立，另一结论类似可得。

（2）若 $x\in B\cap (\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})$ ，则 $x\in B$ 且 $x\in \underset{n=1}{\overset{\infty}{\bigcap}}A_{n}$，从而$\forall n$，使得 $x\in A_{n}\cap B$ ，因此 $x\in \underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cap B)$ ， $B\cap (\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})\subset \underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cap B)$ 。若 $x\in \underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cap B)$ ，则$\forall n$，使得 $x\in A_{n}\cap B$ ，因此 $x\in \underset{n=1}{\overset{\infty}{\bigcap}}A_{n}$ ，从而 $x\in B\cap (\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})$ ， $ \underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cap B)\subset B\cap (\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})$ 。综上， $B\cap (\underset{n=1}{\overset{\infty}{\bigcap}}A_{n})= \underset{n=1}{\overset{\infty}{\bigcap}}(A_{n}\cap B)$ 成立，另一结论类似可得。

注：定理2.7（1）是分配律的推广，（2）是结合律的推广；定理2.7的结论推广位指标集族也成立。

>  定理2.8：对于集列 $A_{n}$ 和 $B_{n}$ ，有$(\underset{m=1}{\overset{\infty}{\bigcup}}A_{m})\cap (\underset{n=1}{\overset{\infty}{\bigcup}}B_{n})=\underset{m,n\geq 1}{\bigcup}A_{m}\cap B_{n}$ ，$(\underset{m=1}{\overset{\infty}{\bigcap}}A_{m})\cup (\underset{n=1}{\overset{\infty}{\bigcap}}B_{n})=\underset{m,n\geq 1}{\bigcap}A_{m}\cup B_{n}$ 。

上面的结论利用定理2.7（1）两次即可得证，具体证明略。

### **第三章    集合的差、补运算**

>  定义3.1：对于集合 $A$ ，$B$ 属于集合 $A$ 而不属于集合 $B$ 的元素称为 $A$ 减 $B$ 的差集，记作 $A\setminus B=\{ x\in A$ 且 $x\notin B \}$ ；当 $B\subset A$ 时，则 $A\setminus B$ 也记作 $C_{A}B$ ；当我们讨论的集合都是 $X$ 的子集时，称 $X$ 为全集，$C_{X}B$ 一般记作 $B^{c}$，称作 $B$ 的补集。

注：以下讨论中，我们一般只使用$A\setminus B$ 与 $B^{c}$ 两种符号， $C_{A}B$ 一般不使用，因任何情况下都可以用 $A\setminus B$ 代替；此外，$A\setminus B$ 在一些教材中也记作$A-B$。

例3.1：设 $A$ 是集合，则 $A\setminus A=\emptyset$ ，$A\setminus\emptyset=A$ 。

>  定理3.1：设 $S$ 是全集，集合  $A\subset S$ ，则有： （1） $A\cap A^{c}=\Phi$ ，$A\cup A^{c}=S$ 。 （2）若 $x\in S$ ，则 $x\notin A\Leftrightarrow x\in A^{c}$ ，$x\in A\Leftrightarrow x\notin A^{c}$。 （3） $(A^{c})^{c}=A$ 。

证：（1）若 $\exists x\in A\cap A^{c}$ ，则 $x\in A$ 且 $x\in A^{c}$，由此得出 $x\notin A$ ，矛盾，从而 $A\cap A^{c}=\Phi$ 。显然 $A\cup A^{c}\subset S$ ，而 $\forall x\in S$ ，若 $x\notin A$ ，则有 $x\in \{x|x\in S$ 且 $x\notin A\}=A^{c}$ ，故 $S\subset A\cup A^{c}$ ，综上$A\cup A^{c}=S$ 。

（2）若 $x\notin A$ ，由 $ A^{c}$ 的定义得， $x\in A^{c}$ ，故 $\Rightarrow$ 成立，同理 $\Leftarrow$ 成立。另一命题可将上述结论取逆否命题得到。

（3）由（2）结论得，若 $x\in S$ ，则 $x\in A\Leftrightarrow x\notin A^{c}\Leftrightarrow x\in (A^{c})^{c}$ ，因而得证。

注：如果将 $S$ 为全集的条件去掉，同时将 $A^{c}$ 改为 $S\setminus A$ ，结论仍然成立。

>  定理3.2：若集合 $A,B\subset S$ ，则有 （1） $A\subset B\Leftrightarrow B^{c}\subset A^{c}$ 。 （2） $A\setminus B=A\cap B^{c}$ 。

证：（1）由子集的定义，$\forall x\in A$ ，都有 $x\in B$ ，取逆否命题：若 $x\notin B$ ，则 $x\notin A$ ，这正是 $A\subset B\Leftrightarrow B^{c}\subset A^{c}$ 的定义， $\Rightarrow$ 得证，再根据定理3.1（3）立即可证 $\Leftarrow$ 。

（2）若 $x\in A\setminus B$ ，则 $x\in A$ 且 $x\notin B$ ，由定理3.1（2）， $x\in B^{c}$ ，从而 $x\in A\cap B^{c}$ ，证得 $A\setminus B\subset A\cap B^{c}$ 。若 $x\in A\cap B^{c}$ ，则 $x\in A$ 且 $x\in B^{c}$ ，由定理3.2（2） $x\notin B$ ，从而 $x\in A\setminus B$ ，证得 $A\cap B^{c}\subset A\setminus B$ 。综上， $A\setminus B=A\cap B^{c}$ 。

>  定理3.3：$(A\setminus B)\cap C=A\cap C\setminus B\cap C$ ，$(A\setminus B)\setminus C=A\setminus(B\cup C)$ 。

证：若 $x\in (A\setminus B)\cap C$ ，则 $x\in C$ 且 $x\in A$ ，故 $x\in A\cap C$，另外 $x\notin B$ ，因而 $x\notin B\cap C$ ，故 $(A\setminus B)\cap C\subset A\cap C\setminus B\cap C$；若 $x\in A\cap C\setminus B\cap C$ ，则 $x\in A$ ，且 $x\in C$ ，但 $x\notin B\cap C$ ，因为已经有了 $x\in C$ ，于是 $x\notin B$ ，因此 $A\cap C\setminus B\cap C\subset (A\setminus B)\cap C$ 。

若 $x\in (A\setminus B)\setminus C$ ，则 $x\in A$ ，$x\notin B$ ，$x\notin C$ ，于是 $x\notin B\cup C$ ，因而 $(A\setminus B)\setminus C\subset A\setminus(B\cup C)$ 。若 $x\in A\setminus(B\cup C)$ ，则 $x\in A$，$x\notin B\cup C$ ，于是 $x\notin B$ ，$x\notin C$ ，因此 $A\setminus(B\cup C)\subset (A\setminus B)\setminus C$ 。

>  定理3.4（De Morgan 公式）：若集合 $A,B\subset S$ ，则有 $(A\cup B)^{c}=A^{c}\cap B^{c}$ ， $(A\cap B)^{c}=A^{c}\cup B^{c}$ 。

证：若 $x\in (A\cup B)^{c}$ ，则 $x\notin A\cup B$ ，故 $x\notin A$ 且 $x\notin B$ ，故$x\in A^{c}$ 且 $x\in B^{c}$，从而 $(A\cup B)^{c}\subset A^{c}\cap B^{c}$ 。

若 $x\in A^{c}\cap B^{c}$ ，则$x\notin A$ 且 $x\notin B$ ，从而 $x\notin A\cup B$ ，$x\in (A\cup B)^{c}$ ，综上， $(A\cup B)^{c}=A^{c}\cap B^{c}$ 。

若 $x\in (A\cap B)^{c}$ ，则 $x\notin A\cap B$ ，故 $x\notin A$ 或 $x\notin B$ ，故$x\in A^{c}$ 或 $x\in B^{c}$，从而 $(A\cap B)^{c}\subset A^{c}\cup B^{c}$ 。

若 $x\in A^{c}\cup B^{c}$ ，则$x\notin A$ 或 $x\notin B$ ，从而 $x\notin A\cap B$ ，$x\in (A\cap B)^{c}$ ，综上， $(A\cup B)^{c}=A^{c}\cap B^{c}$ 。

>  定理3.5：设 $\left\{  A_{\alpha}\right\}$ 为指标集族， $S$ 为全集，则 $(\underset{\alpha\in D}{\bigcup}A_{\alpha})^{c}=\underset{\alpha\in D}{\bigcap}A_{\alpha}^{c}$ ， $(\underset{\alpha\in D}{\bigcap}A_{\alpha})^{c}=\underset{\alpha\in D}{\bigcup}A_{\alpha}^{c}$ 。

定理3.5可看做定理3.4的推广，不再给出证：。更一般地，有下面的结论：

>  定理3.6：$A\setminus(\underset{\alpha\in D}{\bigcup}A_{\alpha})=\underset{\alpha\in D}{\bigcap}A\setminus A_{\alpha}$ ，$A\setminus(\underset{\alpha\in D}{\bigcap}A_{\alpha})=\underset{\alpha\in D}{\bigcup}A\setminus A_{\alpha}$ 。

证：首先， $A\setminus A_{\alpha}=A\cap(A\setminus A_{\alpha})=(A\cap A)\setminus (A\cap A_{\alpha})=A\setminus (A\cap A_{\alpha})$ ，由定理2.6可得 $A\setminus(\underset{\alpha\in D}{\bigcup}A_{\alpha})=A\setminus(\underset{\alpha\in D}{\bigcup}A_{\alpha}\cap A)=A\setminus[\underset{\alpha\in D}{\bigcup}(A_{\alpha}\cap A)]$ ，$A\setminus(\underset{\alpha\in D}{\bigcap}A_{\alpha})=A\setminus(\underset{\alpha\in D}{\bigcap}A_{\alpha}\cap A)=A\setminus[\underset{\alpha\in D}{\bigcap}(A_{\alpha}\cap A)]$ ，这样，我们就把 $A$ 看作全集，利用定理3.5得证。

至此，我们已经讲完了集合的并、交、差、补运算。在全集明确的情况下，由定义3.1，补运算可由差运算得到；由定理3.2（2），差运算可由补运算和交运算复合达到；由定理3.4，交运算可由补运算与并运算得到，并运算可由补运算与交运算得到。由此，我们可以说，集合的以上四种运算可以归结为其中两种，我们只需取并、交运算中的一种，差、补运算中的一种，经过复合即可得到剩下的运算。以下，我们补充一下集合的对称差运算。

>  定义3.2：对于集合 $A,B$ ， $(A\setminus B)\cup(B\setminus A)$ 称为它们的对称差，记作 $A\triangle B$ 。

对称差描述了两个集合不相交的部分，因对称差是之前我们讨论的运算的复合，它的性质相信读者能够自行证：

>  定理3.7：（1） $A\triangle B=(A\cup B)\setminus(A\cap B)=(A\cap B^{c})\cup(B\cap A^{c})=A^{c}\triangle B^{c}$ 。（2）$A\triangle B=\emptyset \Leftrightarrow A=B$ 。（3）$A\triangle B=B\triangle A$ 。（4） $(A\triangle B)\triangle C=A\triangle (B\triangle C)$ 。