# Fouier Trans & Laplace Trans

## &emsp;傅里叶变换和拉普拉斯变换在信号处理和机器学习等方面有着极其重要的作用

## Chap1 傅里叶级数

&emsp;&ensp;法国数学家傅里叶猜想道:"任何一个周期函数都可以表示为一系列三角函数的和"根据这个猜想,反推出了傅里叶级数, 用数学形式可以表示为:        
<font size = 5><center>$f(t) = A_{0}+ A_{n}{\textstyle \sum_{0}^{∞}}sin(nw_{0}+\varphi )$</center></font>

## 1.1推导

$Sin (n\omega_{0}+\varphi) = Ansin(\varphi)cos(n\omega _{0}t)+Ancos(\varphi)sin(n\omega_{0}t)$  
由MacLaurin展开可知: $A_{0}$ = f(0) , $f(x) =  {\textstyle \sum_{1}^{∞}}f^{n}(x)/n!$    
<font size = 4>$\int_{-T/2}^{T/2}f(t)  = \int_{-T/2}^{T/2}A_{0}+\int_{-T/2}^{T/2}(...)$</font>    
由三角函数的正交性:      
$\int_{-\pi}^{\pi}sin(kx)cos(nx) = 0$   
$\int_{-\pi}^{\pi}sin(kx)six(nx) = 0 (k ≠ n)$   
$\int_{-\pi}^{\pi}sin(kx)cos(nx) = 0 (k ≠ n)$   
所以<font size = 5><center>$f(...)$ = 0</center></font>这样就得到了$A_{0}$     
&emsp;记:$Ansin(\varphi) = a_{n}$       
&emsp;&emsp;$Ancos(\varphi)= b{n}$      
现在求$a_{n},b_{n}$
在两边乘上$cos(tk\omega)$, 变为     
<font size = 4>$\int_{-T/2}^{T/2}f(t)cos(k\omega t) = {\textstyle\sum_{1}^{∞}}[\int_{-T/2}^{T/2}cos(nt\omega)cos(kt\omega)+\int_{-T/2}^{T/2}sin(nt\omega)cos(kn\omega)]+\int_{-T/2}^{T/2}cos(kt\omega)A_{0}$</font>       
由三角函数的正交性
可以得到:   
右边 = <font size  = 4>$\int_{-T/2}^{T/2}cos(n\omega t)^{2}+\int_{-T/2}^{T/2}sin(nt\omega)^{2} = TA_{n}/2$</font>  
$b_{n}$也可以得到:  
由此可以得到最终结论:       

<font size = 5><center>$f(t)=a_{0}/2+{\textstyle\sum_{0}^{∞}}[a_{n}cos(n\omega t)+b_{n}sin(n\omega t)]$     

$a_{n} = 2/T\int_{t_{0}-T/2}^{t_{0}+T/2}cos(n\omega t)dt $      

$b_{n} = 2/T\int_{t_{0}-T/2}^{t_{0}+T/2}sin(n\omega t)dt $


