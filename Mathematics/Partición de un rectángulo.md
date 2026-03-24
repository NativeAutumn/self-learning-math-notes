Tema: [[Integral en Rⁿ]]


Sea $R=\prod_{i=1}^n [a_i,b_i]\subset\mathbb{R}^n$ un rectángulo.  
Una **partición** $P$ de $R$ consiste en elegir, para cada coordenada $i$, una subdivisión finita $a_i=x_{i,0}<x_{i,1}<\cdots<x_{i,k_i}=b_i$. La colección de todos estos puntos determina cómo se “corta” el rectángulo $R$ en piezas más pequeñas.

---

### El conjunto $\mathcal{P}(R)$

$\mathcal{P}(R)$ denota el **conjunto de todas las particiones** posibles del rectángulo $R$. Es decir, $\mathcal{P}(R)$ contiene todas las formas finitas de subdividir $R$ mediante puntos en cada coordenada.

---

### Rectángulos inducidos por una partición

Dada una partición $P\in\mathcal{P}(R)$, los **rectángulos inducidos por $P$** son los subrectángulos de la forma $\prod_{i=1}^n [x_{i,j_i-1},x_{i,j_i}]$, donde para cada $i$ se toma un intervalo consecutivo de la subdivisión en esa coordenada. Intuitivamente, son los “bloques” pequeños en los que queda dividido $R$ al aplicar la partición.