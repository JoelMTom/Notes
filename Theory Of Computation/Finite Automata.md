---
aliases: [FSM, Finite State Machine, FSA, Finite State Automata, FA, Finite Automata]
---

#### Finite Automata
----
A [[Finite Automata|Finite State Machine]] ([[Finite Automata|Finite State Automata]], [[Finite Automata|Finite Automata]]) is a computational device whose input is a string and whose output is one of two values(Accept or Reject).

Two Types of [[Finite Automata|FA]] are: 
- [[Deterministic Finite Automata]]
- [[Non-deterministic Automata]]


>[!INFO]
Theorem: If $D = (Q_D, \sum, \delta_D, \{q_0\}, F_D)$ is the [[Deterministic Finite Automata|DFA]] constructed from [[Non-deterministic Automata|NFA]] $D = (Q_N, \sum, \delta_N, q_0, F_N)$ by the subset construction, then $L(D) = L(N)$


> [!Info]
> Theorem: A language $L$ is accepted by some [[Deterministic Finite Automata|DFA]] if and only if $L$ is accepted by some [[Non-deterministic Automata|NFA]]


[[Theory Of Computation]]