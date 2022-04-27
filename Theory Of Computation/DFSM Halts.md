$$
\begin{align}
proof&:\\
&On\ input\ w, M\ executes\ some\ computation\ C_0 |_{-M}\ C_1 |_{-M}\ C_2 |_{-M} … |_{-M} C_n,\\
&where\ C_0\ is\ an\ initial\ configuration\ and\ Cn\ is\ of\ the\ form\ (q, \epsilon),\\
&for\ some\ state\ q \in K_M. C_n\ is\ either\ an\ accepting\ or\ a\ rejecting\ \\
&configuration,\ so\ M\ will\ halt\ when\ it\ reaches\ C_n.\ Each\ step\ in\ the\ \\
&computation\ consumes\ one\ character\ of\ w.\ So\ n = |w|.\ Thus\ M\ will\ halt\\
&after\ |w|\ steps
\end{align}
$$
