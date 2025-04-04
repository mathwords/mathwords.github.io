[Home](/index.html)  >  [Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)



**1.3   Functions**



---

***Exercise 1***

**a)**    We first prove that $\forall x \in X, \exists y_1 \in Y$ $((x,y_1) \in \mathcal{R}_1 \and (y_1,x) \in \mathcal{R}_2).$ This establishes *existence* of the image of $x$ in $Y.$ We will then prove that if $\exists (x,y_2) \in \mathcal{R}_1,$ then $y_1 = y_2,$ thereby establishing *uniqueness* of the image of $x$ in $Y.$ 

* $x \in X$ $\implies (x,x) \in \Delta_X$ $\implies (x,x) \in \mathcal{R}_2 \circ \mathcal{R}_1$ $\implies$ $\exists y_1 \in Y ((x,y_1) \in \mathcal{R}_1 \and (y_1,x) \in \mathcal{R}_2).$

* Now, assume further that, $(x,y_2) \in \mathcal{R}_1.$ Then,
  $$
  \begin{align*}
   &((x,y_1) \in \mathcal{R}_1) \and ((x,y_2) \in \mathcal{R}_1) \\
  &\implies (y_1,x) \in \mathcal{R}_2) \and ((x,y_2) \in \mathcal{R}_1 \\
  &\implies (y_1,y_2) \in \mathcal{R}_1 \circ \mathcal{R}_2 \\
  &\implies (y_1,y_2) \in \Delta_Y \\
  &\implies y_1 = y_2
  \end{align*}
  $$

The above arguments establish that $\mathcal{R}_1$ is functional. An exactly analogous argument can be used to establish that the relation $\mathcal{R}_2$ is also functional.  

Furthermore, the above arguments of existence and uniqueness have also established that: $\forall x \in X, \exists! y \in Y$ such that $(x,y) \in \mathcal{R}_1 \and (y,x) \in \mathcal{R}_2.$

Since $\mathcal{R}_1$ and $\mathcal{R}_2$ are both functions, say $f_1$ and $f_2$ respectively, it follows from the above result that:
$$
(f_2(f_1(x)) = x) \and (f_1(f_2(y)) = y).
$$
$\mathcal{R}_1$ and $\mathcal{R}_2$ therefore define mutually inverse mappings of $X$ and $Y.$

**b)**    Let $\mathcal{R} \subset X^2.$ 

* $(\Rightarrow)$ Suppose that $\mathcal{R}$ is transitive. The following reasoning proves that $\mathcal{R} \circ \mathcal{R} \subset \mathcal{R}.$
  $(x_1, x_2) \in \mathcal{R} \circ \mathcal{R}$ $\implies$ $\exists x_3 \in X ((x_1,x_3) \in \mathcal{R} \and (x_3,x_2) \in \mathcal{R})$ $\implies$ $(x_1,x_2) \in \mathcal{R}.$ 
  The first implication follows from the definition of $\mathcal{R} \circ \mathcal{R}.$ The second implication follows from the transitivity of $\mathcal{R}.$  
* $(\Leftarrow)$ Suppose that $\mathcal{R} \circ \mathcal{R} \subset \mathcal{R}.$ The following reasoning proves that $\mathcal{R}$ is transitive.
  $((x_1,x_3) \in \mathcal{R} \and (x_3,x_2) \in \mathcal{R})$ $\implies$ $(x_1, x_2) \in \mathcal{R} \circ \mathcal{R}$  $\implies$ $(x_1,x_2) \in \mathcal{R}.$
  The first implication follows from the definition of $\mathcal{R} \circ \mathcal{R}.$ The second implication is true because $\mathcal{R} \circ \mathcal{R} \subset \mathcal{R}.$  

**c)**    Let $\mathcal{R} \subset X^2.$ 

