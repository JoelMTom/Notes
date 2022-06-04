##### Homomorphisms
----
A string $homomorphism$ is a function on strings that works by substituting a particular string for each symbol.

###### Example
The function h, $h(0) = abb$ and $h(1) = ba$. Thus $h(1011) = baabbbaba$ 

If $h$ is homomorphism on alphabet $\sum$, and $w = a_1a_2...a_n$ is string of symbols in $\sum$, then $h(w) = h(a_1)h(a_2)...h(a_n)$

If $L$ is a language over alphabet $\sum$, and $h$ is a homomorphism on $\sum$, then $h(L) = \{h(w) | w\ is\ in\ L\}$

##### Theorem:
> [!Info]
> If $L$ is a regular language over alphabet $\sum$, and $h$ is a homomorphism on $\sum$, then $h(L)$ is also regular.

