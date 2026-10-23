
# Programación Concurrente 🤖

## 🎯 Objetivo del módulo

Realizar varias tareas al mismo tiempo para alcanzar un **objetivo en común**, mediante la cooperación y coordinación de múltiples robots.

## 📚 Conceptos importantes

- **Bloquear y liberar:** controlar el acceso a recursos compartidos.
- **Compartir recursos:** permitir que varios robots utilicen recursos en común.
- **Cooperar y coordinarse:** organizar el trabajo entre robots para alcanzar un objetivo compartido.
- **Maximizar la concurrencia:** permitir que la mayor cantidad posible de tareas se ejecuten simultáneamente.
- **Eficiencia:** aprovechar los recursos disponibles y evitar bloqueos o esperas innecesarias.

## 📍 Tipos de áreas

| Tipo de área | Descripción |
|---|---|
| **Privada** | Puede acceder únicamente un robot. |
| **Parcialmente compartida** | Pueden acceder algunos robots, pero no todos. |
| **Compartida** | Pueden acceder todos los robots. |

## ⚠️ Reglas importantes

1. **Áreas disjuntas:** las áreas deben ser disjuntas, es decir, no deben superponerse.
2. **Asignación de áreas:** un robot puede tener asignada más de un área, pero obligatoriamente debe tener al menos una.
3. **Posición inicial:** la esquina inicial de cada robot debe ser diferente.
4. **Tipos de robots:** cuando los trabajos a realizar son diferentes, debe declararse más de un tipo de robot.
5. **Orden de ejecución:** no es posible conocer ni garantizar el orden en que se ejecutan los robots.
