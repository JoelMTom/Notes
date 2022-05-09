##### Proof:

$$
\begin{align}
If\ x\ and\ y\ are\ strings,\ & then\ \forall x (\forall y ((xy)^R = y^R x^R ))\\
(L_1 L_2)^R &= \{(xy)^R : x \in L_1\ and\ y \in L_2\}\\
			&= {y^R x^R : x \in L_1 and\ y \in L_2}\\
			&= L_2^R L_1^R
\end{align}
$$
