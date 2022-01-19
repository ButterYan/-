Fisher信息量：$I(\theta)=E_\theta(\frac{\partial \ln f(X,\theta)}{\partial \theta})^2$

引理1：$E_\theta(\frac{\partial \ln f(X,\theta)}{\partial \theta})=0$

证：

$I(\theta)=-E_\theta(\frac{\partial^2 \ln f(X,\theta)}{\partial \theta^2})$

证明：$I(\theta)=E_\theta(\frac{\partial \ln f(X,\theta)}{\partial \theta})^2=\int(\frac{\partial \ln f(X,\theta)}{\partial \theta})^2f(x)dx=\int\frac{\partial \ln f(X,\theta)}{\partial \theta}\frac{\partial f(x,\theta)}{\partial\theta}dx$

发现 $\frac{\partial}{\partial \theta}[\frac{\partial \ln f(X,\theta)}{\partial \theta}f(x,\theta)]=\frac{\partial \ln f(X,\theta)}{\partial \theta}\frac{\partial f(x,\theta)}{\partial\theta}+\frac{\partial^2 \ln f(X,\theta)}{\partial \theta^2}f(x,\theta)$

因此 $I(\theta)=\int\frac{\partial}{\partial \theta}[\frac{\partial \ln f(X,\theta)}{\partial \theta}f(x,\theta)]dx-\int\frac{\partial^2 \ln f(X,\theta)}{\partial \theta^2}f(x,\theta)dx=\frac{\partial}{\partial \theta}E_\theta(\frac{\partial \ln f(X,\theta)}{\partial \theta})-E_\theta(\frac{\partial^2 \ln f(X,\theta)}{\partial \theta^2})$