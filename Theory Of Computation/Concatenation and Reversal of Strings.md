##### Proof:
$$
\begin{align}
&Proof \ by \  induction\ on \  |x| \\
&Base\  Case:\ |x| = 0.\ Then\ x = \epsilon, and\  (wx)^R  = (w\epsilon)^R = w^R = (\epsilon w)^R = (xw)^R.\\
&Prove: \forall n \ge, ((|x| = n) \rightarrow ((wx)^R = x^Rw^R)) \rightarrow ((|x| = n+1) \rightarrow ((wx)^R = x^Rw^R)).\\ \\
&Consider\  any\  string\  x,\  where\  |x| = n + 1.\ Then\  x = ua\ for\  some\  character\  a\ and\  |u| = n. So:\\
\end{align}
$$
$$
\begin{align}
(w x)^R &= (w (u a))^R  \\
		&= ((w u) a)^R  \\
		&= a (w u)^R  \\
		&= a (u^R w^R )  \\
		&= (a u^R) w^R \\
		&= (ua)^R w^R  \\
		&= x^R w^R 
\end{align}
$$