* $(\Rightarrow)$ Suppose that $\mathcal{R}$ is antisymmetric. The following reasoning proves that $\mathcal{R} \cap \mathcal{R}' \subset \Delta_X.$
  $(x,y) \in \mathcal{R} \cap \mathcal{R}'$ $\implies$ $x\mathcal{R}y \and x\mathcal{R}'y$ $\implies$ $x\mathcal{R}y \and y\mathcal{R}x$ $\implies$ $x = y$ $\implies$ $(x,y) \in \Delta_X.$
  The second implication follows from the definition of $\mathcal{R}'.$ The third implication is true because $\mathcal{R}$ is antisymmetric.
* $(\Leftarrow)$ Suppose that $(f \circ h = \mathrm{id}_Y)$ $\and$ $\neg (f \text{ is surjective}).$ The second condition tells us that $\exists y \in Y,\forall x \in X : (f(x) \ne y).$  The first condition tells us $\forall y \in Y : f(h(y)) = y.$ But $h(y) \in X.$ So we now have $\forall y \in Y,\exists x \in X : (f(x) = y).$ This contradiction establishes that the original assumption is false. Therefore, $(f \circ h = \mathrm{id}_Y)$ $\Rightarrow$ $(f \text{ is surjective}).$

**d)**    Suppose that $(a,b)$ is an arbitrary element of $X^2.$ We have,

$(a,b) \in \mathcal{R} \cup \mathcal{R}'$ $\iff$ $a \mathcal{R} b \or a \mathcal{R}' b$ $\iff$  $a \mathcal{R} b \or b \mathcal{R} a.$



---

***Exercise 2***

**a)**    For the mapping $\mathrm{pr}_1 : X_1 \times X_2 \to X_1,$ the fiber over the singleton $\{ x_1 \} \subset X_1$ is defined by:
$$
f^{-1}(x_1) = \{ (x_1, x) \mid x \in X_2 \}
$$
Similarly, for the mapping $\mathrm{pr}_2 : X_1 \times X_2 \to X_1,$ the fiber over the singleton $\{ x_2 \} \subset X_2$ is defined by:
$$
f^{-1}(x_2) = \{ (x, x_2) \mid x \in X_1 \}
$$
**b)**    An element $x_1 \in X$ will be considered connected with an element $x_2 \in X$ by the relation $\mathcal{R} \subset X^2,$ if $x_1$ and $x_2$ both lie in the same fiber. We verify that $\mathcal{R}$ is an equivalence relation.

* Reflexivity:
  Each element trivially lies in the same fiber as itself. That is $\forall x \in X \big(f(x) = f(x)\big).$ Hence, $x\mathcal{R}x.$

* Symmetry:
  $\forall x_1,x_2 \in X$ we have: $f(x_1) = f(x_2)$ $\Rightarrow$ $f(x_2) = f(x_1).$ Hence, $x_1\mathcal{R}x_2$ $\implies$ $x_2\mathcal{R}x_1.$

* Transitivity:
  $\forall x_1,x_2,x_3 \in X$ we have: $f(x_1) = f(x_2)$ $\and$ $f(x_2) = f(x_3)$ $\implies$ $f(x_1) = f(x_3).$ That is, if $x_1$ and $x_2$ lie in the same fiber, and also $x_2$ and $x_3$ lie in the same fiber, then $x_1$ and $x_3$ lie in the same fiber. Hence, $x_1\mathcal{R}x_2$ $\and$ $x_2\mathcal{R}x_3$ $\implies$ $x_1\mathcal{R}x_3.$

**c)**    Consider the fibers of a mapping $f:X \to Y.$

* The fibers of a mapping do not intersect one another. 
  Indeed, suppose that the $f^{-1}(x_1)$ and $f^{-1}(x_2)$ intersect one another. Then, $\exists x \big(x\in f^{-1}(x_1) \and x \in f^{-1}(x_2) \big).$ But then, $f(x_1) = f(x)$ $\and$ $f(x) = f(x_2).$ Consequently, $f(x_1) = f(x_2).$ In other words, $f^{-1}(x_1)$ and $f^{-1}(x_2)$ represent the same fiber.

