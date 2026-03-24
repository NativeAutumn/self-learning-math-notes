
Sea $C\subset[0,1]$ el conjunto ternario de Cantor y $\mathbf{1}_C$ su función indicadora.

Para cada $n\in\mathbb{N}$, definimos

$$
C_n=\bigcup_{k=0}^{2^n-1}  
\left[\frac{x+k}{2^n}, \frac{x+1+k}{2^n} \right] \mid x \in C.  
$$


Definimos la función

$$  
g(x)=\sum_{n=1}^{\infty} 2^{-n},\mathbf{1}_{C_n}(x),  
\qquad x\in[0,1],  
$$

y su subgrafo

$$  
G={(x,y)\in[0,1]^2:\ 0\le y\le g(x)}.  
$$

---

## Preguntas

1. Probar que $g$ está bien definida y es acotada.
    
2. Determinar el conjunto de discontinuidades de $g$.
    
3. Calcular la medida interior de Jordan $m_*(G)$.
    
4. Calcular la medida exterior de Jordan $m^*(G)$.
    
5. Decidir si $G$ es Jordan medible.
    
6. Analizar la frontera $\partial G$.