# Bezier-curves 贝塞尔曲线
This article mainly explains the derivation process of Bessel curves

### Introduction 
[A Bézier curve (pronounced [bezje] in French) is a parametric curve used in computer graphics and related fields.](https://en.wikipedia.org/wiki/B%C3%A9zier_curve)

### Example 以二阶贝塞尔曲线为例来引入推导过程
Bézier curves are widely used in computer graphics to model smooth curves. As the curve is completely contained in the convex hull of its control points, the points can be graphically displayed and used to manipulate the curve intuitively.

![image](https://github.com/HisenLee/Bezier-curves/blob/master/aaa.png)

如图从线段AB和线段BC分别任意取点D和点E，使得AD/AB = BE/BC = t (t可以理解为变化过程中的恒定值)，连接D和E，并取点F，使得DF/DE 也等于t ， 
即AD/AB = BE/BC =  DF/DE = t， 那么点F就为最终曲线上的一个点。将上述过程中极限化，即点D为A到B过程中的任意点的集合，
点E为B到C过程中任意点的集合，生成点F的集合就会构成最终的曲线路径，如动态图所示。

![image](https://github.com/HisenLee/Bezier-curves/blob/master/2.gif)

### Linear Bezier curves 一阶贝塞尔曲线公式的推导
  * Formula

    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/1.png)
  * Detail Derivation Process
    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/11.png)
    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/111.png)
    
  * Dynamic display    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/1.gif)
  
    
### Quadratic Bezier curves 二阶贝塞尔曲线公式的推导
  * Formula

    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/2.png)
  * Detail Derivation Process
    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/22.png)
    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/222.png)
    
  * Dynamic display    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/2.gif)
    
    
 ### Cubic Bezier curves 三阶贝塞尔曲线公式的推导
  * Formula

    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/3.png)
  * Detail Derivation Process
    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/33.png)
    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/333.png)
    
  * Dynamic display    
    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/3.gif)
    
  
  ### Verify Higher-order curves 验证高阶贝塞尔曲线公式
  
   ![image](https://github.com/HisenLee/Bezier-curves/blob/master/n.png) 
   
   公式当中, ![image](https://github.com/HisenLee/Bezier-curves/blob/master/cv.png)
   
   用通项公式来验证n=3(i依次替换为0,1,2,3)的情况与之前推导的三阶公式是否一致，推导过程如下，得到的结果经过验证与之前结果一致。
   
   ![image](https://github.com/HisenLee/Bezier-curves/blob/master/nn.jpg)
   
   ### [Non-uniform rational basis spline (NURBS) 贝塞尔曲线扩展到三维的贝塞尔曲面](https://en.wikipedia.org/wiki/Non-uniform_rational_B-spline)
   
   ![image](https://github.com/HisenLee/Bezier-curves/blob/master/mian1.png)    ![image](https://github.com/HisenLee/Bezier-curves/blob/master/mian2.png)
  
   
  
    