* The union of all the fibers is the whole set $X.$
  Let the set $F$ be the union of all the fibers of the given mapping. 
  $x \in X$ $\Rightarrow$ $\exists y \in Y (y = f(x))$ $\Rightarrow$ $x \in f^{-1}(y)$ $\Rightarrow$ $x \in F.$ Hence, $X \subset F.$
  On the other hand, $F \subset X$ follows from the definition of fiber.

**d)**    Suppose that $\mathcal{R} \subset X^2$ is an equivalence relation between the elements of $X.$ We now define the set $[x_i] =\{ x \in X \mid x \mathcal{R} x_i \}$. The sets $[x_i]$ (where $i$ belongs to some indexing set $I$) have the following properties:

* From reflexivity of the equivalence relation, it follows that every element of $X$ belongs to some set $[x_i],$ and that each $[x_i]$ is non-empty.

* Moreover, $\big( x_0 \in [x_i] \big)$ $\wedge$ $\big( x_0 \in [x_j] \big)$ $\implies$  $\big( x_0 \mathcal{R} x_i \big)$ $\wedge$ $\big( x_0 \mathcal{R} x_j \big)$ $\implies$  $\big( x_i \mathcal{R} x_0 \big)$ $\wedge$ $\big( x_0 \mathcal{R} x_j \big)$ $\implies$  $\big( x_i \mathcal{R} x_j \big).$

The first of the above arguments shows that the union of all equivalence classes $[x_i]$ is $X,$ while the second argument shows that the $[x_i]$ so defined are disjoint.



---

***Exercise 3***

In the following, $f : X \to Y,$ is a mapping from $X$ into $Y.$ $A$ and $B$ are subsets of $X,$ while $A'$ and $B'$ are subsets of $Y.$

**a)**    Suppose that $A \subset B.$ 

* $y \in f(A)$ $\Rightarrow$ $\exists x \in A (y = f(x))$ $\Rightarrow$ $(x \in B) \and (y = f(x))$ $\Rightarrow$ $y \in f(B).$ 

  Hence $A \subset B$ $\implies$ $f(A) \subset f(B).$

* To prove that $f(A) \subset f(B)$ $\centernot\implies$ $A \subset B,$ provide a counterexample.

  *<u>Counterexample-1</u>* 

  $f : \mathbb{R} \to \{k\},$ where $k$ is a constant, and $A$ and $B$ are any disjoint sets in $\mathbb{R}.$

  *<u>Counterexample-2</u>*

  $\sin : \mathbb{R} \to [-1,1],$ where $A = [-\pi,0]$ and $B = [0, 2\pi].$ 

**b)**    $A \neq \varnothing$ $\implies$ $x \in A$ $\implies$ $f(x) \in f(A)$ $\implies$ $f(A) \neq \varnothing.$

**c)**    $y \in f(A \cap B)$ $\iff$ $\exists x \in A \cap B$ such that $y = f(x)$ $\iff$ $(x \in A)$ $\and$ $(x \in B)$ $\and$ $y = f(x)$ $\implies$ $y \in f(A) \and y \in f(B)$ $\iff$ $y \in f(A) \cap f(B).$

> [!Note]
>
> Contrast the above chain of reasoning (all equivalences except one) with the reasoning in the next problem (all equivalences).

**d)**   $y \in f(A \cup B)$ $\iff$ $\exists x \in A \cup B$ such that $y = f(x)$ $\iff$ $((x \in A) \or (x \in B))$ $\and$ $y = f(x)$ $\iff$ $((x \in A) \and (y = f(x)))$ $\or$ $((x \in B) \and (y = f(x)))$ $\iff$ $y \in f(A) \cup f(B).$ 

**e)**    Suppose that $A' \subset B'.$ Then,

$x \in f^{-1}(A')$ $\implies$ $\exists y \in A'$ such that $f(x) = y$ $\implies$ $\exists y \in B'$ such that $f(x) = y$  $\implies$ $x \in f^{-1}(B').$

