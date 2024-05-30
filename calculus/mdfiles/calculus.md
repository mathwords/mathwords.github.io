[< Home](/index.html)



### Calculus Theorems



1. **Extreme Value Theorem** (**EVT**)
   Let $f$ be a continuous function over a closed interval $[a,b].$ Then there exists a point in the interval where $f$ has a maximum, and there exists a point in the interval where $f$​ has a minimum. 

   *Proof:* 
   Real numbers. $\varepsilon$-$\delta.$​ 

   

2. **Intermediate Value Theorem** (**IVT**)
   Let $f$ be a continuous function on the interval $[a,b].$ Let $\alpha = f(a)$ and $\beta = f(b).$ Let $\gamma$ be a number between $\alpha$ and $\beta.$  Then $\exists c \in [a,b]$ such that $f(c) = \gamma.$

   *Proof:* 
   Real numbers. $\varepsilon$-$\delta.$

   

3. **Fermat's Theorem**
   Let $f$ be a function which is defined and differentiable in the open interval $(a,b).$ Let $c$ be a number in the interval at which the function has a local maximum or a local minimum. Then $f'(c) = 0.$ 

   *Proof:* 
   From definition of local extremum and definition of derivative.

   

4. **Rolle's Theorem** (**RMVT**)
   If a function $f : [a, b] → \mathbb{R}$ is continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$ and $f (a) = f (b),$ then there exists a point $c \in (a, b)$ such that $f'(c) = 0.$

   *Proof:* 
   From definition of derivative, EVT and Fermat's Theorem.

   

5. **Lagrange's Mean Value Theorem** (**LMVT**)
   If a function $f : [a, b] → \mathbb{R}$ is continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$ and $f (a) = f (b),$ then there exists a point $c \in (a, b)$ such that: 
   $$
   f'(c) = \frac{f(b) - f(a)}{b-a}.
   $$
   *Proof:* 
   From RMVT.

   

6. **Cauchy's (Generalised) Mean Value Theorem** (**CMVT**)
   If functions $f, g : [a, b] → \mathbb{R}$ are continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$ and $f (a) = f (b),$ then there exists a point $c \in (a, b)$ such that: 
   $$
   f'(c)(g(b) - g(a)) = g'(c)(f(b) - f(a)).
   $$
   *Proof:* 
   From RMVT.



**Note:** All three mean value theorems are equivalent. That is, RMVT $\Leftrightarrow$ LMVT $\Leftrightarrow$ CMVT.



7. **Corollary to LMVT** (Criteria for function to be **constant**)
   Let a function $f$ be a function continuous on the closed interval $[a, b].$ Then,
   $f$ is constant on $[a,b$] $\iff$ $\forall x \in [a,b], f'(x) = 0.$

   *Proof:* 
   $(\Rightarrow)$ follows directly from the definition of the derivative, and indeed is used in the proof of RMVT.
   $(\Leftarrow)$ is a corollary of LMVT.

   

8. **Corollary to LMVT** (Criteria for function to be **monotonic**)

   * If the derivative of a function is nonnegative (resp. positive) at every point of an open interval, then the function is increasing (resp. strictly increasing) on that interval.
   * If the derivative of a function is nonpositive (resp. negative) at every point of an open interval, then the function is decreasing (resp. strictly decreasing) on that interval.

   *Proof:* 
   Corollary of LMVT.



---

#### Notes

* From AE-Analysis

  > The following theorem, which shows that there is only one order complete extension field of $\mathbb{Q}$​, is the most fundamental result of analysis and the starting point for all research into the ‘limiting processes’ which are at the center of all analytic investigation.
  >
  > **Theorem** There is, up to isomorphism, a unique order complete extension field $\mathbb{R}$ of $\mathbb{Q}$​. This extension is called the field of real numbers.
  
* From SL-AFCIC

  > The point of the mean value theorem is not so much to find explicitly a value $c$ such that $f'(c) = \frac{f(b) - f(a)}{b-a},$ as to use it for theoretical considerations. 



[< Home](/index.html)