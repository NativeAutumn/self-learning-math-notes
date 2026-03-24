
**Enunciado**. Sea $f:A \subset \mathbb{R}^n \to \mathbb{R}^m$ de clase $C^1$  con $n<m$. Demuestre que si $x_0 \in A$  es tal que la matriz $f'(x_0)$  tiene rango $n$, entonces  $f$  es abierta.

**Lema**. Sea $n \in \mathbb{N}$, $r \in \mathbb{R}$  y $x_0 \in \mathbb{R}^n$. Dado lo anterior, existe $f: \mathbb{R}^n \to \mathcal{B}_{r}(x_0)$ inyectiva de clase $C^1$.

**Demostración**. Sea $f: \mathbb{R}^n \to \mathcal{B}_{r}(x_0)$ definida como: $$f(x_1, x_2, ..., x_n) = x_0 + \frac{2r}{\pi n}(arctan(x_1), arctan(x_2),...,arctan(x_n))$$Notemos que $f$ esta bien definida pues$$||x_0-f(\hat{x})||=\frac{2r}{\pi n}||(arctan(x_1), arctan(x_2),...,arctan(x_n))|| \leq$$ $$\frac{2r}{\pi n} \sum_{i=1}^n |arctan(x_i)| \leq \frac{2r}{\pi n} \frac{\pi n}{2} = r$$Por lo que $||x_0-f(\hat{x})|| \leq r$. Así $f(\hat{x}) \in  \mathcal{B}_{r}(x_0)$.

Af. $f$ es inyectiva. Si $f(\hat{x}) = f(\hat{y})$, entonces $$\forall i \in \{1,2,...,n\} \hspace{0.25cm} x_0 + \frac{2r}{\pi}arctan(x_i) = x_0 + \frac{2r}{\pi}arctan(y_i)$$lo que implica que $$arctan(x_i) = arctan(y_i) \Rightarrow x_i = y_i \Rightarrow \hat{x} = \hat{y}$$Por lo que $f$ es inyectiva.

Finalmente, dado que $arctan$ es infinitamente derivable, entonces todas las coordenadas parciales de $f$ son derivables y ademas las derivadas son continuas.

Por lo tanto $f$ es inyectiva de clase $C^1$. 
$\Box$  

**Demostración**. Por contradicción: supongamos que $f$ es abierta.
Por Ejercicio 22 de esta misma tarea $\exists U,V \subset \mathbb{R}^m$ (abiertos) y $g:U \to V$ una biyección de clase $C^1$ en $U$ y $g^{-1}$ de clase $C^1$ en $V$ tal que $$(x_0,\hat{0}) \in V, f(x_0) \in U \hspace{0.2cm} y \hspace{0.2cm} si \ \hat{x} \in f^{-1}[U] \hspace{0.15cm} es  \ tal \ que \ (\hat{x}, \hat{0}) \in V, \ entonces  \hspace{0.15cm} g(f(\hat{x})) = (\hat{x}, \hat{0})$$
Como $U$ es abierto, entonces $\exists \sigma, \mu > 0 \mid \mathcal{B}_{\sigma}(f(x_0)) \subset U$ y $\mathcal{B}_{\mu}((x_0, \hat{0})) \subset V$. Dado que $f$ es $C^1$ y $A$ es abierto, entonces $f$ es continua, por lo que $$\exists \delta \in (0,\mu) \mid \hat{x}\in \mathcal{B}_\delta(x_0) \subset A \Rightarrow f(\hat{x}) \in \mathcal{B}_{\sigma}(f(x_0)) \subset U$$Dado que $f[\mathcal{B}_\delta(x_0)]$ es abierto y $f(x_0) \in f[\mathcal{B}_\delta(x_0)]$, entonces $\exists \epsilon > 0 \mid \mathcal{B}_{\epsilon}(f(x_0)) \subset f[\mathcal{B}_\delta(x_0)]$. Definimos $\Omega := \mathcal{B}_{\epsilon}(f(x_0))$. Evidentemente $\Omega \subset U$ y ademas $\forall \hat{y} \in \Omega$  $\exists \hat{x} \in \mathcal{B}_\delta(x_0) \mid  f(\hat{x}) = \hat{y}$ .
 
Como $g$ es biyectiva y de clase $C^1$ en $U$, entonces $g|_{\Omega}$ es inyectiva y de clase $C^1$ en $\Omega$. Ademas, $g|_{\Omega}(\hat{y}) = g|_{\Omega}(f(\hat{x}))$ para alguna $\hat{x} \in \mathcal{B}_\delta(x_0)$ y dado que $$||(\hat{x}, \hat{0}) - (x_0, \hat{0})|| = || (\hat{x}, x_0)|| < \delta < \mu$$Entonces $(\hat{x}, \hat{0}) \in \mathcal{B}_{\mu}((x_0, \hat{0})) \subset V$, por lo que $g(\hat{y}) = g(f(\hat{x})) = (\hat{x}, 0)$. Así $$g[\Omega] \subset \{(\hat{x},\hat{0}) \in \mathbb{R}^m \mid \hat{x} \in \mathbb{R}^n\} := J^n$$  
 Definamos $\phi: J^n \subset \mathbb{R}^m \to \mathbb{R}^n$ como $\phi((\hat{x}, \hat{0})) = \hat{x}$. Claramente $\phi$ es inyectiva y de clase $C^1$.
 Por lema $\exists h: \mathbb{R}^m \to \Omega$ inyectiva y de clase $C^1$.

Finalmente $h \circ g|_{\Omega} \circ \phi$ es inyectiva y de clase $C^1$ que va de $\mathbb{R}^m$ en $\mathbb{R}^n$. Pero lo anterior es absurdo, ya que por ejercicio 15 de esta misma tarea tal función no puede ser inyectiva.

$\therefore \ f$  no es abierta.
$\Box$ 