**f)**   $x \in f^{-1}(A' \cap B')$ $\iff$ $\exists y \in A' \cap B'$ such that $y = f(x)$ $\iff$ $(y \in A') \and (y \in B')$ $\and$ $y = f(x)$ $\iff$ $((y \in A') \and (y = f(x)))$ $\and$ $((y \in B') \and (y = f(x)))$ $\iff$ $x \in f^{-1}(A') \cap f^{-1}(B').$ 

**g)**   $x \in f^{-1}(A' \cup B')$ $\iff$ $\exists y \in A' \cup B'$ such that $y = f(x)$ $\iff$ $((y \in A') \or (y \in B'))$ $\and$ $y = f(x)$ $\iff$ $((y \in A') \and (y = f(x)))$ $\or$ $((y \in B') \and (y = f(x)))$ $\iff$ $x \in f^{-1}(A') \cup f^{-1}(B').$ 

**h)**    Suppose that $Y \supset A' \supset B'.$ Then,

$x \in f^{-1}(A'\setminus B')$ $\iff$ $\exists y \in A' \setminus B'$ such that $f(x) = y$ $\iff$ $((y \in A') \and (y \notin B'))$ $\and$ $y = f(x)$ $\iff$ $x \in f^{-1}(A')$ $\and$ $x \notin f^{-1}(B')$ $\iff$ $x \in f^{-1}(A') \setminus f^{-1}(B').$

**i)**   In the solution of Exercise (h) above, replace $A'$ with $Y$ and $B'$ with $A'.$

$x \in f^{-1}(C_YA')$ $\iff$ $\exists y \in C_YA'$ such that $f(x) = y$ $\iff$ $((y \in Y) \and (y \notin A'))$ $\and$ $y = f(x)$ $\iff$ $x \in f^{-1}(Y)$ $\and$ $x \notin f^{-1}(A')$ $\iff$ $x \in X \and x \notin f^{-1}(A')$ $\iff$ $x \in C_Xf^{-1}(A').$ 

**j)**    $x \in A$ $\implies$ $f(x) \in f(A)$ $\iff$ $x \in f^{-1}(f(A)).$

**k)**   $y \in f(f^{-1}(B'))$ $\iff$ $\exists x \in f^{-1}(B')$ such that $y = f(x)$ $\implies$ $y \in B'.$



---

***Exercise 4***

**a)**    Let $f : X \to Y,$ and $B'$ be an arbitrary subset of $Y.$ We will prove that $f$ is surjective if and only if $f(f^{-1}(B')) = B'$ for every set $B' \subset Y.$

