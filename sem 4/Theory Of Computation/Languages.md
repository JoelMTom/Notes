### Languages
---
A language is a(finite or infinite) set of strings over a finite alphabet $\sum$.

>[!Note]
>##### The Empty Language
$Let\ L = \{\} = \phi$.
> L is the language that contains no strings
> ##### The Empty Language is Different From the Empty String
>$Let\ L = \{\epsilon\}$, the language that contains a single string, $\epsilon$.
>L is different from $\epsilon$ 

#### Cardinality of a Language
The largest language over any alphabet $\sum$ is $\sum$*. 

$$
\begin{align}
&if\ \sum = \phi.
&Then\ \sum* = \{\epsilon\}\ and\ |\sum*| = 1 
\end{align}
$$

#### Theorem The Cardinality of $\sum$*
>[!INFO]
Theorem: If $\sum \neq \phi$, then $\sum*$ is countably infinite.

#### Theorem An Uncountably Infinite Number of Languages
>[!INFO]
Theorem: If $\sum \neq \phi$, then the set of languages over $\sum$ is uncountably infinite.



##### Kleene  Star
Let L be a language defined over some alphabet $\sum$. Then the Kleene star of L, written L* is:
$$
\begin{align}
&L* = \{\epsilon\} \cup \{w \in \sum* : \exists k \geq 1 (\exists w_1, w_2, … w_k \in L (w = w_1 w_2 … w_k))\}.
\end{align}
$$
$L^+ = LL^*$
$L^+ = L^* - \{\epsilon\}$

##### Theorem ![[Concatenation and Reverse of Languages]]
>[!INFO]
Theorem: If $L_1$ and $L_2$ are languages, then $(L_1 L_2)^R = L_2^R L_1^R$

[[Language Hierarchy]]
[[Theory Of Computation]]
