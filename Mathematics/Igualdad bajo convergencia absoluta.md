Tema: [[Series de números]]

Si una serie $$\sum_{i=1}^{\infty} x_i$$ converge [[Convergencia absoluta y condicional|absolutamente]], entonces para cualquier [[Re - ordenamientos de series|re - ordenamiento]] $\{x_{\sigma(n)}\}_{n \in \mathbb{N}}$ de $\{{x_n}\}_{n \in \mathbb{N}}$  se tiene que $$\sum_{i=1}^{\infty} x_{\sigma(i)} = \sum_{i=1}^{\infty} x_i$$

> **Esquema demostración**: Si una serie converge absolutamente, entonces $\exists N \in \mathbb{N}$ tal que $\sum_{i=N}^{\infty} |x_i|$ es tan pequeño como quieras, por lo que $\sum_{i=1}^{\infty} x_{\sigma(i)} = \sum_{\sigma(i)<N} x_{\sigma(i)} + \sum_{\sigma(i)\geq N} x_{\sigma(i)}$ debe distar poco de la original, pues $\sum_{\sigma(i)<N} x_{\sigma(i)} = \sum_{i=1}^{N-1} x_i$. Y el **punto clave** 🔑 es que $|\sum_{\sigma(i)\geq N} x_{\sigma(i)}| \leq \sum_{i=N}^{\infty} |x_i|$ pues eso garantiza que la otra parte del sumando se pueda controlar. 

> 🛑 **Error que me paso**: pensar que $\sum_{\sigma(i)\geq N} x_{\sigma(i)} = \sum_{i=N}^{\infty} x_i$ pues aunque tengan los mismos términos las sumas pueden ser distintas.

