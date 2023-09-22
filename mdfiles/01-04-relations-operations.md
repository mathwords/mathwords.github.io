[< Home](/index.html)



**I.4   Relations and Operations**



---

***Exercise 1***

We will prove that $f_* : X/\!\! \sim \, \to Y/ \dot\sim$ defined by $f_*([x]) = [f(x)]$ is the function that fulfils the required conditions. 

* Indeed, $(p_Y \circ f)(x)$ $=$ $(p_Y(f(x)))$ $=$ $[f(x)].$ Whereas, $(f_* \circ p_X)(x)$ $=$ $f_* (p_X(x))$ $=$ $f_*([x])$ $=$ $[f(x)].$ Thus, $f_* \circ p_X = p_Y \circ f$ and consequently the given diagram is commutative. 
* Now suppose that $g$ is another function that fulfils the required condition, then we require that $g \circ p_X = p_Y \circ f,$ that is, $g(p_X(x)) = [f(x)].$ But $p_X(x) = [x],$ and $[f(x)] = $ $f_*([x]).$ Hence, $g([x]) = $ $f_*([x]).$ We have proved this result for all $p_X(x) \in X/\!\! \sim.$ But since $p_X$ is surjective, it follows that *every* $[x] \in X/\!\! \sim$ can be written as $p_X(x)$ for some $x \in X.$ We therefore have, $g = f_*$ so that $f_*$ is unique. 



---

***Exercise 2***

Let $X$ be a set with at least two elements and $\mathcal{X} := \mathcal{P}(X)\setminus \{X \}$ with the inclusion order. We will prove that the identity function $\mathcal{X} \to \mathcal{X}, A \mapsto A$ is not bounded. 
Suppose to the contrary that the given function is bounded. Then $\exists B \in \mathcal{X},\forall A \in \mathcal{X} : A \subseteq B.$ But then we have $x \in X$ $\Rightarrow$ $\{x\} \in \mathcal{X}$ $\Rightarrow$ $\{x\} \subseteq B$ $\Rightarrow$ $x \in B.$ That is, $X \subseteq B.$ Whereas, $B \in \mathcal{P}(X)$ $\Rightarrow$ $B \subseteq X.$ It follows that $B = X,$ and hence $X \in \mathcal{X},$ which is a contradiction. The original assumption is False, so that $\forall B \in \mathcal{X},\exists A \in \mathcal{X} : A \not\subseteq B.$ The given function is not bounded.



---

***Exercise 3***

Suppose that $a, b \in X : a \ne b.$ Now consider $f, g \in \text{Funct}(X,X)$ defined by $f(x) = a$ and $g(x) = b.$ We now have $(f \circ g)(x) = a,$ whereas $(g \circ f)(x) = b.$   



---

**Exercise 4**

Let $\circledast$ be an anticommutative operation on $X.$ Then we have, from the given conditions:

1. $x = y \Rightarrow x \circledast y = r$
2. $(x \circledast y) \circledast (y \circledast x) = r \Rightarrow x = y$

Let $X$ be a set that has more than one element. Then, in addition to $r$ (the right identity), $\exists a \in X: a \ne r.$ 

Now, if $\circledast$ is commutative, or if $r$ is also a left identity, then we have in particular: $r \circledast a = a \circledast r.$ It follows from condition (1) that $(r \circledast a) \circledast (a \circledast r) = r.$ But then it follows from condition (2) that $r = a,$ which is a contradiction. Hence, $\circledast$ cannot be commutative.



---

**Exercise 5**

Let $\circledast$ and $\circledcirc$ be anticommutative operations on $X$ and $Y$ respectively. Further, $f : X \to Y$ satisfies:

1. $f(r_X) = r_Y$
2. $f(x \circledast y) = f(x) \circledcirc f(y),$ $\ \ x,y \in X.$

**a)**    Consider $x \sim y\ $ $:\!\!\iff$ $f(x \circledast y) = r_Y.$ 

* The relation is <u>reflexive</u> because $f(x \circledast x)$ $= f(r_X)$ $= r_Y.$ 
* Next, we assume that $f(x \circledast y) = r_Y.$ It follows that $f(x) \circledcirc f(y) = r_Y.$ From the anticommutativity of $\circledcirc,$ we have $f(x) = f(y).$ Whereas, $f(y \circledast x)$ $= f(y) \circledcirc f(x) = r_Y.$ Where the last step follows from the anticommutativity of $\circledcirc$ and the fact that $f(x) = f(y).$ Hence $\sim$ is <u>symmetric</u>.
* Suppose that $x \sim y\ $ and $y \sim z.$ Then, it follows as above that $f(x) = f(y)$ and $f(y) = f(z).$ Thus, $f(x) = f(z).$ From this it follows that $f(x \circledast z)$ $= f(x) \circledcirc f(z)$ $= r_Y.$ Hence, $\sim$ is <u>transitive</u>.

Therefore, $\sim$ is an equivalence relation.

**b)**    Consider the mapping $\tilde{f} : X/\!\! \sim \, \to Y,$ $[x] \mapsto f(x).$ From part (a), recall that we proved that $x \sim y \Leftrightarrow f(x) = f(y).$ It follows that $[x] = [y] \Leftrightarrow f(x) = f(y).$ Therefore, $\tilde{f}$ is well defined and injective. If $f$ is surjective, then $y \in Y \Rightarrow y = f(x).$ But $f(x) = \tilde{f}([x]),$ so that $\tilde{f}$ is also surjective, and hence bijective.   



---

**Exercise 9**

* $A \in \mathcal{A} \Rightarrow A \subseteq \bigcup\mathcal{A}.$ Hence, $\bigcup\mathcal{A}$ is an upper bound of $\mathcal{A}.$ 
  Now, suppose $B$ is any upper bound of $\mathcal{A},$ then $x \notin B$ $\Rightarrow$ $\forall A \in \mathcal{A} : x \notin A$ $\Rightarrow$ $x \notin \bigcup\mathcal{A}.$ Hence, $\bigcup\mathcal{A} \subseteq B.$ Therefore, $\bigcup\mathcal{A}$ is the *least* upper bound of $\mathcal{A}.$
* $A \in \mathcal{A} \Rightarrow \bigcap\mathcal{A} \subseteq A.$ Hence, $\bigcap\mathcal{A}$ is a lower bound of $\mathcal{A}.$ 
  Now, suppose $B$ is any lower bound of $\mathcal{A},$ then $x \in B$ $\Rightarrow$ $\forall A \in \mathcal{A} : x \in A$ $\Rightarrow$ $x \in \bigcap\mathcal{A}.$ Hence, $B \subseteq \bigcap\mathcal{A}.$ Therefore, $\bigcap\mathcal{A}$ is the *greatest* lower bound of $\mathcal{A}.$ 



[< Home](/index.html)

