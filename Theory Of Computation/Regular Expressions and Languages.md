---
aliases: [RE, Regular Expression]
---


#### Regular Expressions and [[Languages]]
---
We can recursively define **[[Regular Expressions and Languages|Regular Expression]]**,
For each regular Expression $E$, the language it represent is $L(E)$.

**BASIS**: The basis consist of three parts:

- The constant $\epsilon$ and $\phi$ are regular expressions, denoting the [[languages]] $\{\epsilon\}$ and $\phi$ respectively. That is, $L(\epsilon) = \{\epsilon\}$, and $L(\phi) = \phi$.
- If a is any symbol, then **a** is a regular expression. This expression denotes the language $\{a\}$. That is, $L(\boldsymbol{a}) = \{a\}$.
- A variable, usually capitalized and italic, like $L$, is a variable, representing any language.

**INDUCTION**: There are four parts to the inductive step:

- If $E$ and $F$ are regular expressions, then $E + F$ is a regular expression denoting the union of $L(E)$ and $L(F)$. $L(E+F) = L(E) \cup L(F)$.
- If $E$ and $F$ are regular expressions, then $EF$ is a regular expression denoting the concatenation of $L(E)$ and $L(F)$. $L(EF) = L(E)L(F)$.
- If $E$ is a regular expression then $E^*$ is a regular expression, denoting the closure of $L(E)$. $L(E^*) = (L(E))^*$.
- If $E$ is a regular expression, then $(E)$, a parenthesized $E$, is also a regular expression, denoting the same language as $E$. $L((E)) = L(E)$

[[Finite Automata and Regular Expression]]
[[Theory Of Computation]]
