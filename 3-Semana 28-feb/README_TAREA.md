# Tarea – Algoritmos voraces (Greedy) – LeetCode

Tarea del **segundo tema** del curso (algoritmos voraces). Debes resolver **un** problema de optimización en LeetCode aplicando una estrategia greedy, justificando la elección y evaluando la complejidad (según evaluación del curso, cap. XII RE).

---

## Ejercicio: Non-overlapping Intervals

### Enlace a LeetCode

**Non-overlapping Intervals**  
🔗 **https://leetcode.com/problems/non-overlapping-intervals/**

---

### Descripción

- Recibirás un arreglo de intervalos `intervals`, donde `intervals[i] = [start_i, end_i]`.
- Dos intervalos **se solapan** si comparten algún punto en común (por ejemplo `[1, 2]` y `[2, 3]` se solapan en el punto 2).
- Objetivo: devolver el **mínimo número de intervalos que hay que eliminar** para que los intervalos restantes **no se solapen** entre sí.

**Ejemplos:**

- Entrada: `intervals = [[1,2], [2,3], [3,4], [1,3]]`  
  Salida: `1`  
  (Eliminando `[1,3]` los demás no se solapan.)

- Entrada: `intervals = [[1,2], [1,2], [1,2]]`  
  Salida: `2`  
  (Hay que quitar 2 de los 3 para que no haya solapamiento.)

- Entrada: `intervals = [[1,2], [2,3]]`  
  Salida: `0`  
  (Ya no se solapan.)

**Relación con la clase:** En clase vimos el problema de “elegir el **máximo** número de intervalos no solapados” ordenando por tiempo de fin. Este problema es el “complementario”: minimizar cuántos **quitar** para que no haya solapamientos. La misma idea greedy (ordenar por `end` y tomar decisiones en una pasada) aplica: piensa en “cuántos intervalos tendría que eliminar” o en “cuántos me quedo” para no solapar.

---

### Qué se espera

1. **Implementación** en Python que resuelva el problema en LeetCode hasta **Accepted**.
2. **Justificación breve** de por qué tu estrategia greedy es correcta (por ejemplo: criterio de ordenamiento y regla de decisión en cada paso).
3. **Análisis de complejidad**: tiempo y espacio en notación Big O.

---

### Entrega

1. Resuelve el problema en LeetCode hasta **Accepted**.
2. Sube al **repositorio del grupo** (o según indicación del docente):
   - **Pantallazo** donde se vea el enunciado, tu código y el mensaje **Accepted**.
   - El **código** de tu solución.
   - Un breve párrafo (o comentarios en el código) con la **justificación** de la estrategia greedy y el **análisis de complejidad**.

---

**Fecha límite:** Según indicación del profesor en clase o en Teams (evaluación segundo tema: 21/03/2026).
