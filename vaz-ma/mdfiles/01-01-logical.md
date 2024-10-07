[Home](/index.html)  >  [Solutions](/vaz-ma/vaz-ma-solutions.html)



**1.1	Logical Symbolism**



---

***Exercise 1***

Based on the truth table for $ A \implies B $, we note in particular, that in a given context, if a statement is known to be false, then it implies the truth of  *any* statement. For example:
$$
(1 + 2 = 7) \implies \text{Every circle is a square.}
$$
This construct can be used to prove that the empty set is a subset of any set. We reason as follows:
$$
x \in \varnothing \implies x \in A
$$
Since the left side of the above statement is always false, it implies the truth of the statement on the right. It then follows from the definition of a subset that: $ \varnothing \subset A.$



---

***Exercise 2***

Based on the definition of the negation $( \neg )$, we can arrive at the following conventions for handling truth tables of various operations involving negations:

* To obtain the truth table of the negation of an operation from the truth table of the original operation, interchange the values of 1's and 0's in the table. For example, given that the first truth table below represents $ A \wedge B $, then $ \neg ( A \wedge B )$ is represented by the second table:
  $$
  \begin{array}{|c|cc|}
  \hline
   A \and B & (B = 0) & (B = 1) \\ 
  \hline
     (A = 0) & 0 & 0 \\
     (A = 1) & 0 & 1 \\ 
  \hline
  \end{array}
  $$

  $$
  \begin{array}{|c|cc|}
  \hline
   \neg (A \and B) & (B = 0) & (B = 1) \\ 
  \hline
     (A = 0) & 1 & 1 \\
     (A = 1) & 1 & 0 \\ 
  \hline
  \end{array}
  $$

* To obtain the truth table of an operation when one of the statements involved in the operation is negated, interchange the row (or column) representing the values of the statement when true with its values when false. For example to obtain the table of $  A \wedge  \neg B $ from the table of $ A \wedge B $, interchange the two columns.
  $$
  \begin{array}{|c|cc|}
  \hline
   A \and B & (B = 0) & (B = 1) \\ 
  \hline
     (A = 0) & 0 & 0 \\
     (A = 1) & 0 & 1 \\ 
  \hline
  \end{array}
  $$

  $$
  \begin{array}{|c|cc|}
  \hline
   A \and \neg B & (B = 0) & (B = 1) \\ 
  \hline
     (A = 0) & 0 & 0 \\
     (A = 1) & 1 & 0 \\ 
  \hline
  \end{array}
  $$

* To obtain the truth table of an operation when the implication is reversed, interchange the rows and columns. That is to say, move the element $x_{ij}  $ to the $ji$ position. For example to obtain the table of $  B \implies A $ from the table of $ A \implies B $:
  $$
  \begin{array}{|c|cc|}
  \hline
   A \Rightarrow B & (B = 0) & (B = 1) \\ 
  \hline
     (A = 0) & 1 & 1 \\
     (A = 1) & 0 & 1 \\ 
  \hline
  \end{array}
  $$

  $$
  \begin{array}{|c|cc|}
  \hline
   B \Rightarrow A & (B = 0) & (B = 1) \\ 
  \hline
     (A = 0) & 1 & 0 \\
     (A = 1) & 1 & 1 \\ 
  \hline
  \end{array}
  $$

We now use the above rules to obtain the truth tables for each of the following operations based on the truth tables given in the beginning of section 1.1.5.

**a)**    $ \neg ( A \wedge B )  \iff \neg A \vee  \neg B $
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
**b)**    $ \neg ( A \vee B )  \iff \neg A \wedge  \neg B $
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







[< Home](/index.html)