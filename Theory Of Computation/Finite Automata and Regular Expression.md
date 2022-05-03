#### Finite Automata and Regular Expression
---
>[!INFO]
Theorem: If $L = L(A)$ for some DFA $A$, then there is a regular expression $R$ such that $L =  L(R)$.

##### DFA To RE
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
---| ---

  