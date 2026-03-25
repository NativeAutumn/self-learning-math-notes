---
tags:
  - Teoríadenúmeros
---
Tema: [[Teoría de números]]

**Def.** Dados $a,b \in \mathbb{Z}$. Decimos que **a divide a b**, en caso de que $\exists q \in \mathbb{Z}$ tal que $$b = qa$$en cuyo caso lo denotamos como $a \ | \ b$.

##### Propiedades
*  La divisibilidad es reflexiva y transitiva.
* $\forall a \in \mathbb{Z}$,  $1 \ | \ a$  y  $a \ | \ 0$.
* Si $a \  | \ b$  y  $a \ | \ c$  entonces  $a \ | \ b+c$.
* Si $a \ | \ b$  entonces  $a \ | \ cb$  $\forall c \in \mathbb{Z}$.
* Si $a \ | \ b$  entonces $a \ | \ -b$, $-a \ | \ b$,  $-a \ | \ -b$  y $|a| \ | \ |b|$.
* Si $a \ | \ b$  entonces  $|a| \leq |b|$ 

---
##### El algoritmo de la división
Si $a,b \in \mathbb{Z}$ y $b \neq 0$ entonces $\exists! q,r$ con $0\leq r<|b|$ tales que $$a = bq + r$$
> **Dem**. Usar buen orden para encontrar $q$ tal que $q \leq \frac{a}{b}<q+1$, proponer $r = a - bq$. Para la unicidad notar que $0 \leq r_1 \leq r_2 < |b| \Rightarrow |r_2 - r_1| < |b| \Rightarrow 0 \leq |q_2 - q_1| < 1$.

El algoritmo anterior se puede convertir en un algoritmo de la siguiente forma:

1. Si $a - b < 0$ entonces toma $q = 0$ y $r= a$.
2. En otro caso, busca $t \in \mathbb{Z}$ tal que $a - bt < 0$ y así toma $q = t-1$ y $r = a - bq$.

---

##### Teorema: Euclides
Si $a \mid bc$  y $mcd(a,b)=1$ [[Máximo común divisor | (máximo común divisor)]], entonces $a \mid c$.

> **Dem**. Por [[Máximo común divisor#Teorema 1|Teorema]], $1 = at_0 + bs_0$  y así $c= c(a)t_0 + (cb)s_0$ por lo que $a \mid c$.


##### Corolario 1
Si $p$ es [[Números primos|primo]] y $p \mid ab$ entonces $p \mid a$  o $p \mid b$.

> **Dem**. Si $p \nmid b$, entonces dado que los divisores positivos de $p$ son $1$ y $p$, entonces $mcd(p,b) = 1$ y así por el teorema anterior $p \mid a$.


##### Corolario 2
Si $a \mid c$  y $b \mid c$  y $mcd(a,b)=1$, entonces $ab \mid c$.

> **Dem**. Misma prueba que el teorema: Euclides.

---

#### Ejercicios útiles

1. Si $mcd (a,b) = 1$ y $mcd(a,c) = 1$ entonces $mcd(a,bc)=1$.
2. . Si $mcd (a,b) = 1$, entonces $\forall c \in \mathbb{Z}$ se tienes que $mcd(a,bc) = mcd(a,c)$.
3. $\forall a,b \in \mathbb{Z}$ se tiene que $mcd(\frac{a}{mcd(a,b)}, \frac{b}{mcd(a,b)}) = 1$.
4. Si $mcd(a,b)=1$ entonces todos los divisores de $ab$ son de la forma $cd$, donde $c \mid a$ y $d \mid b$.