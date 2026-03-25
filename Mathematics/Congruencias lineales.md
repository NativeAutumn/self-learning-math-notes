---
tags:
  - Teoríadenúmeros
---
Tema: [[Teoría de números]]

**Def**. Una congruencia de la forma $$ax \equiv b \ mod(m)$$Se le llama congruencia lineal, en donde se busca obtener el valor de la $x \in \mathbb{Z}$ que satisfaga la congruencia.

---
##### Teorema 1 (Soluciones congruencia)
La congruencia lineal $ax \equiv b \ mod(m)$ tiene soluciones si y solo si $mcd(a,m) \mid b$, y además las soluciones son de la forma $$x = x_0 +t\frac{m}{mcd(a,m)}$$
> **Dem**. Esto es un consecuencia directa de los resultados obtenidos en las [[Ecuaciones diofantinas lineales]].

Más interesante que obtener las soluciones explicitas de las congruencias lineales es saber cuantas de estas soluciones son diferentes módulo $m$. 

##### Teorema 2 (Cancelar termino, general)
Sea $a,x,y \in \mathbb{Z}$ y $g = mcd(a,m)$. $ax \equiv ay \ mcd(m) \iff x \equiv y \ mcd(\frac{m}{g})$ 

> **Dem**. Para la ida, nos queda que $\frac{a}{g}x \equiv \frac{a}{g}y \ mcd(\frac{m}{g})$ lo que implica que $x \equiv y \ mcd(\frac{m}{g})$ por el [[Divisibilidad#Teorema Euclides|Teorema de Euclides]]. La vuelta es trivial.

##### Teorema 3 (Cantidad soluciones)
Todas las soluciones distintas modulo $m$ de $ax \equiv b \ mod(m)$ son $$x = x_0 + t\frac{m}{mcd(a,m)}$$Donde $t \in \{0,1,...,mcd(a,m)-1\}$ 

> **Dem**. 


