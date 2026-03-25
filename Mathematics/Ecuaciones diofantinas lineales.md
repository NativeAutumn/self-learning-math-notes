---
tags:
  - Teoríadenúmeros
---
Temas: [[Teoría de números]]

**Def**. Una ecuación diofantina lineal de dos incógnitas es de la forma $$ax + by =c$$Donde $a,b,c \in \mathbb{Z}$ y $x,y$ también deben pertenecer a $\mathbb{Z}$. 

##### Teorema 1
La ecuación diofantina $ax+by=c$ tiene soluciones $\iff$  $mcd(a,b) \mid c$.

> **Dem**. $\boxed{\Rightarrow}$  Trivial. $\boxed{\Leftarrow}$ $c = mcd(a,b)q$ y $mcd(a,b) = at_0 + bs_0$ lo que implica que $c = a(qt_0) + b(qs_0)$.

Dado una ecuación diofantina $ax+by =c$, notemos que si $(x_0,y_0)$ y $(x_1,y_1)$ son soluciones, entonces $a(x_0 - x_1) + b(y_0 - y_1) = 0$, y así $(x_0-x_1,y_0-y_1)$ es una solución a la ecuación homogénea.  Además, si $\dot{x_0} = (x_0,y_0)$ es una solución a la ecuación diofantina y $\overline{x} = (c,d)$ es cualquier solución a la ecuación homogénea, entonces $\dot{x_0} + \overline{x}$ es una solución a la ecuación diofantina. Con esto tenemos que todas las soluciones de la ecuación diofantina son de la forma $\dot{x_0} + \overline{x}$.

Dada una ecuación homogénea $ax + by = 0$, si tomamos $x=bt$ y $y = -at$, entonces se satisface la ecuación, sin embargo no todas las soluciones son de esa forma. Para encontrar todas hay que analizar la ecuación $\frac{a}{mcd(a,b)}x + \frac{b}{mcd(a,b)}y=0$, la cual consta de las mismas soluciones que la ecuación anterior y viceversa. Tomando $x=\frac{b}{mcd(a,b)}t$ y $y= -\frac{a}{mcd(a,b)}t$ se satisface la ecuación, pero ahora si tenemos una solución $(c,d)$ de la ecuación, entonces $\frac{a}{mcd(a,b)}c = -\frac{b}{mcd(a,b)}d$, lo que implica que $\frac{b}{mcd(a,b)} \mid c$  pues por [[Divisibilidad#Ejercicios útiles|Ej. 3]] 
$mcd(\frac{a}{mcd(a,b)}, \frac{b}{mcd(a,b)}) = 1$, y con eso  $c=\frac{b}{mcd(a,b)}t$, lo mismo con $d$. Por lo tanto, todas las soluciones a la ecuación homogénea son de la forma  $x=\frac{b}{mcd(a,b)}t$ y $y= -\frac{a}{mcd(a,b)}t$. 

##### Teorema 2
Dada la ecuación diofantina $ax + by = c$, todas las soluciones son de la forma $$x = x_0 + \frac{a}{mcd(a,b)}t, \hspace{0.5cm}y = y_0 - \frac{b}{mcd(a,b)}t$$
donde $(x_0, y_0)$ es una solución particular.

> **Dem**. La prueba es todo el desarrollo previo que se hizo.

==En la practica para resolver ecuaciones diofantinas se checa el mcd para ver si se puede resolver y se hace la combinación lineal del Teorema 1 para obtener la solución particular.==

