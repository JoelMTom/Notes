#### Regular Expressions and Languages
---
We can recursively define **Regular Expressions**,
For each regular Expression $E$, the language it represent is $L(E)$.

BASIS: The basis consist of three parts:
	- The constant $\epsilon$ and $\phi$ are regular expressions, denoting the languages $\{\epsilon\}$ and $\phi$ respectively. That is, $L(\epsilon) = \{\epsilon\}$, and $L(\phi) = \phi$.
	- If a is any symbol, then **a** is a regular expression. This expression denotes the language $\{a\}$. That is, $L(a) = \{a\}$.
