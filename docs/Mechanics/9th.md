# 第九次习题

## 7.4 如果保留泰勒展开(7.114) 中的二阶小量，请重新推导波$ψ(x, t)$.

$$\begin{aligned} \psi(x,t) \approx \int_{-\infty}^{\infty}\exp\Big[-\frac{(k-k_{0})^{2}}{2\sigma^{2}}\Big]e^{ikx - i\omega(k_{0})t -i\omega^{\prime}(k_{0})(k-k_{0})t- \frac{1}{2}i\omega''(k_0)(k-k_0)^2t } ~dk \end{aligned}$$

$$\quad =\begin{aligned} \sqrt{2\pi}\exp\Big[-\frac12(k-k_0)^2\left(\frac1{\sigma^2}+i\omega^{\prime\prime}(k_0)t\right)-i(\omega^{\prime}(k_0)t)(k-k_0)+ik_0x\Big] \end{aligned}$$

$\quad =\begin{aligned} \sqrt{2\pi}\exp\Big[-\frac12\left(\frac1{\sigma^2}+i\omega^{\prime\prime}(k_0)t\right)[(k-k_0)+\frac{i(\omega^{\prime}(k_0)t)}{\frac1{\sigma^2}+i\omega^{\prime\prime}(k_0)t}]^2+\frac12(\frac{i(\omega^{\prime}(k_0)t)}{\frac1{\sigma^2}+i\omega^{\prime\prime}(k_0)t})^2 + ik_0x\Big] \end{aligned}$

$\quad =\begin{aligned} \sqrt{2\pi}\exp\Big[\frac12\frac{-(\omega^{\prime}(k_0)t)^2}{(\frac1{\sigma^2}+i\omega^{\prime\prime}(k_0)t)^2} + ik_0x\Big] \end{aligned} $



## 8.1

$$
\begin{equation}
    \begin{cases}
   		\frac{dx_1}{dt}=\{x_1,H\},\quad\frac{dp_1}{dt}=\{p_1,H\} ,\\
   		\frac{dx_2}{dt}=\{x_2,H\},\quad\frac{dp_2}{dt}=\{p_2,H\} ,\\
   		\frac{dx_3}{dt}=\{x_3,H\},\quad\frac{dp_3}{dt}=\{p_3,H\} .
    \end{cases}
\end{equation}
$$

且
$$
\frac{dx}{dt}=\frac{\partial x}{\partial x}\frac{\partial H}{\partial p}-\frac{\partial x}{\partial p}\frac{\partial H}{\partial x}=\frac{\partial H}{\partial p} \\
\frac{dp}{dt}=\frac{\partial p}{\partial x}\frac{\partial H}{\partial p}-\frac{\partial p}{\partial p}\frac{\partial H}{\partial x}=-\frac{\partial H}{\partial x} \\
H=\frac{p_1^2}{2m_1}+\frac{p_2^2}{2m_2}+\frac{p_3^2}{2m_3}+V_0\big[e^{(x_1-x_2)/r_0}+e^{(x_2-x_3)/r_0}+e^{(x_3-x_1)/r_0}\big]
$$


即
$$
\begin{equation}
    \begin{cases}
   		\frac{dx_1}{dt}=\{x_1,H\},\quad\frac{dp_1}{dt}=\{p_1,H\} ,\\
   		\frac{dx_2}{dt}=\{x_2,H\},\quad\frac{dp_2}{dt}=\{p_2,H\} ,\\
   		\frac{dx_3}{dt}=\{x_3,H\},\quad\frac{dp_3}{dt}=\{p_3,H\} .
    \end{cases}
\end{equation}
$$
即
$$
\begin{equation}
    \begin{cases}
   		\frac{dx_1}{dt}=\frac{p_1}{m_1},\quad\frac{dp_1}{dt}=-\frac{V_0}{r_0}(e^{(x_1-x_2)/r_0}-e^{(x_3-x_1)/r_0}) ,\\
   		\frac{dx_2}{dt}=\frac{p_2}{m_2},\quad\frac{dp_2}{dt}=-\frac{V_0}{r_0}(e^{(x_2-x_3)/r_0}-e^{(x_1-x_2)/r_0}) ,\\
   		\frac{dx_3}{dt}=\frac{p_3}{m_3},\quad\frac{dp_3}{dt}=-\frac{V_0}{r_0}(e^{(x_3-x_1)/r_0}-e^{(x_2-x_3)/r_0}) .
    \end{cases}
\end{equation}
$$


## 8.2

证明：

$$\begin{aligned}
&\{f_{1},f_{2}\}=-\{f_{2},f_{1}\} , \\
&\begin{aligned}\{af_1+bf_2,f_3\}=a\{f_1,f_3\}+b\{f_2,f_3\} ,\end{aligned} \\
&\begin{aligned}\{f_1\cdot f_2,f_3\}=\{f_1,f_3\}f_2+f_1\{f_2,f_3\} ,\end{aligned} \\
&\begin{aligned}\{f_1,\{f_2,f_3\}\}+\{f_2,\{f_3,f_1\}\}+\{f_3,\{f_1,f_2\}\}=0 .\end{aligned}
\end{aligned}$$



