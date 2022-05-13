##### Theorem:
> [!Info]
> If $L$ is a regular language, so is $L^R$.

proof:

###### By Automata Construction

Given a language $L$ that is $L(A)$ for some finite automaton, perhaps with non-determinism and $\epsilon$-transitions, we may construct an automaton for $L^R$ by:

1. Reverse all the arcs in the transition diagram for A.
2. Make the start state of A be the only accepting state for the new automaton.
3. Create a new start state $p_0$ with transition on $\epsilon$ to all accepting states of A.

The resultant automaton accepts string $w$ if and only if A accepts $w^R$

###### By Regular Expression(by structural induction in size of E)
Assume $L$ is defined by regular expression $E$. We can show that there is another regular expression $E^R$ such that $L(E^R) = (L(E))^R$, that is language of $E^R$ is the reversal of language of $E$.

BASIS:

If $E$ is $\epsilon$, $\phi$ or $a$, then $E^R$ is same as $E$. That is $\{\epsilon\}^R = \{\epsilon\}$, $\phi^R = \phi$ and $\{a\}^R = \{a\}$.

INDUCTION: Three cases:

- $E = E_1 + E_2$. Then $E^R = E_1^R + E_2^R$
- $E = E_1E_2$. Then $E = E_2^RE_1^R$
- $E = E_1^*$. Then $E^R = (E_1^*)$. 

	Any string $w$ in $L(E_1)$ can be written as $w_1w_2...w_n$, where each $w_i$ is in $L(E)$. But $w^R = w_n^Rw_{n-1}^R...w_1^R$.. Each $w_i$ is in $L(E)$, so $w^R$ is in $L()
