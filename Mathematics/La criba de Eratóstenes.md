---
tags:
  - Teoríadenúmeros
---
Tema: [[Divisibilidad]]-[[Teoría de números]]

La criba de Eratóstenes es un procedimiento para encontrar primos ideado por el mismo Eratóstenes, el cual permite encontrar los números primos del $1$ hasta el $n$ y consiste en lo siguiente:

1. Enumeras los números hasta el n.
2. Tachas el 1.
3. Avanzas hasta el siguiente que no este tachado y tachas todos sus múltiplos (salvo el propio número).
4. Repites el paso 3 hasta que se acaben los números.

El procedimiento se puede mejorar sabiendo que si un numero es compuesto, entonces debe tener algún divisor en $(1,\sqrt{p}]$.