* $(\Rightarrow)$  We observe that $f(f^{-1}(B')) \subset B'$ is true for any $f$ as proved in Exercise 3(k). Now suppose that $f$ is surjective and proceed as follows:

  $y \in B'$ $\implies$ $\exists x \in f^{-1}(B')$ such that $y = f(x)$ $\implies$ $y \in f(f^{-1}(B')).$

  Therefore, $B' \subset f(f^{-1}(B')).$

* $(\Leftarrow)$  Suppose that $f(f^{-1}(B')) = B'$ for every $B' \subset Y.$ Then, in particular, the statement is true for $B' = Y.$ Thus, $Y = f(f^{-1}(Y)).$ But $f^{-1}(Y) = X$ by definition. Therefore, we have $Y = f(X),$ so $f$ is surjective.

**b)**    Let $f : X \to Y.$ 

* In Exercise $4(a)$ we have proved that $f$ is surjective if and only if $f(f^{-1}(B')) = B'$ for every set $B' \subset Y.$ 
* From Exercises 5(a) and 5(b) together it follows that $f$ is injective if and only if $f^{-1}(f(A)) = A$ for every set $A \subset X.$

From the two statements above it follows that $f$ is bijective if and only if
$$
\big(f^{-1}(f(A)) = A\big) \and \big(f(f^{-1}(B')) = B' \big)
$$
for every set $A \subset X$ and every set $B' \subset Y.$ 

 

---

***Exercise 5***

**a)** $\iff$ **b)**

* $(\Rightarrow)$ We observe that $ A \subset f^{-1}(f(A))$ is true for any $f$ as proved in Exercise 3(j). Now suppose that $f$ is injective and proceed as follows:

  $x \in f^{-1}(f(A))$ $\implies$ $\exists y \in f(A)$ such that $y = f(x).$ 

  But, $y \in f(A)$ $\implies$ $\exists x' \in A$ such that $y = f(x').$ 

  From the above, it follows that $f(x) = f(x'),$ and since $f$ is injective, it follows that $x = x'.$ But then, $x' \in A,$ and consequently, $f^{-1}(f(A)) \subset A.$

  Therefore, $f^{-1}(f(A)) = A.$

* $(\Leftarrow)$  Suppose that $f^{-1}(f(A)) = A$ for every $A \subset X.$ Then, in particular, the statement is true for each of the singletons $\{ x_1 \}$ and $\{ x_2 \}$ for any $x_1,x_2 \in X.$ We now reason as follows:

  $f(x_1) = f(x_2)$ $\implies$ $f(\{x_1\}) = f(\{x_2\})$ $\implies$ $f^{-1}\big(f(\{x_1\})\big) = f^{-1}\big(f(\{x_2\})\big)$ $\implies$ $\{ x_1 \} = \{ x_2 \}$ $\implies$ $x_1 = x_2.$

  Therefore, $f$ is injective.

**a)** $\iff$ **c)**

* $(\Rightarrow)$  $f(A \cap B) \subset f(A) \cap f(B)$ is true for any $f.$ Indeed, $y \in f(A \cap B)$ $\implies$ $\exists x \in A \cap B$ such that $y = f(x)$ $\implies$ $(x \in A) \and (x \in B) \and y = f(x)$ $\implies$ $y \in f(A) \cap f(B).$

  Let us now assume that $f$ is injective. The following reasoning proves that $f(A) \cap f(B) \subset f(A \cap B).$

  $y \in f(A) \cap f(B)$ $\implies$ $\exists x \in A$ and $\exists x' \in B$ such that $f(x) = f(x') = y.$ But, since $f$ is injective, it follows that $x = x'.$ It follows that $x \in A \cap B,$ and hence $y \in f(A \cap B).$ 

* $(\Leftarrow)$  Suppose that $f(A \cap B) = f(A) \cap f(B)$ for any two subsets $A$ and $B$ of $X.$ Consider arbitrary elements $x_1, x_2 \in X.$ The following reasoning proves that $f$ is injective.

  $f(x_1) = f(x_2) = y$ $\implies$ $y \in f\big(\{ x_1 \}\big) \and y \in f\big(\{ x_2 \}\big)$ $\implies$ $y \in f\big(\{ x_1 \}\big) \cap f\big(\{ x_2 \}\big)$ $\implies$ $y \in f\big(\{ x_1 \} \cap \{ x_2 \}\big)$ $\implies$ $\{ x_1 \} \cap \{ x_2 \} \ne \varnothing$ $\implies$ $x_1 = x_2.$

**a)** $\iff$ **d)**

* $(\Rightarrow)$  $f(A) \cap f(B) = \varnothing$ $\implies$ $A \cap B = \varnothing$ is true for any $f.$ This relationship becomes transparent if we consider the contrapositive of the statement. That is, $A \cap B \ne \varnothing$ $\implies$ $f(A) \cap f(B) \ne \varnothing.$  Now suppose that $f$ is injective. We will prove that $A \cap B = \varnothing$ $\implies$ $f(A) \cap f(B) = \varnothing.$ Once again, let us prove the contrapositive statement, namely, $f(A) \cap f(B) \ne \varnothing$ $\implies$ $A \cap B \ne \varnothing.$ Indeed,

  $f(A) \cap f(B) \ne \varnothing$ $\implies$ $y \in f(A) \cap f(B)$ $\implies$ $\exists x \in A$ and $\exists x' \in B$ such that $f(x) = f(x') = y.$ But, since $f$ is injective, it follows that $x = x'.$ It follows that $x \in A \cap B,$ and therefore $A \cap B \ne \varnothing.$ 

