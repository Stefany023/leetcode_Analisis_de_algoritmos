# Tarea – Programación dinámica (Clase 14 de marzo)

Resuelve los **2 ejercicios** siguientes con **programación dinámica** (memoización o tabulación). Para cada uno debes:

1. Entregar el **código** de la solución (recomendado en Python; puede probarse en LeetCode).
2. Indicar **subproblema**, **recurrencia** y **casos base**.
3. Dar el **análisis de complejidad** (tiempo y espacio) en notación Big O.

---

## Ejercicio 1: House Robber (LeetCode 198)

🔗 **https://leetcode.com/problems/house-robber/**

- **Entrada:** Arreglo `nums`, donde `nums[i]` es la cantidad de dinero en la casa `i`. Las casas están en línea; no se pueden robar dos casas **adyacentes**.
- **Objetivo:** Maximizar la **cantidad total** que se puede robar.

**Qué se pide:** Definir un subproblema (por ejemplo “máximo beneficio al considerar las primeras `i` casas” o “máximo beneficio hasta la casa `i` según si la robamos o no”), escribir la recurrencia, implementar en DP y dar la complejidad.

---

## Ejercicio 2: Climbing Stairs con costos (LeetCode 746 – Min Cost Climbing Stairs)

🔗 **https://leetcode.com/problems/min-cost-climbing-stairs/**

- **Entrada:** Arreglo `cost`, donde `cost[i]` es el coste del escalón `i`. Puedes empezar en el escalón 0 o en el 1, y en cada paso puedes subir 1 o 2 escalones. Al salir del escalón `i` pagas `cost[i]`. Objetivo: llegar **más allá del último escalón** (arriba de la escalera) con **coste total mínimo**.
- **Objetivo:** Devolver el **coste mínimo** para llegar al tope.

**Qué se pide:** Subproblema (por ejemplo “coste mínimo para llegar al escalón `i`”), recurrencia (elegir entre llegar desde `i-1` o desde `i-2` más el coste correspondiente), implementación DP y análisis de complejidad.

---

## Formato de entrega

Por cada ejercicio incluir:

1. Enlace al problema en LeetCode.
2. Código de la solución (o enlace al envío aceptado).
3. Breve descripción:
   - **Subproblema:** qué representa `dp[i]` (o la tabla que uses).
   - **Recurrencia y casos base.**
   - **Complejidad:** tiempo y espacio en notación O(·).

Entregar según indicación del docente (repositorio, plataforma o correo).
