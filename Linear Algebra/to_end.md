<!--
 * @Author: your name
 * @Date: 2020-07-04 06:02:07
 * @LastEditTime: 2020-07-04 06:53:17
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
--> 
# 卷积
1.$(c*d)_k = \sum_{i+j=k} c_i d_j=\sum c_id_{k-i}$,其中$c=c_0+c_1x+...+c_nx^n,d=d_0+d_1x_...+d_nx^n$,而对于连续函数而言，有$f(x)*g(x)=(f*g)(tx)=\it f(t)g(x-t)dt$，当x为循环卷积阵时，【未看懂part】，但有循环卷积矩阵的特征矩阵为傅里叶矩阵。并且满足$F\left[\begin{matrix}
    c_0\\
    c_1\\
    \vdots\\
    c_n
\end{matrix}\right]=特征值$
2. 卷积法则
   1.  $F(c\bigotimes d)=(Fc)*(Fd)$，由于FFT（快速傅里叶变换）便捷，因此可用于解方程，见百度，属于数值计算内容
   2.  Cholesley分解，$X^TX=LDL^T,X=\sqrt{D}L^T$，已知$X^TX$如何求解X。
# 距离矩阵与位置矩阵
1. 有$||x_1-x_2||=1,||x_2-x_3||=1,||x_1-x_3||=6$,由三角不等式可知不成立，反映在距离矩阵D与位置矩阵G上即有满足三角不等式的D，必有G正定
2. 求解问题$XQ\approx Y$,也即$min_{Q^TQ=I}||YQ-X||^2_{F},则有若Y^TX=U\Sigma V^T,Q_{best}=UV^T$
3. $||A||^2_F=trace(A^TA)=\sigma_1^2+...+\sigma_r^2$,关于trace,有$trace(A^TB)=trace(B^TA)=trace(BA^T),在涉及trace时，考虑1.对角线元素，2.特征值$
# 拉普拉斯矩阵
1. 拉普拉斯矩阵L必有一特征值为0，此时特征向量为常数，即  $\lambda_1=0,x_1=\left[\begin{matrix}
    c\\
    c\\
    c\\
    \vdots
\end{matrix}\right]$,可由  
$L\left[\begin{matrix}
    1\\
    1\\
    1\\
    \vdots
\end{matrix}\right]=0\left[\begin{matrix}
    1\\
    1\\
    1\\
    \vdots
\end{matrix}\right]$得到.
2. $\lambda_n$与$\lambda_1$正交，必然有  
$\lambda_n=\left[\begin{matrix}
    a_1\\
    a_2\\
    a_3\\
    \dots
\end{matrix}\right],\lambda_n^T\lambda_1=0=a_1+a_2+...a_n$，固必然有正有负
# 完结撒花
线代是十分必要的科目，不仅是运算，也是认识世界的工具。