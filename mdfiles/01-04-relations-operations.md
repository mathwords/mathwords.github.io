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

  



[< Home](/index.html)

