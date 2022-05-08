#### Finite Automata and Regular Expression
---
>[!INFO]
Theorem: If $L = L(A)$ for some DFA $A$, then there is a regular expression $R$ such that $L =  L(R)$.

##### DFA To RE
---
For example,
![[dfatore.svg]]
$$
R_{ij}^{(k)} = R_{ij}^{(k-1)} + R_{ik}^{(k-1)}(R_{kk}^{(k-1)})^*R_{kj}^{(k-1)}
$$

Regular Expression | Direct Substitution
---| ---
 $R_{11}^{(0)}$ | $\epsilon + 1$
 $R_{12}^{(0)}$ | $0$
 $R_{21}^{(0)}$ | $\phi$
 $R_{22}^{(0)}$ | $\epsilon + 1 + 0$

 Regular Expression | Direct Substitution | Simplified
---| --- | ---
 $R_{11}^{(1)}$ | $\epsilon + 1 + (\epsilon + 1)(\epsilon + 1)^*(\epsilon + 1)$ | $1^*$
 $R_{12}^{(1)}$ | $0 + (\epsilon + 1)(\epsilon + 1)^*(0)$ | $1^*0$
 $R_{21}^{(1)}$ | $\phi + \phi(\epsilon + 1)^*(\epsilon + 1)$ | $\phi$
 $R_{22}^{(1)}$ | $\epsilon + 1 + 0 + \phi(\epsilon + 1)^*0$ | $\epsilon + 0 + 1$
 
   Regular Expression | Direct Substitution | Simplified
---| --- | ---
 $R_{11}^{(2)}$ | $1^* + 1^*0(\epsilon + 0 + 1)^*\phi$ | $1^*$
 $R_{12}^{(2)}$ | $1^*0 + 1^*(\epsilon + 0 + 1)^*(\epsilon + 0 + 1)$ | $1^*0(0 +1)^*$
 $R_{21}^{(1)}$ | $\phi + (\epsilon + 0 + 1)(\epsilon + 0 + 1)^*\phi$ | $\phi$
 $R_{22}^{(1)}$ | $\epsilon + 0 + 1 + (\epsilon + 0 + 1)(\epsilon + 0 + 1)^*\epsilon + 0 + 1$ | $(0 + 1)^*$

##### Converting DFA's to Regular Expression by Eliminating States
----
We suppose that the automaton of which $s$ is a state has predecessor states $q_1, q_2, ... , q_k$ for $s$ and sucessor states $p_1, p_2, ... ,p_m$ for $s$. For each arc from one of the $q's$ to s, expression $Q_1$ labels the arc from $q_i$. Similarly,  expression $P_i$ labels the arc from $s$ to $p_i$.
 

The strategy for constructing a regular expression from a finite automaton is as follows:

- For each accepting state $q$ , apply the 