---
tags:
  - Teoríadenúmeros
---
Tema: [[Divisibilidad]]-[[Teoría de números]]

**Def**. Dados $a,b \in \mathbb{Z}$ tales que $a\neq 0$ o  $b \neq 0$, se define **el máximo común divisor** de $a$ y $b$, como $$mcd(a,b) = g \in \mathbb{Z}⁺ \mid \begin{cases} g \ | \ a \ \land \ g \ | \ b \\ \forall h \in \mathbb{Z}⁺ \mid h \ | \ a \ \land \ h \ | \ b \ \Rightarrow h \ | \ g\end{cases}$$
*Notemos que esta bien definido, pues siempre $1 \ | \ a$. Si hubiera dos que cumplen lo mismo, entonces $g_1 \ | \  g_2$  y  $g_2 \ | \ g_1$ lo que implica que $|g_1| = |g_2|$ y así  $g_1 = g_2$. Por  lo que es único.

##### Teorema 1
El $mcd(a,b)$ es la minima combinación lineal positiva de $a$ y $b$. Es decir, se ve como: $$mcd(a,b) = at_0 + bs_0 \hspace{0.3cm} \text{minimal}$$
> **Dem**. Sea $g = at_0 + bs_0$  mínimo positivo, entonces si $g \nmid a$  $\exists q,r \in \mathbb{Z}$ con $0< r < g$ tal que $r = a - gq$. Así $r$ es combinación lineal positiva de $a$ y $b$, y además $r < g$, lo cuál es absurdo. Por lo que $g \mid a$  y  $g \mid b$, y cualquier otro que divida a $a$ y $b$ debe dividir a cualquier combinación lineal, incluyendo a $g$.

##### Lema 1
Sean $a,b,q \in \mathbb{Z}$, entonces $mcd(a,b)=mcd(a + bq, b)$.

> **Dem**. El resultado es trivial.

##### Algoritmo de Euclides
Sea $a,b \in \mathbb{Z}$ con $|b| \leq |a|$ , entonces el $mcd(a,b) = r_n$ donde $a = r_{-1}, b = r_0$  y $r_k$ es el residuo de $r_k$ entre $r_{k-1}$ y $r_n$ es el último residuo no cero.

> **Dem**. Se puede suponer que $a$ y $b$ son positivos. Por el lema anterior, $mcd(a,b) = mcd(b, r_1) = ...=(r_n,0) = r_n$. Este proceso termina pues los $r_k$ son estrictamente decrecientes.






