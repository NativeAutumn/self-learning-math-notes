
1. **$\mathbb{R}$ no es numerable**

	**Demostración.**  
	Basta probar que el intervalo $[0,1]$ no es numerable, pues $[0,1] \subset \mathbb{R}$.
	
	Supongamos por contradicción que $[0,1]$ es numerable.  
	Entonces existe una biyección
	$$
	f:\mathbb{N}\to [0,1].
	$$
	
	Definimos una sucesión de intervalos cerrados anidados $\{I_n\}$ de la siguiente forma:
	
	- $I_0=[0,1]$.
	- Dado $I_{n-1}$, definimos $I_n$ como:
	  - $I_n=I_{n-1}$ si $f(n)\in I_{n-1}$,
	  - en otro caso, $I_n=[a,b]$, donde $[a,b]\subset I_{n-1}$ y $f(n)\notin [a,b]$.
	
	Notamos que:
	$$
	I_0 \supset I_1 \supset I_2 \supset I_3 \supset \cdots
	$$
	
	Por el **teorema de los intervalos anidados**, se tiene:
	$$
	\bigcap_{n=0}^{\infty} I_n \neq \varnothing.
	$$
	
	Sea $y\in \bigcap_{n=0}^{\infty} I_n$.  
	Entonces $y\in [0,1]$.
	
	Como $f$ es sobreyectiva, existe $m\in\mathbb{N}$ tal que:
	$$
	f(m)=y.
	$$
	
	Pero por construcción, $y\notin I_m$, lo cual contradice que  
	$y\in \bigcap_{n=0}^{\infty} I_n$.
	
	Por lo tanto, $[0,1]$ no es numerable y en consecuencia:
	$$
	\mathbb{R}\ \text{no es numerable} \ \Box
	$$


2. **Todo subconjunto $A \subset \mathbb{R}$ tiene un subconjunto numerable $C \subset A$ tal que $A \subset \overline{C}.$**

	**Demostración**
	Sea
	$$
	\Phi := \{(a,b)\mid a,b \in \mathbb{Q}\ \text{y}\ (a,b)\cap A \neq \varnothing\}.
	$$
	Dado que $\mathbb{Q}\times\mathbb{Q}$ es numerable entonces también $\Phi$, por lo que existe una biyección
	$$
	f: I \subset \mathbb{N} \to \Phi.
	$$
	Sea
	$$
	C := \{x_i \in A \mid x_i \in f(i)\cap A\ \mid i \in I \}.
	$$
	Así, $C \subset A$.
	Sea $x \in A$. Si $x \notin C$, entonces para todo $r>0$ existe $a,b \in \mathbb{Q}$ tales que
	$$
	x-r < a < x < b < x+r.
	$$
	Por lo tanto,
	$$
	(a,b)\cap A \neq \varnothing,
	$$
	y así existe $c \in C$ con $c \neq x$ tal que
	$$
	c \in (x-r,x+r).
	$$
	Por lo que $x \in C^o$. En cualquier caso, $x \in C \lor C^o$ 
	Por consiguiente,
	$$
	A \subset \overline{C}.
	\qquad \square
	$$

