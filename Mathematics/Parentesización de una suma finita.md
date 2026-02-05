Tema: [[Series de números]]

Sea una sucesión finita $x_1, x_2, \dots, x_n$.

Una **parentesización** de la suma $x_1 + x_2 + \cdots + x_n$ es cualquier expresión construida usando únicamente el símbolo $+$ y paréntesis, tal que:

- Cada $x_i$ aparece **exactamente una vez**,
    
- Se respeta el **orden** $x_1, x_2, \dots, x_n$,


### Definición recursiva

Para $1 \le i \le j \le n$, una expresión $P(i,j)$ es una parentesización de $x_i + x_{i+1} + \cdots + x_j$ si:

- **Base:** si $i=j$, entonces $P(i,i)=x_i$.
    
- **Paso recursivo:** si $i<j$, existe un índice $k$ con $i \le k < j$ tal que $P(i,j)=\big(P(i,k)+P(k+1,j)\big)$.