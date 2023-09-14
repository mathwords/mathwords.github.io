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

**b)**    Construct $h$ as follows. $\forall y \in f(X),$ define $h:Y \to X$ by the mapping $y \mapsto x,$ such that $f(x) =y.$ Since $f$ is injective, this is a valid mapping (ie: $\forall y \in f(X) \ \exists!x$ such that $y \mapsto x$). And $\forall y \in Y\setminus f(X),$ define $h:Y \to X$ by the mapping $y \mapsto x_1,$ where $x_1$ is any element of $X.$ We now have $h$ such that $h \circ f (x) = h(f(x)) = h(y) = x.$ Hence, $h\circ f = \mathrm{id}_X.$

  




[< Home](/index.html)

