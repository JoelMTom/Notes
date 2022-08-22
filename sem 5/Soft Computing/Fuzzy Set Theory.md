### Fuzzy Set Theory
---

#### Classical Sets

A Classical Set is a set with crisp boundary. For example,

$$
A\ =\ \{x\ |\ x>6\}
$$
#### Fuzzy Sets

##### Basic Definitions And Terminology

A $charactersitic\ function$ for each element $x$ in $X$, we can represent a classical set $A$ by a set of ordered pairs $(x, 0)$ or $(x, 1)$, which indicates $x \notin A$ or $x \in A$, respectively.

##### $Fuzzy\ Sets\ and\ Membership\ functions$

If $X$ is a collection of objects denoted generically by $x$, then a $fuzzy\ set\ A$ in $X$ is defined as a set of ordered pairs: 

$$
A\ =\ \{x\,\ \mu_A(x)\ |\ x\ \in\ X\},
$$
where $\mu_A(x)$ is called  the $membership\ funnction(MF)$ for the fuzzy set $A$. The MF maps each elements of $X$ to a membership grade between 0 and 1.

A fuzzy set can be denoted as follows:
$$
\begin{aligned}
A\ =\ \sum_{x_i \in X }\ & \mu_A(x_i)/x_i\ (discrete)\\
&Or \\
A\ =\ \int_X & \mu_A(x)/x\ (continuous)
\end{aligned}
$$

#### Support
The support of a fuzzy set $A$ is the set of all points $x$ in $X$ such that $\mu_A = 1$:

$$
\begin{aligned}
support(A)\ =\ \{x\ |\ \mu_A(x)\ >\ 0\}
\end{aligned}
$$
#### Core
The core of a fuzzy set $A$ is the set of all points $x$ in $X$ such that $\mu_A(x)\ =\ 1$:
$$
\begin{aligned}
core(A)\ =\ \{x\ |\ \mu_A(X)\ =\ 1\}
\end{aligned}
$$
#### Normality
A fuzzy set $A$ is a $normal$ if its core is nonempty, $i.e,$ we can always find a point $x\ \in\ X$ such that $\mu_A(x)\ =\ 1$.

