[< Home](/index.html)



**I.1 Fundamentals of Logic**



---

***Exercise 1***

Let $H$ represent the statement: ***Homer** will visit the Flanders*. 

And let $M$, $B$, $L$, and $G$ each, be similar statements that claim Marge, Bart, Lisa and Maggie respectively will visit the Flanders. The statements made by Maud Flanders can be constructed from the above statements as follows.

1. $H \Rightarrow M$
2. $G \vee L$
3. $(M \vee B) \wedge \neg(M \wedge B)$
4. $B \Leftrightarrow L$
5. $G \Rightarrow (L \and H)$

If we assume that $L$ is False, then we have:
$$
\neg L \Rightarrow G \Rightarrow L
$$
where the first implication follows from (2), and the second implication follows from (5). We arrive at a contradiction, therefore $L$ is True. We now reason as follows:
$$
L \Rightarrow B \Rightarrow \neg M \Rightarrow \neg H \Rightarrow \neg G
$$
The above implications follow from the statements (4), (3), (1) and (5) respectively.

We therefore conclude that only Lisa and Bart will visit the Flanders.



---

***Exercise 2***

Let $n_B$ represent the number of books in the library of Count Dracula and let $n_W$ represent the total number of words in all the books. Let $E(x)$ be the property that book $x$ contains at least one word. We can now make the following deduction.
$$
\forall x\ E(x) \implies n_W \geq n_B
$$
But this is a contradiction since it is given that $n_W < n_B.$ Hence, the statement $\forall x\ E(x)$ is False. Its negation is therefore True.
$$
\neg(\forall x\ E(x))\ \iff\ \exists x\ \neg E(x)
$$
In other words, there exists a book in Count Dracula's library that contains zero words.





[< Home](/index.html)