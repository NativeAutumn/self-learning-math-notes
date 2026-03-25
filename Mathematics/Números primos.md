---
tags:
  - Teoríadenúmeros
---
Tema: [[Divisibilidad]]-[[Teoría de números]]

**Def**. Decimos que un numero $p \in \mathbb{Z}⁺$  es primo si sus únicos divisores positivos son $1$ y $p$. 

##### Teorema fundamental de la aritmética
Todo entero $a \in \mathbb{Z}$ distinto de $0$ y $\pm 1$ se puede factorizar como producto de primos de manera única, es decir si $$ a = \prod_{i=1}^n q_i = \prod_{i=1}^k p_i$$con $q_i$ y $p_i$ primos, entonces existe una biyección entre los $q_i$ y los $p_i$.

> **Dem**. Para probar que se puede es por inducción fuerte (únicamente concentrándose en valores positivos). Para la biyección, basta notar que si $p_1 p_2 ... p_k = q_1 q_2 ... q_n$, entonces $p_1 \mid  q_1 q_2 ... q_n$ lo que implica que $p_1 \mid q_j$ para algún $j$, osea $p_1 = q_j$. El mismo proceso se hace con todos los demás.

##### Infinitud de los primos
Los  primos son infinitos.

> **Dem**. Supongamos que son finitos, entonces sea $\{1,2,3,5,..., p_k\}$ todos los primos. Notemos que $p_k < \prod p_i + 1$, pero $\forall i \in \{1,2,...,k\}$ $p_i \nmid \prod p_i + 1$. Por lo tanto, este último debe ser un primo mayor que $p_k$, lo cuál es una contradicción.





