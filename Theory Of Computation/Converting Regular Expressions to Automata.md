#### Converting [[Regular Expressions and Languages|Regular Expression]] to Automata
---
>[!INFO]
Theorem: Every language defined by a regular expression is also defined by finite automaton.

##### Example
Convert the regular expression $(0+1)^*1(0+1)$ to an $\epsilon$-NFA.

First, construct an automaton for $0+1$. We can use two automata, one with label $0$ on the arc and one with label $1$. These two automata are then combined using the union.
![[0+1.svg]]
Now, we apply star construction for the automata for $0+1$.
![[(0+1)s.svg]]
Construct an automata which accepts only the string $1$.

![[1.svg]]

The final automata,
![[(0+1)s1(0+1).svg]]
[[Regular Expressions and Languages]]
