# cs21001-assignment-2--solving-recurrence-relations-solved
**TO GET THIS SOLUTION VISIT:** [CS21001 Assignment 2 -Solving Recurrence Relations Solved](https://www.ankitcodinghub.com/product/cs21001-assignment-2-solving-recurrence-relations-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;92840&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS21001 Assignment 2 -Solving Recurrence Relations Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Solving Recurrence Relations

In this assignment, you write a program to find the solution of recurrence relations of the form an =ran−1+san−2+t,

where r,s,t and the first two terms a0,a1 of the sequence are supplied by the user as integer constants. We assume that s ̸= 0. The characteristic equation of this recurrence is x2 − rx − s = 0. You need to compute the roots of this equation, and handle all the cases like integer roots with possible repetitions, and non- integer (real or complex) roots occurring in conjugate pairs. Moreover, for the non-homogeneous part, you should consider all the possibilities of 1 being a root of the characteristic equation with multiplicity 0, 1, or 2. Since the theory of recurrence relations is covered in detail in the lectures, we concentrate only on the programming part and the input/output specifications of your program.

Part 1: Dealing with rationals and quadratic irrationals

1 􏰌􏰊1+√5􏰋n 􏰊1−√5􏰋n􏰍

</div>
</div>
<div class="layoutArea">
<div class="column">
We have solved the recurrence for Fibonacci numbers as Fn = √5 2

a floating-point approximation for √5. In this assignment, we will follow the same idea, and never go for floating-point approximations of rational or irrational numbers. Since we start with the roots of quadratic equations, we need to exactly represent real/complex numbers of the form

a+b√d c

Here, c is a positive integer, whereas a, b, d are arbitrary integers. We enforce gcd(a, b, c) = 1. Let us call these special numbers. Depending upon the value of d, there are different types of special numbers.

</div>
</div>
<div class="layoutArea">
<div class="column">
− 2 . We did not go for

</div>
</div>
<div class="layoutArea">
<div class="column">
If d &gt; 0 is not a perfect square, our special number is a quadratic irrational. The two roots of the characteristic equation are r±√r2+4s. If r is even and r2 +4s is a multiple of 4 but not a perfect square,

</div>
</div>
<div class="layoutArea">
<div class="column">
2

we cancel one factor of 2 from the numerator and the denominator. We fix the value of d to r2 + 4s or

</div>
</div>
<div class="layoutArea">
<div class="column">
(r2 + 4s)/4 in all future computations. Do not attempt to process square factors further in it. For example, keep √45 as such, do not try to simplify it as 3√5.

If d 􏰅 0 is a perfect√square, then the two roots of the characteristic equation are actually integers. We absorb the contribution of d in a, and take d = 0. In this case, we deal with rational numbers of the form ac .

</div>
</div>
<div class="layoutArea">
<div class="column">
Finally, if d &lt; 0, we are dealing with complex numbers. We will keep the negative sign of d inside the radical as in 1+√−3 .

</div>
</div>
<div class="layoutArea">
<div class="column">
2

Define a data type splnum to store the four components a, b, c, d (all are integers) of special numbers. If you

use C, you need to define a structure. If you use C++, you may use a structure or define a class. (2)

</div>
</div>
<div class="layoutArea">
<div class="column">
Write the following functions to implement the arithmetic of special numbers. If you use a C++ class for splnum, you may overload the standard arithmetic operators. You may add other functions (like negation, check for zero) if you find those convenient. (6)

<pre>  splnum addspl ( splnum u, splnum v );  /* Returns u+v */
  splnum subspl ( splnum u, splnum v );  /* Returns u-v */
  splnum mulspl ( splnum u, splnum v );  /* Returns uv */
  splnum invspl ( splnum u );            /* Returns 1/u provided that u is not zero */
  splnum divspl ( splnum u, splnum v );  /* Returns u/v provided that v is not zero */
  void prnspl ( splnum u );              /* Print u as in the sample outputs */
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
— Page1of4 —

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Write a function

</div>
</div>
<div class="layoutArea">
<div class="column">
void findroots ( int r, int s, splnum roots[2] );

to compute the two roots of the characteristic equation and store them in the array roots. (4)

Part 2: Solving the homogeneous recurrence (8)

Write a function

<pre>  void solvehomogeneous ( int r, int s, int a0, int a1 );
</pre>
to print the closed-form solution of the homogeneous recurrence an = ran−1 + san−2 with the two initial termsa0,a1 asspecifiedinthecall.Thisfunctionshouldcallfindrootstocomputethetworootsρ1,ρ2 of thecharacteristicequation. Ifρ1 ̸=ρ2,thenthesolutionisan =Uρ1n+Vρ2n. Ifρ1 =ρ2 =ρ,thenthesolution is an = (U n + V )ρ n . The constants U , V are to be determined as splnum’s from the initial conditions.

Part 3: Solving the non-homogeneous recurrence (12)

Write a function

<pre>  void solvenonhomogeneous ( int r, int s, int t, int a0, int a1 );
</pre>
to print the closed-form solution of the homogeneous recurrence an = ran−1 + san−2 + t with the two initial terms a0,a1 as specified in the call. Compute and print the particular solution first. Then compute the homogeneous solution, and print it. Since t = t × 1n, you need to check whether 1 is a root of the characteristic equation, and if so, what its multiplicity is. The particular solution depends on that.

The main function

• Read r,s,t,a0,a1 from the user.

• Call solvehomogeneous() to print the solution of the homogeneous equation.

• Call solvenonhomogeneous() to print the solution of the nonhomogeneous equation.

Output (8)

Your code will be tested on several inputs. Some test cases are supplied below, Do not use global/static variables. Submit a single C/C++ file. Do not use STL. Your code must compile without any extra flag (except -lm for C programs).

**************** TEST CASE 1 (Fibonacci-type recurrence) **************** r=1

s=1

t=2

a0 = 0 a1 = 1

+++ Solving the homogeneous recurrence

Characteristic equation: x^2 + (-1)x + (-1) = 0

Root 1 = (1 + sqrt(5)) / 2

Root 2 = (1 – sqrt(5)) / 2

Homogeneous solution :

[(sqrt(5)) / 5] [(1 + sqrt(5)) / 2]^n + [(-sqrt(5)) / 5] [(1 – sqrt(5)) / 2]^n

+++ Solving the nonhomogeneous recurrence

Characteristic equation: x^2 + (-1)x + (-1) = 0

Root 1 = (1 + sqrt(5)) / 2

Root 2 = (1 – sqrt(5)) / 2

Particular solution : -2

Homogeneous solution :

[(5 + 2 sqrt(5)) / 5] [(1 + sqrt(5)) / 2]^n + [(5 – 2 sqrt(5)) / 5] [(1 – sqrt(5)) / 2]^n

</div>
</div>
<div class="layoutArea">
<div class="column">
— Page2of4 —

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
**************** TEST CASE 2 (Complex roots) **************** r=1

s = -7

t = -1

a0 = 1 a1 = 3

+++ Solving the homogeneous recurrence

Characteristic equation: x^2 + (-1)x + (7) = 0

Root 1 = (1 + sqrt(-27)) / 2

Root 2 = (1 – sqrt(-27)) / 2

Homogeneous solution :

[(27 – 5 sqrt(-27)) / 54] [(1 + sqrt(-27)) / 2]^n + [(27 + 5 sqrt(-27)) / 54] [(1 – sqrt(-27)) / 2]^n

+++ Solving the nonhomogeneous recurrence

Characteristic equation: x^2 + (-1)x + (7) = 0

Root 1 = (1 + sqrt(-27)) / 2

Root 2 = (1 – sqrt(-27)) / 2

Particular solution : (-1) / 7

Homogeneous solution :

[(12 – 2 sqrt(-27)) / 21] [(1 + sqrt(-27)) / 2]^n + [(12 + 2 sqrt(-27)) / 21] [(1 – sqrt(-27)) / 2]^n

**************** TEST CASE 3 (Distinct integer roots) **************** r=2

s=3

t=3

a0 = 1 a1 = 2

<pre>+++ Solving the homogeneous recurrence
    Characteristic equation: x^2 + (-2)x + (-3) = 0
    Root 1 = 3
    Root 2 = -1
    Homogeneous solution :
    [3 / 4] [3]^n + [1 / 4] [-1]^n
</pre>
<pre>+++ Solving the nonhomogeneous recurrence
    Characteristic equation: x^2 + (-2)x + (-3) = 0
    Root 1 = 3
    Root 2 = -1
    Particular solution : -3 / 4
    Homogeneous solution :
    [9 / 8] [3]^n + [5 / 8] [-1]^n
</pre>
**************** TEST CASE 4 (Repeated roots) **************** r=4

s = -4

t=3

a0 = 1 a1 = 1

<pre>+++ Solving the homogeneous recurrence
    Characteristic equation: x^2 + (-4)x + (4) = 0
    Root 1 = 2
    Root 2 = 2
    Homogeneous solution :
    [(-1 / 2)n + (1)] 2^n
</pre>
<pre>+++ Solving the nonhomogeneous recurrence
    Characteristic equation: x^2 + (-4)x + (4) = 0
    Root 1 = 2
    Root 2 = 2
    Particular solution : 3
    Homogeneous solution :
    [(1)n + (-2)] [2]^n
</pre>
**************** TEST CASE 5 (1 is a root of multiplicity 1) **************** r=4

s = -3

t=1

a0 = 2 a1 = 7

<pre>+++ Solving the homogeneous recurrence
    Characteristic equation: x^2 + (-4)x + (3) = 0
    Root 1 = 3
    Root 2 = 1
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
— Page3of4 —

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
<pre>Homogeneous solution :
    [5 / 2] [3]^n + [-1 / 2] [1]^n
</pre>
<pre>+++ Solving the nonhomogeneous recurrence
    Characteristic equation: x^2 + (-4)x + (3) = 0
    Root 1 = 3
    Root 2 = 1
    Particular solution : [-1 / 2] n
    Homogeneous solution :
    [11 / 4] [3]^n + [-3 / 4] [1]^n
</pre>
**************** TEST CASE 6 (1 is a root of multiplicity 2) **************** r=2

s = -1

t=1

a0 = 4 a1 = 7

<pre>+++ Solving the homogeneous recurrence
    Characteristic equation: x^2 + (-2)x + (1) = 0
    Root 1 = 1
    Root 2 = 1
    Homogeneous solution :
    [(3)n + (4)] 1^n
</pre>
<pre>+++ Solving the nonhomogeneous recurrence
    Characteristic equation: x^2 + (-2)x + (1) = 0
    Root 1 = 1
    Root 2 = 1
    Particular solution : [1 / 2] n^2
    Homogeneous solution :
    [(5 / 2)n + (4)] 1^n
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
— Page4of4 —

</div>
</div>
</div>
