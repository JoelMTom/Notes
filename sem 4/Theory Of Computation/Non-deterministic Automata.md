---
aliases: [NDFSM, Non-Deterministic State Machine, NFA, Non-deterministic Automata]
---

#### [[Non-deterministic Automata]]
---
A Non-Deterministic [[Non-deterministic Automata|NDFSM]] M is quintuple $(K, \sum, \Delta, s, A)$, where:
- $K$ is a finite set of states, 
- $\sum$ is an alphabet, 
- $s \in K$ is the start state, 
- $A \subseteq K$ is the set of final states, and 
- $\Delta$ is the transition relation.


##### [[Finite Automata]] With $\epsilon$-Transitions($\epsilon$-[[Non-deterministic Automata|NFA]])

We represent $\epsilon$-NFA A by $A = (Q, \sum, \delta, q_0, F)$, where all components have their same interpretation as for an [[Non-deterministic Automata|NFA]], expect that $\delta$ is now a function that takes as arguments:

- A state in Q,
- A member of $\sum\ \cup\ \{\epsilon\}$, that is, either an input symbol, or the symbol $\epsilon$.

[[Deterministic Finite Automata]]
[[Theory Of Computation]]
[[Regular Expressions and Languages|Regular Expression]]