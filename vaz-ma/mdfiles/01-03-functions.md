[Home](/index.html)  >  [Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)


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
  First implication is true because $g$ is injective and the second implication is true because $f$ is injective.
  Hence injectivity of $f$ and $g$ implies injectivity of $g \circ f.$
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

  * First, define $h:Y\setminus f(X) \to X$ by the mapping $y \mapsto x_1,$ where $x_1$ is any element of $X.$
  * We will now define $h : f(X) \to X$ to complete the construction of $h : Y \to X.$ From the injectivity of $f$ it follows that $\forall y \in f(X),\ \exists! x\in X,$ such that $y = f(x).$ This permits us to define  $h:f(X) \to X$ by the mapping $f(x) \mapsto x.$

  With these two steps, we have constructed $h: Y \to X$ such that $(h \circ f) (x) = h(f(x)) = x.$ Hence, $\exists h,$ such that $h\circ f = \mathrm{id}_X.$

* $(\Leftarrow)$ Suppose that $(h \circ f = \mathrm{id}_X)$ $\and$ $\neg (f \text{ is injective}).$ Then $\exists x_1, \exists x_2 \in X,$ such that $(x_1 \ne x_2) \and (f(x_1) = f(x_2)).$  But since $h$ is a function, we have: $f(x_1) = f(x_2) \Rightarrow h(f(x_1)) = h(f(x_2)).$ But given that $h \circ f = \mathrm{id}_X,$ we have $h(f(x_1)) = h(f(x_2)) \Rightarrow x_1 = x_2.$ This contradiction establishes that the original assumption is false. Therefore, $(h \circ f = \mathrm{id}_X)$ $\Rightarrow$ $(f \text{ is injective}).$

**c)**    Once again, we need to prove both sides of the implication.

* $(\Rightarrow)$ Suppose that $f$ is surjective. We construct $h : Y \to X$ as follows. From the surjectivity of $f$ it follows that $\forall y \in Y,\ \exists x\in X,$ such that $y = f(x).$ If for each $y,$ we select any one such $x,$ then every $y \in Y$ can be written in the form $f(x).$ Now, define $h:Y \to X$ by the mapping $f(x) \mapsto x.$ Based on this definition of $h,$ we now have: $h(y) = h(f(x)) = x.$ We can now evaluate $f \circ h$ as follows: $(f \circ h) (y)$ $= f(h(y))$ $=$ $f(x) = y.$ Hence, $\exists h,$ such that $f\circ h = \mathrm{id}_Y.$

* $(\Leftarrow)$ Suppose that $(f \circ h = \mathrm{id}_Y)$ $\and$ $\neg (f \text{ is surjective}).$ The second condition tells us that $\exists y \in Y,\forall x \in X : (f(x) \ne y).$  The first condition tells us $\forall y \in Y : f(h(y)) = y.$ But $h(y) \in X.$ So we now have $\forall y \in Y,\exists x \in X : (f(x) = y).$ This contradiction establishes that the original assumption is false. Therefore, $(f \circ h = \mathrm{id}_Y)$ $\Rightarrow$ $(f \text{ is surjective}).$



---

***Exercise 4***

