[< Home](/index.html)



### Calculus Theorems



1. **Archimedean Property of Reals** (**APR**)
   If $x,y \in \mathbb{R}$ and $x>0,$ then $\exists n\in \mathbb{N}$ such that $y < nx.$​

   *Proof:*
   Real numbers.

   

2. **Corollary to APR** 
   For any positive number $\varepsilon$ there exists a natural number $n$ such that $0 < \frac{1}{n} < \varepsilon.$​

   *Proof:*
   Set $y = 1,$ and $x = \varepsilon$​ in APR.

   

3. **Proposition**

   1. $\forall b \in \mathbb{R},$ $\exists n \in \mathbb{Z}^+, n > b.$
   2. If $\forall n \in \mathbb{Z}^+, 0 \le a < \frac{1}{n},$ then $a = 0.$​

   *Proof:*
   Proof of 3.1 follows from Real numbers (especially completeness / APR). Then 3.2 follows from 3.1.

   

4. **Proposition** (Limit of a function is unique)
   Let $S$ be a set of numbers arbitrarily close to $x_0$ and let $S'$ be a subset of $S$, also arbitrary close to $x_0.$ Let $f$ be a function defined on $S.$ If
   $$
   \begin{align*}
   \lim_{x \to x_0} f(x) &= L, \ \text{with respect to } S \\
   \lim_{x \to x_0} f(x) &= M, \ \text{with respect to } S'
   \end{align*}
   $$
   Then $L = M.$​ In particular, the limit is unique.

   *Proof:*
   Definition of limit and Proposition 3.2.

   

5. **Extreme Value Theorem** (**EVT**)
   Let $f$ be a continuous function over a closed interval $[a,b].$ Then there exists a point in the interval where $f$ has a maximum, and there exists a point in the interval where $f$​​ has a minimum. 

   *Proof:* 
   Real numbers. $\varepsilon$-$\delta.$​ 

   

6. **Intermediate Value Theorem** (**IVT**)
   Let $f$ be a continuous function on the interval $[a,b].$ Let $\alpha = f(a)$ and $\beta = f(b).$ Let $\gamma$ be a number between $\alpha$ and $\beta.$  Then $\exists c \in [a,b]$ such that $f(c) = \gamma.$

   *Proof:* 
   Real numbers. $\varepsilon$-$\delta.$

   

7. **Fermat's Theorem**
   Let $f$ be a function which is defined and differentiable in the open interval $(a,b).$ Let $c$ be a number in the interval at which the function has a local maximum or a local minimum. Then $f'(c) = 0.$ 

   *Proof:* 
   From definition of local extremum and definition of derivative.

   

8. **Rolle's Theorem** (**RMVT**)
   If a function $f : [a, b] → \mathbb{R}$ is continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$ and $f (a) = f (b),$ then there exists a point $c \in (a, b)$ such that $f'(c) = 0.$

   *Proof:* 
   From definition of derivative, EVT and Fermat's Theorem.

   

9. **Lagrange's Mean Value Theorem** (**LMVT**)
   If a function $f : [a, b] → \mathbb{R}$ is continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$ and $f (a) = f (b),$ then there exists a point $c \in (a, b)$ such that: 
   $$
   f'(c) = \frac{f(b) - f(a)}{b-a}.
   $$
   *Proof:* 
   From RMVT.

   

10. **Cauchy's (Generalised) Mean Value Theorem** (**CMVT**)

    If functions $f, g : [a, b] → \mathbb{R}$ are continuous on a closed interval $[a, b]$ and differentiable on the open interval $(a, b)$ and $f (a) = f (b),$ then there exists a point $c \in (a, b)$ such that: $f'(c)(g(b) - g(a))$ $=$ $g'(c)(f(b) - f(a)).$​

    *Proof:* 
    From RMVT.

    

11. **Proposition** (**Equivalence of MVTs**)
    RMVT $\Leftrightarrow$ LMVT $\Leftrightarrow$​​​ CMVT.

    *Proof:* The standard proofs of LMVT and CMVT provide

    * RMVT $\Rightarrow$ LMVT, and
    * RMVT $\Rightarrow$ CMVT.

    On the other hand, LMVT is a special case of CMVT, whereas RMVT is a special case of LMVT. This gives us:

    * CMVT $\Rightarrow$ LMVT, and
    * LMVT $\Rightarrow$ RMVT.

    The four conditions stated above complete the proof.

    

12. **Corollary to LMVT** (Criteria for function to be **constant**)
    Let a function $f$ be a function continuous on the closed interval $[a, b].$ Then,
    $f$ is constant on $[a,b$] $\iff$ $\forall x \in [a,b], f'(x) = 0.$

    *Proof:* 
    $(\Rightarrow)$ follows directly from the definition of the derivative, and indeed is used in the proof of RMVT.
    $(\Leftarrow)$​​ is a corollary of LMVT.

    

13. **Corollary to LMVT** (Criteria for function to be **monotonic**)

    * If the derivative of a function is nonnegative (resp. positive) at every point of an open interval, then the function is increasing (resp. strictly increasing) on that interval.

    * If the derivative of a function is nonpositive (resp. negative) at every point of an open interval, then the function is decreasing (resp. strictly decreasing) on that interval.

      

14. 



---

#### Notes

* From AE-Analysis

  > The following theorem, which shows that there is only one order complete extension field of $\mathbb{Q}$​, is the most fundamental result of analysis and the starting point for all research into the ‘limiting processes’ which are at the center of all analytic investigation.
  >
  > **Theorem** There is, up to isomorphism, a unique order complete extension field $\mathbb{R}$ of $\mathbb{Q}$​. This extension is called the field of real numbers.
  
* From SL-AFCIC

  > The point of the mean value theorem is not so much to find explicitly a value $c$ such that $f'(c) = \frac{f(b) - f(a)}{b-a},$ as to use it for theoretical considerations. 



[< Home](/index.html)