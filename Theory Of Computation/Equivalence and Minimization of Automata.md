#### Testing Equivalence of States
---
We say that states $p$ and $q$ are $equivalent$ if:

- For all input strings $w$, $\hat\delta(p,w)$ is an accepting state if and only if $\hat\delta(q,w)$ is an accepting state.

If  two states are not equivalent, then we say they are $distinguishable$. That is, if there is at least one string $w$ such that one of $\hat\delta(p,w)$ and $\hat\delta(q,w)$ is accepting, and the other is not accepting.

#### Equivalence of Regular Languages
If the starting states of two [[Deterministic Finite Automata|DFA]] are equivalent then the given [[Deterministic Finite Automata|DFA]]'s are equivalent.

#### Minimization of [[Deterministic Finite Automata|DFA]]'s
---

###### Algorithm:
1. First, eliminate any state that cannot be reached from the start state.
2. Then, partition the remaining states into blocks, so that all states in the same block are equivalent, and no pair of states from different blocks are equivalent.

