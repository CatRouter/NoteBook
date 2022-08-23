# Signal & System

## Chap 0

<font size = 4> Courseware : [SIGNAL AND SYSTEM Alan V. Oppenheim , MIT OCW](https://ocw.mit.edu/courses/res-6-007-signals-and-systems-spring-2011/resources/lecture-1-introduction/)     
Textbook : [Signal and System by Alan V. Oppenheim](../TextBooks/%E4%BF%A1%E5%8F%B7%E4%B8%8E%E7%B3%BB%E7%BB%9F%20%20%20%E7%AC%AC%E4%BA%8C%E7%89%88%20(%E8%89%BE%E4%BC%A6V.%E5%A5%A5%E6%9C%AC%E6%B5%B7%E5%A7%86)%20.pdf)</font>  

![avatar](./images/J.B.Fouier.jpg)  
J.B Fourier

## Chap 1 : INTRODUCTION

### 1.1 What's signal? 

&emsp;&emsp;&emsp;Signal's unformal definition(or mathematically):     
<b><font size = 3><center> Functions of one or more independent variables that typically carry some information</center></font></b>
Like voice and image , can be regarded as signal.
![avtar](./images/Dow%20Jones.png)

### 1.2 What's system?
<b><font size = 3><center> System typcally used to process signals</center></font></b>

![avtar](./images/system.png) 

A system may  a continous system or a discrete time system ( $x(t)$ or $x[n]$ )     
system can be basically devided into linear and non-linear or time-invariant and time-varying.  
In this course we focus on LTI(lin.. Time.. in..) and Time & Frequnency domain

### 1.3 Interconnections of system:

<font size = 4 >Series  
Parallel    
Feedback  (Important in control)
</font>  

## Chap 2 Signals 

### Chap 2.1 sinusoidal signal
<font size = 3><center>CONTINOUS-TIME SINUSOIDAL SIGNAL    
$x(t) = A cos(\omega_{0} t + \phi)$</center></font>     

<font size = 3><center> DISCRETE SINUSOIDAL SIGNAL
![avatar](./images/discrte.png)    
 </center></font>

Remeber :
<font size = 4><center>Time shift = Phase change</center></font>   

And someting you should pay attention to : The period of discrete signal    
EG:

<font size = 3><center>$f[n] = sin(4n\pi/31)$</center></font>The period isn't be <font size = 4>$\frac{31\pi}{4}$</font> cause $n$ must be an integer. so the period is 31    
Another case is that the  $\frac{2\pi}{\omega_{0}}*n$ can't be a integer. The sigal is inperiodic 


### Chap 2.2 expontial signal

<center> REAL EXPOTENTIAL CONTINOUS-TIME SIGNAL</center>

<font size = 4><center>$x(t) = Ce^{at}$</center></font>
<center> REAL  EXPOTENTIAL DIACRETE-TIME SIGNAL</center>

<font size = 4><center>$x(n) = C\alpha^{n} = Ce^{\beta n}$</center></font>

Remeber :
<font size = 4><center>Time shift = Scale change</center></font> 

<center> CONTINOUS TIME COMPLEX EXPOTENTIAL</center>

<font size = 4><center>$x(t) = Ce^{at}$</center></font>

but parameter $C$ and $a$ is complex number     
C = $|C|e^{j\theta}$    (Polar form)    
a = $r + j\omega_{0}$   (Rectancular form)  
$x(t) = $