* Suppose that $\mathsf{a}$ is True. We will now examine $\mathsf{b}.$ 

  * We proceed as follows.  $x \in f^{-1}(f(A))$ $\Rightarrow$ $f(x) \in f(A)$ $\Rightarrow$ $\exists x' \in A : f(x') = f(x).$ But from the injectivity of $f$ we have $f(x') = f(x) \Rightarrow x' = x.$ It follows that $x \in A.$ Hence, $f^{-1}(f(A)) \subseteq A.$ 
  * On the other hand, $A \subseteq f^{-1}(f(A))$ is True irrespective of the injectivity of $f.$ Indeed, $x \in A$ $\Rightarrow$ $f(x) \in f(A)$ $\Rightarrow$ $x \in f^{-1}(f(A)).$ 

  Assuming the injectivity of $f,$ we have proved that $f^{-1}(f(A)) = A.$ We therefore have $\mathsf{a} \Rightarrow \mathsf{b}.$ 

* Suppose that $\mathsf{a}$ is False. Then $\exists x_1, \exists x_2 \in X,$ such that $(x_1 \ne x_2) \and (f(x_1) = f(x_2)).$ Now consider the set $\{x_1\} \subset X.$ We find that $(x_2 \notin \{x_1\}) \and (x_2 \in f^{-1}(f(\{x_1\}))).$ In other words, we have shown that $\exists A = \{x_1\} \subset X$ such that $f^{-1}(f(A)) \ne A.$ We therefore have, $\neg\mathsf{a} \Rightarrow \neg\mathsf{b},$ which is the same as $\mathsf{b} \Rightarrow \mathsf{a}.$ 

* Suppose that $\mathsf{a}$ is True. We will now examine $\mathsf{c}.$ We proceed as follows.

  * $f(x) \in f(A \cap B)$ $\Rightarrow$ $\exists x' \in A \cap B : f(x') = f(x).$ But from the injectivity of $f$ we have $f(x') = f(x) \Rightarrow x' = x.$ It follows that $x \in A \cap B$ which in turn implies that $(x \in A) \and (x \in B)$ $\Rightarrow$ $(f(x) \in f(A)) \and (f(x) \in f(B))$ $\Rightarrow$ $f(x) \in f(A) \cap f(B).$  Hence, $f(A \cap B) \subseteq f(A) \cap f(B).$ 
  * On the other hand, $f(x) \in f(A) \cap f(B)$ $\Rightarrow$ $\exists x_1 \in A : f(x_1) = f(x),$ and $\exists x_2 \in B : f(x_2) = f(x).$ But from the injectivity of $f$ we have $f(x_1) = f(x) \Rightarrow x_1 = x,$ and likewise $f(x_2) = f(x) \Rightarrow x_2 = x.$ We therefore have $(x \in A) \and (x \in B).$ It follows that $x \in A \cap B,$ and consequently $f(x) \in f(A \cap B).$ Hence, $f(A) \cap f(B) \subseteq f(A \cap B).$

  Assuming the injectivity of $f,$ we have proved that $f(A \cap B) = f(A) \cap f(B).$ We therefore have $\mathsf{a} \Rightarrow \mathsf{c}.$  

* Suppose that $\mathsf{a}$ is False. Then $\exists x_1, \exists x_2 \in X,$ such that $(x_1 \ne x_2) \and (f(x_1) = f(x_2)).$ We now find that $f(\{x_1\} \cap \{x_1\})$ $=$ $f(\empty) = \empty.$ However, $f(\{x_1\}) \cap f(\{x_1\}) \ne \empty.$ In other words, we have shown that $\exists A, B \subset X$ such that $f(A \cap B) \ne f(A) \cap f(B).$ We therefore have, $\neg\mathsf{a} \Rightarrow \neg\mathsf{c},$ which is the same as $\mathsf{c} \Rightarrow \mathsf{a}.$ 

From $(\mathsf{a} \Rightarrow \mathsf{b}) \and (\mathsf{b} \Rightarrow \mathsf{a})$ it follows that $\mathsf{a} \Leftrightarrow \mathsf{b}.$ And from $(\mathsf{a} \Rightarrow \mathsf{c}) \and (\mathsf{c} \Rightarrow \mathsf{a})$ it follows that $\mathsf{a} \Leftrightarrow \mathsf{c}.$ We have thus proved that $\mathsf{a} \Leftrightarrow \mathsf{b} \Leftrightarrow \mathsf{c}.$ 



---

***Exercise 6***

* Proof that the given function is <u>injective</u>:
  Suppose that $A$ and $B$ are subsets of $X,$ such that $A \ne B.$ With no loss of generality we can then assume that $A \not\subseteq B.$ Then $\exists a \in A : a \notin B.$ It follows that $(a,1) \in \chi_A,$ but $(a,1) \notin \chi_B.$ We have  shown that $A \ne B \Rightarrow \chi_A \ne \chi_B.$ Therefore the given function is injective.
* Proof that the given function is <u>surjective</u>:
  $\forall \, \chi_K \in \{0,1\}^X,$ we have $K \subseteq X.$ Hence, $K \in \mathcal{P}(X).$ Every $\chi_K \in \{0,1\}^X$ therefore has a preimage $K \in \mathcal{P}(X).$ 





---

***Exercise 7***

**a)**    Both $f|A$ and $f\circ i$ have the same domain ($A$) and codomain ($B$). It remains to be proved that the also have the same value at each $x \in A.$ Indeed, $(f\circ i)(x)$ $=$ $f(i(x))$ $=$ $f(x) = (f|A)(x).$ 

**b)**    $x \in (f|A)^{-1}(B)$ $\Leftrightarrow$ $(x\in A) \and (f(x) \in B)$ $\Leftrightarrow$ $(x \in A) \and (x \in f^{-1}(B))$ $\Leftrightarrow$ $x \in A \cap f^{-1}(B).$ 




[< Home](/index.html)

