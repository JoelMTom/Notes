####  Algebraic Laws for Regular Expressions
---
##### Associativity and Commutativity
- $L + M = M + L$
- $(L + M) + N = L + (M + N)$
- $(LM)N = L(MN)$

  ##### Identities and Annihilators
- $\phi + L = L + \phi = L$
- $\epsilon L = L \epsilon = L$
- $\phi L = L\phi = \phi$

##### Distributive Laws
-  $L(M + N) = LM + LN$
- $(M + N)L = ML + NL$

##### Example Question
Simplify the regular expression $0 + 01^*$

$$
\begin{aligned}
&0 + 01^* = 0 \epsilon + 01^* \\
&= 0(\epsilon + 1^*) = 01^*\ (Since\ L(1^*)\ have\ \epsilon\ in\ it)
\end{aligned}
$$