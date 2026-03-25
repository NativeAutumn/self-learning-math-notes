---
tags:
  - Teoríadenúmeros
---
Tema: [[Divisibilidad]]-[[Teoría de números]]

**Def.** Sean $a,b \in \mathbb{Z}$ con $a,b \neq 0$. Decimos que $mcm[a,b] \in \mathbb{Z}$ es el **mínimo común múltiplo** de $a$ y $b$ si $$mcm[a,b] = m \in \mathbb{Z}⁺ \mid \begin{cases} a \ | \ m \ \land \ b \ | \ m \\ \forall h \in \mathbb{Z}⁺ \mid a \ | \ h \ \land \ b \ | \ h \ \Rightarrow m \leq h\end{cases}$$
*Notemos que esta bien definido pues el hecho de que ambos sean distintos de cero garantiza que existan múltiplos comunes positivos (por ejemplo, |ab|)*

---

##### Lema 1
Sean $a,b \neq 0$. Si $h$ es un múltiplo común de $a$ y $b$, entonces $mcm[a,b] \mid h$.

> **Dem**.  Por el [[Divisibilidad#El algoritmo de la división|Teo]] $\exists q,r \in \mathbb{Z}$ con $0\leq r < mcm[a,b]$ tal que $r = h - mcm[a,b]q$. Notemos que $a \mid r$  y $b \mid r$, y $r < mcm[a,b]$, lo cual no puede pasar a menos de que $r=0$.

##### Teorema 1
Sean $a,b \neq 0$. Se tiene que $mcm[a,b] mcd(a,b) = |ab|$.

> **Dem.** Si $mcd(a,b) = 1$, entonces, dado que $a \mid mcm[a,b]$ y $b$ también, se tiene por [[Divisibilidad#Corolario 2|Cor.2]] que $ab \mid mcm[a,b]$, lo que implica por la [[Divisibilidad#Propiedades | propiedad]] que $|ab| \leq mcm[a,b]$ y entonces $|ab| = mcm[a,b]$. Cuando $mcd(a,b)>1$ se aplica el primer caso a $\frac{a}{mcd(a,b)}$ y $\frac{b}{mcd(a,b)}$, considerando que el $mcm$ y $mcd$ meten escalares positivos.

--- 

#### Ejercicios útiles

1. Si $t>0$, entonces $mcm[ta,tb]=t \ mcm[a,b]$. 
> Aplicar [[Divisibilidad#El algoritmo de la división|El algoritmo de la división]]

2. Si $a = \prod_{i=1}^n p_i ^{e_i}$ y $b = \prod_{i=1}^n p_i ^{d_i}$, entonces $mcm[a,b] = \prod_{i=1}^n p_i ^{max\{d_i,e_i\}}$ 
> Usar que $max\{a,b\} + min\{a,b\} = a+b$ y Aplicar [[Divisibilidad#El algoritmo de la división|El algoritmo de la división]].