**(1)**

$\{f_{1},f_{2}\}=\frac{\partial f_1}{\partial q}\frac{\partial f_2}{\partial p}-\frac{\partial f_1}{\partial p}\frac{\partial f_2}{\partial q}=-(\frac{\partial f_1}{\partial p}\frac{\partial f_2}{\partial q}-\frac{\partial f_1}{\partial q}\frac{\partial f_2}{\partial p})=-\{f_{2},f_{1}\}$

**(2)**

$\{af_1+bf_2,f_3\}=\frac{\partial (af_1+bf_2)}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial (af_1+bf_2)}{\partial p}\frac{\partial f_3}{\partial q} \\ =a\frac{\partial f_1}{\partial q}\frac{\partial f_3}{\partial p}+b\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-(a\frac{\partial f_1}{\partial p}\frac{\partial f_3}{\partial q}+b\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q}) \\=a(\frac{\partial f_1}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_1}{\partial p}\frac{\partial f_3}{\partial q})+b(\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q}) \\=a\{f_1,f_3\}+b\{f_2,f_3\}$

**(3)**

$\{f_1\cdot f_2,f_3\}=\frac{\partial (f_1\cdot f_2)}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial (f_1\cdot f_2)}{\partial p}\frac{\partial f_3}{\partial q} \\= f_2\frac{\partial f_1}{\partial q}\frac{\partial f_3}{\partial p}+f_1\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-(f_2\frac{\partial f_1}{\partial p}\frac{\partial f_3}{\partial q}+f_1\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q}) \\= f_2(\frac{\partial f_1}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_1}{\partial p}\frac{\partial f_3}{\partial q})+f_1(\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q}) \\= \{f_1,f_3\}f_2+f_1\{f_2,f_3\}$

**(4)**
$$
\{f_1,\{f_2,f_3\}\}+\{f_2,\{f_3,f_1\}\}+\{f_3,\{f_1,f_2\}\}=\sum_{cyc} \{f_1,\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q}\} \\=\sum_{cyc} \frac{\partial f_1}{\partial q}\frac{\partial (\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q})}{\partial p}-\frac{\partial f_1}{\partial p}\frac{\partial (\frac{\partial f_2}{\partial q}\frac{\partial f_3}{\partial p}-\frac{\partial f_2}{\partial p}\frac{\partial f_3}{\partial q})}{\partial q} \\= 0
$$


## 8.5

**(1)**
$$
\frac{dq}{dt}=\frac{\partial q}{\partial q}\frac{\partial H}{\partial p}-\frac{\partial q}{\partial p}\frac{\partial H}{\partial q}=\frac{\partial H}{\partial p}=E_2\sin p \\
\frac{dp}{dt}=\frac{\partial p}{\partial q}\frac{\partial H}{\partial p}-\frac{\partial p}{\partial p}\frac{\partial H}{\partial q}=-\frac{\partial H}{\partial q}=-E_1\sin q \\
$$
**(2)**
$$
\frac{d^2q}{dt^2}=\frac{d^2p}{dt^2}=0
$$
得
$$
(q,p)=(n\pi,m\pi) \quad(n,m \in \mathbb{Z})
$$

$$
\begin{equation}
	\begin{cases}
		能量极大值: n=2k_1+1,m=2k_2+1 \\
		能量极小值: n=2k_1,m=2k_2\\
		鞍点:(n=2k_1,b=2k_2+1) 或(n=2k_1+1,m=2k_2)
	\end{cases}
	(k_1,k_2 \in \mathbb{Z})
\end{equation}
$$



**(3)**

<img src="D:\homework\力学\第九次8.5.png" alt="第九次8.5" style="zoom:67%;" />

## 8.6

$$
H=\frac{p_1^2}{2m_1}+\frac{p_2^2}{2m_2}
$$

两对共轭变量：$(x_1,p_1),(x_2,p_2)$
$$
\frac{dx_i}{dt}=\frac{\partial H}{\partial p_i}=\frac{p_i}{m_i} \\
\frac{dp_i}{dt}=-\frac{\partial H}{\partial x_i}=0 \\
$$
故：
$$
\begin{equation}
	\begin{cases}
		p_1(t)=p_1(0), \\
		p_2(t)=p_2(0), \\
		x_1(t)=x_1(0)+\frac{p_1(0)}{m_1}t, \\
		x_2(t)=x_2(0)+\frac{p_2(0)}{m_2}t.
	\end{cases}
\end{equation}
$$
守恒量:

​	(1)$H$

​	(2)$p_1$

​	(3)$p_2$