* $(\Leftarrow)$  Suppose that $f(A) \cap f(B) = \varnothing$ $\iff$ $A \cap B = \varnothing.$ The following reasoning proves that $f$ is injective.

  $x_1 \ne x_2$ $\implies$ $\{ x_1 \} \cap \{ x_2 \} = \varnothing$ $\implies$ $f\big(\{ x_1 \}\big) \cap f\big(\{ x_2 \}\big) = \varnothing$ $\implies$ $f(x_1) \ne f(x_2).$

**a)** $\iff$ **e)**

In the following we have, $X \supset A \supset B.$

* $(\Rightarrow)$  $f(A) \setminus f(B) \subset f(A \setminus B)$ is true for any $f.$ Indeed,  

  $y \in f(A) \setminus f(B)$ $\implies$ $y \in f(A) \and y \notin f(B)$ $\implies$ $(\exists x \in A) \and (y = f(x)) \and (x \notin B)$ $\implies$ $(x \in A \setminus B) \and (y = f(x))$ $\implies$ $y \in f(A \setminus B).$ 

  Next, suppose that $f$ is injective. We will prove that $f(A \setminus B) \subset f(A) \setminus f(B).$ When $A \setminus B = \varnothing$ this is obviously true. Now, consider the case when $A \setminus B \ne \varnothing.$ We will prove the assertion in this case by contradiction. Suppose that $f(A \setminus B) \not\subset f(A) \setminus f(B).$ Then,

  $\exists y \in f(A \setminus B)$ such that $y \notin f(A) \setminus f(B)$ $\implies$ $(\exists x \in A)$ $\and$ $(y = f(x))$ $\and$ $(x \notin B)$ $\and$ $\big( (y \notin f(A)) \or (y \in f(B)) \big)$ $\implies$ $(y \in f(A))$ $\and$ $(y = f(x))$ $\and$ $(x \notin B)$ $\and$ $\big( (y \notin f(A)) \or (y \in f(B)) \big)$ $\implies$ $(y \in f(A))$ $\and$ $(y = f(x))$ $\and$ $(x \notin B)$ $\and$ $(y \in f(B))$ $\implies$ $(y = f(x))$ $\and$ $(x \notin B)$ $\and$ $(\exists x' \in B)$ $\and$ $(f(x') = y)$  $\implies$ $\big( f(x) = f(x') \big)$ $\and$ $(x \notin B)$ $\and$ $(x' \in B)$ $\implies$ $(x = x')$ $\and$ $(x \notin B)$ $\and$ $(x' \in B)$ $\implies$ $(x \notin B)$ $\and$ $(x \in B).$

  The contradiction proves that $f(A \setminus B) \subset f(A) \setminus f(B).$

  Therefore, we finally have $f(A \setminus B) = f(A) \setminus f(B).$

* $(\Leftarrow)$  Suppose that $f(A \setminus B) = f(A) \setminus f(B).$ 

  $x_1 \ne x_2$ $\implies$ $\{ x_1, x_2 \} \setminus \{ x_1 \} = \{ x_2 \}$ $\implies$ $f\big(\{ x_1, x_2 \} \setminus \{ x_1 \} \big) = f\big(\{ x_2 \}\big)$ $\implies$ $f\big(\{ x_1, x_2 \} \big) \setminus f\big(\{ x_1 \} \big) = f\big(\{ x_2 \}\big)$ $\implies$ $f(x_2) \notin f\big(\{ x_1 \}\big)$ $\implies$ $f(x_2) \ne f(x_2).$
  
  > [!Warning]
  >
  > We can write $\{ x_2 \}$ as $\{ x_1, x_2 \} \setminus \{ x_1 \}$ only when $x_1 \ne x_2.$

 


---

***Exercise 6***





---





[Home](/index.html)  >  [Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)

