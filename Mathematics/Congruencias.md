---
tags:
  - Teoríadenúmeros
---
Tema:[[Teoría de números]]

**Def**. Dados $a,b,m \in \mathbb{Z}$ con $m \geq 1$. Decimos que $a$ es congruente con $b$ módulo m, si $$\exists q \in \mathbb{Z} \hspace{0.3cm} s.t \hspace{0.3cm} m \mid a-b$$En cuyo caso se expresara como $a \equiv b \ mod(m)$.

---
##### Propiedades
Sean $a,b,m \in \mathbb{Z}$, con $m \geq 1$, entonces
* Las congruencias módulo m son una relación de equivalencia.
* $\forall c \in \mathbb{Z}$  si $a \equiv b \ mod(m)$, entonces $ca \equiv cb \ mod(m)$
*  $\forall d \in \mathbb{Z}$  si $a \equiv b \ mod(m)$, entonces $d+a \equiv d+b \ mod(m)$
* Si $a\equiv b \ mod(m)$  y $c \equiv d \ mod(m)$, entonces $a+d \equiv b+c \ mod(m)$
* Si $a\equiv b \ mod(m)$  y $c \equiv d \ mod(m)$, entonces $ad \equiv bc \ mod(m)$

> Para el último, usar transitividad.

---

##### Ejercicios útiles

1. Si $a \equiv b \ mod(m) \Rightarrow mcd(a,m) = mcd(b,m)$ 