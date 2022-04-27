# Theory Of Computation
---
## Languages And Strings
### Alphabet

An alphabet is denoted by $\sum$ , a finite set. The members of $\sum$ are called symbols and characters.

### Strings
A string is a finite sequence, possibly empty, of symbols drawn from some alphabet $\sum$. The shortest string that can be formed is the empty string, written as $\epsilon$. The set of all possible strings over an alphabet $\sum$ is written $\sum$*. 

### Functions On Strings
#### Length of string
The **length** of a string s, which we will write as $|s|$, is the number of symbols in $s$. 
$For \  Example$
$$
\begin{aligned}
|\epsilon| = 0 \\
|1001101| = 7
\end{aligned}
$$ 
#### Concatenation of string
The **concatenation** of two strings $s$ and $t$, written $s || t$ or simply $st$, is the string formed by appending $t$ to $s$. 
$For \  example$

$$
\begin{aligned}
if \  x = good \  and \  y = bye, \\ then \  xy = goodbye. \\ So \  |xy| = |x| + |y|. 
\end{aligned}
$$ 
The empty string, $\epsilon$ , is the identity for concatenation of strings. So $\forall x (x\epsilon= \epsilon x = x)$.

Concatenation, as a function defined on strings, is associative. So $\forall s, t, w ((st)w = s(tw))$.

For each string $w$ and each natural number $i$, the string $w^i$ is defined as: $w^0 = \epsilon, \  w^{i+1} = w^i w$ 

#### String Reversal
For each string $w$, the reverse of $w$, which we will write $w^R$ , is defined as: 
$$
\begin{aligned}
if \ |w| = 0 \ then \  w^R = w = \epsilon \\
if |w| \ge  1 then\  \exists a \in \epsilon (\exists u \in \sum* (w = ua)).\\ Then \ define \  w^R = a u^R .
\end{aligned}
$$

##### Theorem ![[Concatenation and Reversal of Strings]]
>[!INFO]
Theorem: If $w$ and $x$ are strings, then $(wx)^R = x^R w^R$ .

#### Relations on Strings
A string $s$ is a **substring** of a string $t$ iff $s$ occurs contiguously as part of $t$. 
$$
\begin{align}
For\ example:\\
&aaa\ is\ a\ substring\ of\ aaabbbaaa\\
&aaaaaa\ is\ not\ a\ substring\ of\ aaabbbaaa
\end{align}
$$
A string $s$ is a **proper substring** of a string $t$ iff $s$ is a substring of $t$ and $s \neq t$.

Every string is a substring of itself. The empty string, $\epsilon$, is a substring of every string.

A string $s$ is a **prefix** of $t$ iff $\exists x \in \sum* (t = sx)$. A string s is a **proper prefix** of a string $t$ iff $s$ is a prefix of $t$ and $s \neq t$. Every string is a prefix of itself. The empty string, $\epsilon$, is a prefix of every string. 
$$
\begin{align}
For\ example,\\
&the\ prefixes\ of\ abba\ are: \epsilon, a, ab, abb, abba.
\end{align}
$$
A string $s$ is a **suffix** of $t$ iff $\exists x \in \sum* (t = xs)$. A string s is a **proper suffix** of a string $t$ iff $s$ is a suffix of $t$ and $s \neq t$. Every string is a suffix of itself. The empty string, $\epsilon$, is a suffix of every string. 

$$
\begin{align}
For\ example,\\
&the\ suffixes\ of\ abba\ are: \epsilon, a, ba, bba, abba.
\end{align}
$$

[[Languages]]
[[Language Hierarchy]]
[[Finite Automata]]



