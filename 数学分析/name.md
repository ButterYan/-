笔者看过这样两个问题。

怎么推导或证明 e^x 的导数是自身？www.zhihu.com![图标](https://pic4.zhimg.com/v2-56ee66384cb80f442090ecd3defc4e6f_180x120.jpg)

如何证明lnx的导数是1/x？www.zhihu.com![图标](https://zhstatic.zhihu.com/assets/zhihu/editor/zhihu-card-default.svg)

下面我们尝试使用定义法证明一下：

![(e^{x})'=\underset{\Delta x \rightarrow 0}\lim\frac{e^{x+\Delta x}-e^{x}}{\Delta x}=e^{x}\underset{\Delta x \rightarrow 0}\lim \frac{e^{\Delta x}-1}{\Delta x}](https://www.zhihu.com/equation?tex=(e%5E%7Bx%7D)%27%3D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7Be%5E%7Bx%2B%5CDelta%20x%7D-e%5E%7Bx%7D%7D%7B%5CDelta%20x%7D%3De%5E%7Bx%7D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%20%5Cfrac%7Be%5E%7B%5CDelta%20x%7D-1%7D%7B%5CDelta%20x%7D)(e^{x})'=\underset{\Delta x \rightarrow 0}\lim\frac{e^{x+\Delta x}-e^{x}}{\Delta x}=e^{x}\underset{\Delta x \rightarrow 0}\lim \frac{e^{\Delta x}-1}{\Delta x} 

![(\ln x)'=\underset{\Delta x \rightarrow 0}\lim\frac{\ln(x+\Delta x)-\ln x}{\Delta x}=\underset{\Delta x \rightarrow 0}\lim\frac{\ln(1+\frac{\Delta x}{x})}{\Delta x}](https://www.zhihu.com/equation?tex=(%5Cln%20x)%27%3D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(x%2B%5CDelta%20x)-%5Cln%20x%7D%7B%5CDelta%20x%7D%3D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2B%5Cfrac%7B%5CDelta%20x%7D%7Bx%7D)%7D%7B%5CDelta%20x%7D)(\ln x)'=\underset{\Delta x \rightarrow 0}\lim\frac{\ln(x+\Delta x)-\ln x}{\Delta x}=\underset{\Delta x \rightarrow 0}\lim\frac{\ln(1+\frac{\Delta x}{x})}{\Delta x} 

令 ![t=\frac{\Delta x}{x}](https://www.zhihu.com/equation?tex=t%3D%5Cfrac%7B%5CDelta%20x%7D%7Bx%7D)t=\frac{\Delta x}{x} ，则原极限化为 ![\frac 1 x\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}](https://www.zhihu.com/equation?tex=%5Cfrac%201%20x%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2Bt)%7D%7Bt%7D)\frac 1 x\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t} 

那么问题来了，极限 ![\underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x}](https://www.zhihu.com/equation?tex=%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7Be%5E%7B%5CDelta%20x%7D-1%7D%7B%5CDelta%20x%7D)\underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x} 和 ![\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}](https://www.zhihu.com/equation?tex=%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2Bt)%7D%7Bt%7D)\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t} 等于几呢？

**我们记** ![I_{1}=\underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x}](https://www.zhihu.com/equation?tex=I_%7B1%7D%3D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7Be%5E%7B%5CDelta%20x%7D-1%7D%7B%5CDelta%20x%7D)**I_{1}=\underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x}** **，** ![I_{2}=\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}](https://www.zhihu.com/equation?tex=I_%7B2%7D%3D%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2Bt)%7D%7Bt%7D)**I_{2}=\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}** 

可以发现，令 ![t=e^{\Delta x}-1](https://www.zhihu.com/equation?tex=t%3De%5E%7B%5CDelta%20x%7D-1)t=e^{\Delta x}-1 ， ![I_{1}=\underset{\Delta x \rightarrow 0}\lim\frac{t}{\ln(1+t)}=\frac{1}{I_{2}}](https://www.zhihu.com/equation?tex=I_%7B1%7D%3D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7Bt%7D%7B%5Cln(1%2Bt)%7D%3D%5Cfrac%7B1%7D%7BI_%7B2%7D%7D)I_{1}=\underset{\Delta x \rightarrow 0}\lim\frac{t}{\ln(1+t)}=\frac{1}{I_{2}} 。

这样，两个极限问题可以理解为同一个问题。

## 下面先给出几种**错误**的做法：

错误做法一：

利用等价无穷小 ![e^{x}-1\sim x](https://www.zhihu.com/equation?tex=e%5E%7Bx%7D-1%5Csim%20x)e^{x}-1\sim x ， ![\ln(1+x)\sim x](https://www.zhihu.com/equation?tex=%5Cln(1%2Bx)%5Csim%20x)\ln(1+x)\sim x ，所以 ![I_{1}=I_{2}=1](https://www.zhihu.com/equation?tex=I_%7B1%7D%3DI_%7B2%7D%3D1)I_{1}=I_{2}=1 。

解析：

我们观察等价无穷小的定义：若 ![f(x)](https://www.zhihu.com/equation?tex=f(x))f(x) 与 ![g(x)](https://www.zhihu.com/equation?tex=g(x))g(x) 为自变量在同一极限过程中的无穷小量，并有 ![\frac{f(x)}{g(x)}\rightarrow 1](https://www.zhihu.com/equation?tex=%5Cfrac%7Bf(x)%7D%7Bg(x)%7D%5Crightarrow%201)\frac{f(x)}{g(x)}\rightarrow 1 则称![f(x)](https://www.zhihu.com/equation?tex=f(x))f(x) 与 ![g(x)](https://www.zhihu.com/equation?tex=g(x))g(x)为等价无穷小。

我们发现，等价无穷小就是用两者商的极限为 ![1](https://www.zhihu.com/equation?tex=1)1 定义的，上述做法说两者是等价无穷小，仅仅是把待证明的东西换一种说法说了一遍，并没有做出实质性证明。

错误做法二：

利用洛必达法则： ![I_{1}=\lim_{\Delta x \rightarrow 0}{\frac{e^{\Delta x}-1}{\Delta x}}=\lim_{\Delta x \rightarrow 0}{\frac{e^{\Delta x}}{1}}=1](https://www.zhihu.com/equation?tex=I_%7B1%7D%3D%5Clim_%7B%5CDelta%20x%20%5Crightarrow%200%7D%7B%5Cfrac%7Be%5E%7B%5CDelta%20x%7D-1%7D%7B%5CDelta%20x%7D%7D%3D%5Clim_%7B%5CDelta%20x%20%5Crightarrow%200%7D%7B%5Cfrac%7Be%5E%7B%5CDelta%20x%7D%7D%7B1%7D%7D%3D1)I_{1}=\lim_{\Delta x \rightarrow 0}{\frac{e^{\Delta x}-1}{\Delta x}}=\lim_{\Delta x \rightarrow 0}{\frac{e^{\Delta x}}{1}}=1 

![I_{2}=\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}= \underset{t\rightarrow 0}\lim\frac{\frac{1}{1+t}}{1}=1](https://www.zhihu.com/equation?tex=I_%7B2%7D%3D%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2Bt)%7D%7Bt%7D%3D%20%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cfrac%7B1%7D%7B1%2Bt%7D%7D%7B1%7D%3D1)I_{2}=\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}= \underset{t\rightarrow 0}\lim\frac{\frac{1}{1+t}}{1}=1 

解析：

使用洛必达法则时涉及到了求导，已经利用到了他们的导数公式，而我们的导数公式又依赖于这两个极限的值，循环论证。

## 下面给出正确做法：

定义：定义数列 ![x_{n}=\underset{n\rightarrow \infty}\lim(1+\frac{1}{n})^{n}](https://www.zhihu.com/equation?tex=x_%7Bn%7D%3D%5Cunderset%7Bn%5Crightarrow%20%5Cinfty%7D%5Clim(1%2B%5Cfrac%7B1%7D%7Bn%7D)%5E%7Bn%7D)x_{n}=\underset{n\rightarrow \infty}\lim(1+\frac{1}{n})^{n} ，记 ![e=\underset{n\rightarrow \infty}\lim x_n](https://www.zhihu.com/equation?tex=e%3D%5Cunderset%7Bn%5Crightarrow%20%5Cinfty%7D%5Clim%20x_n)e=\underset{n\rightarrow \infty}\lim x_n 。

引理1： ![\underset{x\rightarrow \infty}\lim(1+\frac{1}{x})^{x}=e](https://www.zhihu.com/equation?tex=%5Cunderset%7Bx%5Crightarrow%20%5Cinfty%7D%5Clim(1%2B%5Cfrac%7B1%7D%7Bx%7D)%5E%7Bx%7D%3De)\underset{x\rightarrow \infty}\lim(1+\frac{1}{x})^{x}=e （这里的 ![x](https://www.zhihu.com/equation?tex=x)x 视作函数的自变量，本引理实现了从数列极限到函数极限的转化）。

证明思路：我们可以将上函数极限进行取整放缩到数列极限 ![x_{n}](https://www.zhihu.com/equation?tex=x_%7Bn%7D)x_{n} 再利用夹逼准则得 ![\underset{x\rightarrow +\infty}\lim(1+\frac{1}{x})^{x}=e](https://www.zhihu.com/equation?tex=%5Cunderset%7Bx%5Crightarrow%20%2B%5Cinfty%7D%5Clim(1%2B%5Cfrac%7B1%7D%7Bx%7D)%5E%7Bx%7D%3De)\underset{x\rightarrow +\infty}\lim(1+\frac{1}{x})^{x}=e ，再利用负代换将负无穷时的极限转化为正无穷时的极限。（具体证明略）

引理2： ![\underset{x\rightarrow 0}\lim(1+x)^{\frac{1}{x}}=e](https://www.zhihu.com/equation?tex=%5Cunderset%7Bx%5Crightarrow%200%7D%5Clim(1%2Bx)%5E%7B%5Cfrac%7B1%7D%7Bx%7D%7D%3De)\underset{x\rightarrow 0}\lim(1+x)^{\frac{1}{x}}=e 。

证明：对引理1的结果做倒数代换即可得。

接下来， ![I_{2}=\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}= \underset{t\rightarrow 0}\lim\frac{1}{t}\ln(1+t)=\underset{t\rightarrow 0}\lim \ln(1+t)^{\frac{1}{t}}](https://www.zhihu.com/equation?tex=I_%7B2%7D%3D%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2Bt)%7D%7Bt%7D%3D%20%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B1%7D%7Bt%7D%5Cln(1%2Bt)%3D%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%20%5Cln(1%2Bt)%5E%7B%5Cfrac%7B1%7D%7Bt%7D%7D)I_{2}=\underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}= \underset{t\rightarrow 0}\lim\frac{1}{t}\ln(1+t)=\underset{t\rightarrow 0}\lim \ln(1+t)^{\frac{1}{t}} 

![=\ln(\underset{x\rightarrow 0}\lim(1+x)^{\frac{1}{x}})=\ln e=1](https://www.zhihu.com/equation?tex=%3D%5Cln(%5Cunderset%7Bx%5Crightarrow%200%7D%5Clim(1%2Bx)%5E%7B%5Cfrac%7B1%7D%7Bx%7D%7D)%3D%5Cln%20e%3D1)=\ln(\underset{x\rightarrow 0}\lim(1+x)^{\frac{1}{x}})=\ln e=1 

![I_{1}=\underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x}](https://www.zhihu.com/equation?tex=I_%7B1%7D%3D%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7Be%5E%7B%5CDelta%20x%7D-1%7D%7B%5CDelta%20x%7D)I_{1}=\underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x} ，令 ![t=e^{\Delta x}-1](https://www.zhihu.com/equation?tex=t%3De%5E%7B%5CDelta%20x%7D-1)t=e^{\Delta x}-1 ，

![I_{1}=\underset{\Delta t \rightarrow 0}\lim \frac{t}{\ln(1+t)}=\frac{1}{I_{2}}=1](https://www.zhihu.com/equation?tex=I_%7B1%7D%3D%5Cunderset%7B%5CDelta%20t%20%5Crightarrow%200%7D%5Clim%20%5Cfrac%7Bt%7D%7B%5Cln(1%2Bt)%7D%3D%5Cfrac%7B1%7D%7BI_%7B2%7D%7D%3D1)I_{1}=\underset{\Delta t \rightarrow 0}\lim \frac{t}{\ln(1+t)}=\frac{1}{I_{2}}=1 。

综上：

![(e^{x})'=e^{x}I_{1}=e^{x}](https://www.zhihu.com/equation?tex=(e%5E%7Bx%7D)%27%3De%5E%7Bx%7DI_%7B1%7D%3De%5E%7Bx%7D)(e^{x})'=e^{x}I_{1}=e^{x} 

![(\ln x)'= \frac{1}{x}I_{2}=\frac{1}{x}](https://www.zhihu.com/equation?tex=(%5Cln%20x)%27%3D%20%5Cfrac%7B1%7D%7Bx%7DI_%7B2%7D%3D%5Cfrac%7B1%7D%7Bx%7D)(\ln x)'= \frac{1}{x}I_{2}=\frac{1}{x} 

逻辑链：

![e=\underset{n\rightarrow \infty}\lim(1+\frac{1}{n})^{n}\Rightarrow\underset{x\rightarrow \infty}\lim(1+\frac{1}{x})^{x}=e](https://www.zhihu.com/equation?tex=e%3D%5Cunderset%7Bn%5Crightarrow%20%5Cinfty%7D%5Clim(1%2B%5Cfrac%7B1%7D%7Bn%7D)%5E%7Bn%7D%5CRightarrow%5Cunderset%7Bx%5Crightarrow%20%5Cinfty%7D%5Clim(1%2B%5Cfrac%7B1%7D%7Bx%7D)%5E%7Bx%7D%3De)e=\underset{n\rightarrow \infty}\lim(1+\frac{1}{n})^{n}\Rightarrow\underset{x\rightarrow \infty}\lim(1+\frac{1}{x})^{x}=e 

![\Rightarrow \underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}= 1\Rightarrow \underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x}=1](https://www.zhihu.com/equation?tex=%5CRightarrow%20%5Cunderset%7Bt%5Crightarrow%200%7D%5Clim%5Cfrac%7B%5Cln(1%2Bt)%7D%7Bt%7D%3D%201%5CRightarrow%20%5Cunderset%7B%5CDelta%20x%20%5Crightarrow%200%7D%5Clim%5Cfrac%7Be%5E%7B%5CDelta%20x%7D-1%7D%7B%5CDelta%20x%7D%3D1)\Rightarrow \underset{t\rightarrow 0}\lim\frac{\ln(1+t)}{t}= 1\Rightarrow \underset{\Delta x \rightarrow 0}\lim\frac{e^{\Delta x}-1}{\Delta x}=1

![\Rightarrow](https://www.zhihu.com/equation?tex=%5CRightarrow)\Rightarrow ![(e^{x})'=e^{x},(\ln x)'=\frac{1}{x}](https://www.zhihu.com/equation?tex=(e%5E%7Bx%7D)%27%3De%5E%7Bx%7D%2C(%5Cln%20x)%27%3D%5Cfrac%7B1%7D%7Bx%7D)(e^{x})'=e^{x},(\ln x)'=\frac{1}{x} 