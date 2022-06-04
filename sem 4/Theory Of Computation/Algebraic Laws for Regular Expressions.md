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
##### The Idempotent Law
- $L + L = L$

##### Laws Involving Closures
- $(L^*)^* = L^*$
- $\phi^* = \epsilon$
- $\epsilon^* = \epsilon$
- $L^+ = LL^* = L^*L$
- $L^* = L^+ + \epsilon$

>[!INFO]
Theorem: Let $E$ be a regular expression with variables $L_1, L_2, ... , L_m.$ Form concrete regular expression $C$ by replacing each occurence of $L_i$ by the symbol $a_i$ for $i = 1,2, ..., m$. Then for any languages $L_1, L_2, ..., L_m$, every string $w$ in $L(E)$ can be written $w = w_1w_2...w_k$, where each $w_i$ is one of the languages, say $L_{j_i}$, and the string $a_{j_1}a_{j_2}...a_{j_k}$ is in the language $L(C)$.  Less formally, we can construct $L(E)$ by starting with each string in $L(C)$, say $a_{j_1}a_{j_2}...a_{j_k}$, and substituting for each of the $a_{j_i}$'s any string from the corresponding language $L_{j_i}.$





