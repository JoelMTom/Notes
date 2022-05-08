#### Finite Automata and Regular Expression
---
>[!INFO]
Theorem: If $L = L(A)$ for some DFA $A$, then there is a regular expression $R$ such that $L =  L(R)$.

##### DFA To RE by Induction Method
---
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
---| --- | ---
 $R_{11}^{(1)}$ | $\epsilon + 1 + (\epsilon + 1)(\epsilon + 1)^*(\epsilon + 1)$ | $1^*$
 $R_{12}^{(1)}$ | $0 + (\epsilon + 1)(\epsilon + 1)^*(0)$ | $1^*0$
 $R_{21}^{(1)}$ | $\phi + \phi(\epsilon + 1)^*(\epsilon + 1)$ | $\phi$
 $R_{22}^{(1)}$ | $\epsilon + 1 + 0 + \phi(\epsilon + 1)^*0$ | $\epsilon + 0 + 1$
 
   Regular Expression | Direct Substitution | Simplified
---| --- | ---
 $R_{11}^{(2)}$ | $1^* + 1^*0(\epsilon + 0 + 1)^*\phi$ | $1^*$
 $R_{12}^{(2)}$ | $1^*0 + 1^*(\epsilon + 0 + 1)^*(\epsilon + 0 + 1)$ | $1^*0(0 +1)^*$
 $R_{21}^{(1)}$ | $\phi + (\epsilon + 0 + 1)(\epsilon + 0 + 1)^*\phi$ | $\phi$
 $R_{22}^{(1)}$ | $\epsilon + 0 + 1 + (\epsilon + 0 + 1)(\epsilon + 0 + 1)^*\epsilon + 0 + 1$ | $(0 + 1)^*$

##### Converting DFA's to Regular Expression by Eliminating States
----
We suppose that the automaton of which $s$ is a state has predecessor states $q_1, q_2, ... , q_k$ for $s$ and sucessor states $p_1, p_2, ... ,p_m$ for $s$. For each arc from one of the $q's$ to s, expression $Q_1$ labels the arc from $q_i$. Similarly,  expression $P_i$ labels the arc from $s$ to $p_i$.

When we eliminate state $s$, all arcs involving state $s$ are deleted. To compensate, we introduce, for each predecessor $q_i$ of $s$ and each successor $p_j$, a regular expression that represents all the paths that starts at $q_i$, go to $s$, perhaps loops around $s$ zero or more times, annd finally go to $p_j$. The expression for this path is $Q_iS^*P_j$ This expression is added to the arc from $q_i$ to $p_j$.
 

The strategy for constructing a regular expression from a finite automaton is as follows:

- For each accepting state $q$ , apply the above reduction process to produce an equivalent automaton with regular-expression labels on the arcs. Eliminate all states except $q$ and the start state $q_0$.
- If $q \neq q_0$, then we shall be left with a two-state automaton like the given Fig.
![[twostate.svg]]
The regular expression for the accepted strings can be described in various ways. One is $(R+SU^*T)^*SU^*$.
- If the start state is also an accepting state, then we must also perform a state-elimination from the original automatonn that gets rid of every state but the start state. Then we are left with one-state automaton that looks like the given Fig. 
![[onestate.svg]]
The regular expressionn denoting the strigs that it accepts is $R^*$.
- The desired regular expression is the sum of all expressions derived from the reduced automata for each accepting state.

#### Example
Consider the NFA that accepts all strings of $0's$ and $1's$ such that either the second ot third position from the end has a $1$.
![[01secthird.svg]]
First eliminate state B, it has one predecessor, A, and one successor, C.
$Q_1 = 1,\ P_1 = 0 + 1,\ R_{11} = \phi,\ and\ S = \phi$.
$\therefore$ The expression on the new arc from A to C is $\phi + 1\phi^*(0+1)$ = $1(0+1)$
![[01secthird1.svg]]
Now eliminate C, 
Regular expression for the arc from A to D is $\phi + 1(0+1)\phi(0+1) = 1(0+1)(0+1).$
![[01secthird2.svg]]
$\therefore$ the regular expression is $((0+1) + 1(0+1)(0+1)\phi^*\phi)^*1(0+1)(0+1)\phi^* = (0+1)^*1(0+1)(0+1)$ 

Now eliminate D,
Regular expression for the arc from A to C is $1(0+1)$
![[01secthird3.svg]]
$\therefore$ the regular Expression is $(0+1 + 1(0+1)\phi^*\phi)^*1(0+1)\phi^* = (0+1)^*1(0+1)$   