[Home](/index.html)  >  [Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)



**1.1	Logical Symbolism**



---

***Exercise 1***

* The given truth tables serve as definitions of the **negation** $(\neg)$, **conjunction** $(\and)$, **disjunction** $(\or)$ and **implication** $(\Rightarrow)$. They agree with our natural understanding of these logical operators. We make the following memorable observations:

  * $A \and B$ is true iff both $A$ and $B$ are true. 
  * $A \or B$ is false iff both $A$ and $B$ are false. 
  * $A \Rightarrow B$ is false iff $A$ is true and $B$ is false. 

* A peculiar characteristic of the implication statement is worth remarking upon. Based on the truth table for $ A \implies B $, we note in particular that if a statement $A$ is known to be false, then the aforesaid implication statement is true for *any* statement $B.$ We can occasionally use this situation to our advantage. Consider the following statement:
  $$
  x \in \varnothing \implies x \in A
  $$
  Since the "if" part of this statement is always false, it follows that the above implication is a true statement. From the definition of "subset", it then follows that: $ \varnothing \subset A.$ That is to say, the empty set is a subset of any (every) set.


---

***Exercise 2***

(a) and (b) are **De Morgan's laws for logical operations**. (c) states that the **contrapositive** of the implication statement is equivalent to the implication statement. (d) can be considered the definition of the implication in terms of the 3 basic logical operations. (e) states the negation, or the **contradiction** of the implication statement in terms of the 3 basic logical operations.

**a)**    $\neg ( A \wedge B )  \iff \neg A \vee  \neg B$

To obtain the truth table of the negation of a statement, interchange the values of $1$'s and $0$'s in the truth table of the original statement. Applying this procedure to the truth table of $A \and B,$ we obtain the following truth table for $\neg (A \and B).$
$$
\begin{array}{|c|cc|}
\hline
  & (B = 0) & (B = 1) \\ 
\hline
   (A = 0) & 1 & 1 \\
   (A = 1) & 1 & 0 \\ 
\hline
\end{array}
$$
It is easy to see that the above truth table also represents the statement $\neg A \vee  \neg B.$ Indeed, this statement is false iff both $A$ and $B$ are true.

**b)**    $\neg ( A \vee B )  \iff \neg A \wedge  \neg B$

Following the technique stated in the previous problem, we interchange the $1$'s and $0$'s in the truth table of $A \or B$ to obtain the following truth table of $\neg (A \or B).$
$$
\begin{array}{|c|cc|}
\hline
  & (B = 0) & (B = 1) \\ 
\hline
   (A = 0) & 1 & 0 \\
   (A = 1) & 0 & 0 \\ 
\hline
\end{array}
$$

We at once observe that the above truth table also represents the statement $\neg A \and  \neg B.$ Indeed, this statement is true iff both $A$ and $B$ are false.

**c)**    $( A \Rightarrow B )  \iff (\neg B \Rightarrow  \neg A)$

Consider the following truth table of $A \Rightarrow B.$
$$
\begin{array}{|c|cc|}
\hline
  & (B = 0) & (B = 1) \\ 
\hline
   (A = 0) & 1 & 1 \\
   (A = 1) & 0 & 1 \\ 
\hline
\end{array}
$$
Observe that $X \Rightarrow Y$ is false iff $X$ is true and $Y$ is false. Consequently, $\neg B \Rightarrow  \neg A$ is false iff $\neg B$ is true and $\neg A$ is false. In other words, $\neg B \Rightarrow  \neg A$ is false iff $B$ is false and $A$ is true. This is precisely the condition represented in the above truth table.

**d)**    $( A \Rightarrow B )  \iff (\neg A \or B)$

$X \or Y$ is false iff both $X$ and $Y$ are false. Consequently, $\neg A \or B$ is false iff $\neg A$ is false and $B$ is false. In other words, $\neg A \or B$ is false iff $A$ is true and $B$ is false. This corresponds precisely to the truth table of $A \Rightarrow B$ as shown in **(c)** above.

**e)**    $ \neg ( A \Rightarrow B )  \iff ( A \wedge \neg B) $

Negate both sides of **(d)** and apply **(b)** to the right hand side expression.



[< Zorich Solutions](/vaz-ma/vaz-ma-solutions.html)