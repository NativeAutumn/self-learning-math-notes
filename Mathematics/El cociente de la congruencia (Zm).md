---
tags:
  - Teoríadenúmeros
---
Tema: [[Teoría de números]]

 **Def**. Al conjunto cociente de la relación de congruencia módulo m se le denota como $\mathbb{Z}/m$ y se define como $$\mathbb{Z}/m = \{[a] \mid a \in \mathbb{Z}\} \ \text{donde} \ [a]=\{x\in \mathbb{Z} \mid x \equiv a \ mod(m)\}$$En este sentido $[a]$ es una clase de equivalencia. 

Por el [[Divisibilidad#El algoritmo de la división| algoritmo de la división]] $\forall a \in \mathbb{Z}$  $a=mq+r$, lo que implica que $a \equiv r \ mod(m)$, es decir $a$ es congruente con el residuo que deja con $m$. Notemos que dado dos residuos en $m$, no pueden ser congruentes, pues $|r_2-r_1| < m$. Esto lo que nos dice es que $\mathbb{Z}/m$ tiene exactamente $m$ elementos y son $$\mathbb{Z}/m=\{[0],[1],...,[m-1]\}$$
**Def**. A las clases de equivalencia $[a]$ se les dice **clases residuales módulo m**, a sus elementos $r \in [a]$ se les dice **representantes**. Al elegir un representante de cada una de las clases se forma un **sistema completo de representantes de $\mathbb{Z}/m$**. 

---
##### Operaciones de $\mathbb{Z}/m$
**Def**. Se define la suma de $a,b \in \mathbb{Z}/m$ como $$a+b := [r_1+r_2] \mid r_1\in a \hspace{0.3cm} y \hspace{0.3cm} r_2 \in b$$De igual forma se define el producto como $$ab := [r_1*r_2] \mid r_1\in a \hspace{0.3cm} y \hspace{0.3cm} r_2 \in b$$El hecho de que las operaciones no dependan de los representantes que eliges se explica por las [[Congruencias#Propiedades|propiedades]] de la suma y el producto de las congruencias.

Las propiedades que tienen estas operaciones son similares a las de [[Propiedades de Z|Z]], sin embargo no hay orden y generalmente no es un dominio entero. 

---
##### Teorema 1
Sea $[a] \in \mathbb{Z}/m$. $[a]$ tiene inverso multiplicativo $\iff$ $mcd(a,m)=1$

> **Dem**. Esto se deduce del hecho de que la ecuación $ax-my=1$ tiene soluciones sii $mcd(a,m)=1$ por [[Ecuaciones diofantinas lineales#Teorema 1|Teorema]], la cual es equivalente a buscar una $x$ tal que $ax \equiv 1 \ mod(m)$. 


##### Teorema 2
$\mathbb{Z}/m$ es un campo si y solo $m$ es primo

> **Dem**. Por el teorema anterior si $p$ es primo, entonces todos los elementos de $\mathbb{Z}/m \setminus {0}$ tienes inverso multiplicativo (por [[Congruencias#Ejercicios útiles|Ejercicio]]). Si para todo $[a] \in \mathbb{Z}/m$ tiene inverso multiplicativo, entonces por el teorema anterior $mcd(m,k)=1$ con $k \in \{1,2,...,k-1\}$, por lo que $m$ es primo.

