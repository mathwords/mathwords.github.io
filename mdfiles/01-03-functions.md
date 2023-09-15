[< Home](/index.html)



**I.3   Functions**



---

***Exercise 1***
(Proof of Proposition 3.6)

**Proposition 3.6**   Let $f : X \to Y$ and $g : Y \to V$ be bijective. Then $g \circ f : X \to V$ is bijective and 
$$
(g \circ f)^{-1} = f^{-1} \circ g^{-1}
$$
**Proof** 

* Suppose that $f$ and $g$ are both injective.
  $g(f(x_1)) = g(f(x_2))$ $\implies$ $f(x_1) = f(x_2)$ $\implies$ $x_1 = x_2.$ 
  First implication is true because $g$ is injective and the second implication is true because $f$ is injective.   Hence injectivity of $f$ and $g$ implies injectivity of $g \circ f.$
* Suppose that $f$ and $g$ are both surjective.
  Since $g$ is surjective: $\forall v \in V, \exists y \in Y,$ such that $g(y) = v.$ And, since $f$ is surjective: $\forall y \in Y, \exists x \in X,$ such that $f(x) = y.$ Consequently, $\forall v \in V, \exists x \in X,$ such that $g(f(x)) = v.$
  Hence surjectivity of $f$ and $g$ implies surjectivity of $g \circ f.$
* $(g \circ f) \circ (f^{-1} \circ g^{-1})$ $=$ $((g \circ f) \circ f^{-1}) \circ g^{-1}$ $=$ $(g \circ (f \circ f^{-1})) \circ g^{-1}$ $=$ $(g \circ \mathrm{id}_Y) \circ g^{-1}$ $=$ $g \circ g^{-1}$ $=$ $\mathrm{id}_V.$
  Also,
  $(f^{-1} \circ g^{-1}) \circ (g \circ f)$ $=$ $((f^{-1} \circ g^{-1}) \circ g) \circ f$ $=$ $(f^{-1} \circ (g^{-1} \circ g)) \circ f$ $=$ $(f^{-1} \circ \mathrm{id}_Y) \circ f$ $=$ $f^{-1} \circ f$ $=$ $\mathrm{id}_X.$ 
  It follows from the above results that $f^{-1} \circ g^{-1}$ is the inverse of $g \circ f$  (and by Proposition 3.5, the inverse is unique).



---

***Exercise 3***

**a)**    See Exercise 1.

**b)**    We need to prove both sides of the implication.

* $(\Rightarrow)$ Suppose that $f$ is injective. We construct $h : Y \to X$ as follows.

  * From the injectivity of $f$ it follows that $\forall y \in f(X),\ \exists! x\in X,$ such that $y = f(x).$ 
    We begin our construction of $h$ by first defining $h:f(X) \to X$ by the mapping $f(x) \mapsto x.$ 

  * Next, define $h:Y\setminus f(X) \to X$ by the mapping $y \mapsto x_1,$ where $x_1$ is any element of $X.$

  With these two steps, we have constructed $h: Y \to X$ such that $(h \circ f) (x) = h(f(x)) = x.$ Hence, $h\circ f = \mathrm{id}_X.$

* $(\Leftarrow)$ Suppose that $(h \circ f = \mathrm{id}_X)$ $\and$ $\neg (f \text{ is injective}).$ Then $\exists x_1, \exists x_2 \in X,$ such that $(x_1 \ne x_2) \and (f(x_1) = f(x_2)).$  But since $h$ is a function, we have: $f(x_1) = f(x_2) \Rightarrow h(f(x_1)) = h(f(x_2)).$ But given that $h \circ f = \mathrm{id}_X,$ we have $h(f(x_1)) = h(f(x_2)) \Rightarrow x_1 = x_2.$ This contradiction establishes that the original assumption is false. Therefore, $(h \circ f = \mathrm{id}_X)$ $\Rightarrow$ $(f \text{ is injective}).$

**c)**    Once again, we need to prove both sides of the implication.

* $(\Rightarrow)$ Suppose that $f$ is surjective. We construct $h : Y \to X$ as follows. From the surjectivity of $f$ it follows that $\forall y \in Y,\ \exists x\in X,$ such that $y = f(x).$ If for each $y,$ we select any one such $x,$ then every $y \in Y$ can be written in the form $f(x).$ Now, define $h:Y \to X$ by the mapping $f(x) \mapsto x.$ Based on this definition of $h,$ we now have: $h(y) = h(f(x)) = x.$ We can now evaluate $f \circ h$ as follows: $(f \circ h) (y)$ $= f(h(y))$ $=$ $f(x) = y.$ Therefore, $f\circ h = \mathrm{id}_Y.$

* $(\Leftarrow)$ Suppose that $(f \circ h = \mathrm{id}_Y)$ $\and$ $\neg (f \text{ is surjective}).$ Then $\exists y \in Y,\forall x \in X : (f(x) \ne y).$  But, given that $(f \circ h = \mathrm{id}_Y),$ we have $\forall y \in Y : f(h(y)) = y.$ But $h(y) \in X.$ So we now have $\forall y \in Y,\exists x \in X : (f(x) = y).$ This contradiction establishes that the original assumption is false. Therefore, $(f \circ h = \mathrm{id}_Y)$ $\Rightarrow$ $(f \text{ is surjective}).$




[< Home](/index.html)

