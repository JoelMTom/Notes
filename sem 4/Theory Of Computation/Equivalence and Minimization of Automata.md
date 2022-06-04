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


##### Theorem: 
> [!Info]
> The equivalence of states is transitive. That is, if in some DFA $A = (Q, \sum, \delta, q_0, F)$ we find that states $p$ and $q$ are equivalent, and we also find that $q$ and $r$ are equivalent, then it must be that $p$ and $r$ are equivalent.

###### Theorem: 
> [!Info]
> If we create for each state $q$ of a DFA a block consisting of $q$ and all the states equivalent to $q$, then the different blocks of states form a $partition$ of the set of states.