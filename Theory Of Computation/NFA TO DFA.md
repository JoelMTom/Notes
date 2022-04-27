#### NFA To DFA Conversion
---
$$
\begin{aligned}
Let\ L = \{w \in \{0, 1\}: w\ ends\ with\ 01\}
\end{aligned}
$$

##### [[Non-deterministic Automata|NFA]]

![[end01.svg]]
##### Transition Table for NFA

States/input | 0 | 1 
---| ---| --- 
-> A | {A,B}| {A}
B| $\phi$ | {C}
\*C | $\phi$ | $\phi$

NFA N = ($Q_N$, $\sum$, $\delta_N$, $A$, $F_N$)


##### Transition Table for DFA By Subset Construction
States | 0 | 1
---| --- | ---
 $\phi$ | $\phi$ | $\phi$
 ->{A} | {A,B} | {A}
 {B} | $\phi$| {C}
 \*{C} | $\phi$ | $\phi$
 {A,B} | {A,B} | {A,C}
 \*{A,C} | {A,B} | {A}
 \*{B,C} | $\phi$ | {C}
 {A,B,C} | {A,B} | {A,C} 

Lets name {A} -> A,
{A,B} -> B,
{A,C} -> C

##### [[Deterministic Finite Automata|DFA]]
![[end01dfa.svg]]
