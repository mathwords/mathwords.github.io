[Home](/index.html)  >  [Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)



**I.3   Functions**



---

***Exercise 1***

**a)**    We first prove that $\forall x \in X, \exists y_1 \in Y$ $((x,y_1) \in R_1 \and (y_1,x) \in R_2).$ This establishes *existence* of the image of $x$ in $Y.$ We will then prove that if $\exists (x,y_2) \in R_1,$ then $y_1 = y_2,$ thereby establishing *uniqueness* of the image of $x$ in $Y.$ 

* $x \in X$ $\implies (x,x) \in \Delta_X$ $\implies (x,x) \in R_2 \circ R_1$ $\implies$ $\exists y_1 \in Y ((x,y_1) \in R_1 \and (y_1,x) \in R_2).$

* Now, assume further that, $(x,y_2) \in R_1.$ Then,
  $$
  \begin{align*}
   &((x,y_1) \in R_1) \and ((x,y_2) \in R_1) \\
  &\implies (y_1,x) \in R_2) \and ((x,y_2) \in R_1 \\
  &\implies (y_1,y_2) \in R_1 \circ R_2 \\
  &\implies (y_1,y_2) \in \Delta_Y \\
  &\implies y_1 = y_2
  \end{align*}
  $$

The above arguments establish that $R_1$ is functional. An exactly analogous argument can be used to establish that the relation $R_2$ is also functional.  

Furthermore, the above arguments of existence and uniqueness have also established that:
$$
\forall x \in X, \exists! y \in Y ((x,y) \in R_1 \and (y,x) \in R_2).
$$
Since $R_1$ and $R_2$ are both functions, say $f_1$ and $f_2$ respectively, it follows from the above result that:
$$
(f_2(f_1(x)) = x) \and (f_1(f_2(y)) = y).
$$
$R_1$ and $R_2$ therefore define mutually inverse mappings of $X$ and $Y.$

**b)**    Let $R \subset X^2.$ 

* $(\Rightarrow)$ Suppose that $R$ is transitive. The following reasoning proves that $R \circ R \subset R.$
  $(x_1, x_2) \in R \circ R$ $\implies$ $\exists x_3 \in X ((x_1,x_3) \in R \and (x_3,x_2) \in R)$ $\implies$ $(x_1,x_2) \in R.$ 
  The first implication follows from the definition of $R \circ R.$ The second implication follows from the transitivity of $R.$  
* $(\Leftarrow)$ Suppose that $R \circ R \subset R.$ The following reasoning proves that $R$ is transitive.
  $((x_1,x_3) \in R \and (x_3,x_2) \in R)$ $\implies$ $(x_1, x_2) \in R \circ R$  $\implies$ $(x_1,x_2) \in R.$
  The first implication follows from the definition of $R \circ R.$ The second implication is true because $R \circ R \subset R.$  

**c)**    Let $R \subset X^2.$ 

* $(\Rightarrow)$ Suppose that $R$ is antisymmetric. The following reasoning proves that $R \cap R' \subset \Delta_X.$
  $(x,y) \in R \cap R'$ $\implies$ $xRy \and xR'y$ $\implies$ $xRy \and yRx$ $\implies$ $x = y$ $\implies$ $(x,y) \in \Delta_X.$
  The second implication follows from the definition of $R'.$ The third implication is true because $R$ is antisymmetric.
* $(\Leftarrow)$ Suppose that $(f \circ h = \mathrm{id}_Y)$ $\and$ $\neg (f \text{ is surjective}).$ The second condition tells us that $\exists y \in Y,\forall x \in X : (f(x) \ne y).$  The first condition tells us $\forall y \in Y : f(h(y)) = y.$ But $h(y) \in X.$ So we now have $\forall y \in Y,\exists x \in X : (f(x) = y).$ This contradiction establishes that the original assumption is false. Therefore, $(f \circ h = \mathrm{id}_Y)$ $\Rightarrow$ $(f \text{ is surjective}).$

**d)**    Suppose that $(a,b)$ is an arbitrary element of $X^2.$ We have,

$(a,b) \in R \cup R'$ $\iff$ $a R b \or a R' b$ $\iff$  $a R b \or b R a.$



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



[Home](/index.html)  >  [Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)

