# 🔄 Simulación de Flujo de Trabajo en Jira — Operación Real

## 🎯 Objetivo

Simular la operación real de un sistema Kanban en un equipo de desarrollo, mostrando:

* Cómo fluye el trabajo en el tablero
* Qué problemas emergen en la operación
* Qué decisiones se toman para optimizar el flujo
* Qué impacto tienen dichas decisiones

---

## 🧩 Contexto del caso

Equipo desarrollando una:

👉 **Aplicación de aprendizaje de inglés para niños de 3 a 8 años**

### Situación inicial

* Múltiples historias en progreso simultáneamente
* Testing saturado
* Bloqueos frecuentes
* Falta de visibilidad del flujo

👉 Resultado:

* Cycle Time alto
* Lead Time variable
* Baja predictibilidad

---

## 🧠 Configuración inicial del sistema

### Flujo implementado

```text
Backlog → Ready → Development → Code Review → Testing → QA → Release → Done
```

---

### WIP inicial (antes de mejora)

| Etapa       | WIP |
| ----------- | --- |
| Development | ∞   |
| Code Review | ∞   |
| Testing     | ∞   |

👉 No existían límites → sistema inestable

---

## 🔄 Simulación del flujo (Sprint / Semana de trabajo)

### Día 1

* 5 historias pasan a **Development**
* 2 historias avanzan a **Code Review**

👉 Observación:

* Se inicia mucho trabajo, se termina poco

---

### Día 2

* Code Review se acumula (4 historias)
* Testing recibe solo 1 historia

👉 Problema emergente:

* Desbalance en el flujo

---

### Día 3

* Testing alcanza su capacidad máxima
* Development sigue iniciando nuevas historias

👉 Problema crítico:

* Aumento de WIP
* Tareas detenidas
* Inicio > finalización

---

### Día 4

* Historias bloqueadas en Testing
* Code Review continúa acumulando

👉 Impacto:

* Cycle Time aumenta
* Flujo se vuelve inestable

---

## 🚨 Problemas identificados

### 1. Sobrecarga en Development

* Demasiadas tareas iniciadas
* Falta de foco en finalización

---

### 2. Cuello de botella en Testing

* Capacidad insuficiente
* Acumulación de trabajo

---

### 3. Ausencia de políticas de flujo

* No hay límites WIP
* No hay priorización de bloqueos

---

## 🛠️ Decisiones tomadas

### 1. Implementación de límites WIP

| Etapa       | WIP |
| ----------- | --- |
| Development | 3   |
| Code Review | 2   |
| Testing     | 2   |

---

### 2. Cambio de foco del equipo

👉 De:

* “empezar trabajo”

👉 A:

* “terminar trabajo”

---

### 3. Gestión activa de bloqueos

* Prioridad a tareas detenidas
* Soporte cruzado del equipo

---

### 4. Redistribución de capacidad

* Developers apoyan Testing
* Reducción de multitarea

---

## 🔄 Nuevo comportamiento del sistema

### Día 5–7

* Flujo más continuo
* Menor acumulación
* Mayor movimiento hacia Done

👉 Observación:

* El sistema comienza a estabilizarse

---

## 📊 Impacto medido

| Métrica    | Antes         | Después      |
| ---------- | ------------- | ------------ |
| Lead Time  | Alto          | Reducido     |
| Cycle Time | Variable      | Estable      |
| WIP        | Descontrolado | Limitado     |
| Throughput | Bajo          | Incrementado |

---

## 📈 Interpretación

* Menos trabajo en progreso → mayor velocidad de entrega
* Flujo estable → mayor predictibilidad
* Menos bloqueos → mayor eficiencia

---

## 🔗 Conexión con métricas

Este comportamiento se refleja en:

* 📊 `metricas_flujo.md` → medición de tiempos
* 📊 `cumulative_flow_explicado.md` → visualización del flujo
* 🧱 `diseno_tablero_kanban.md` → base del sistema

👉 La operación valida el diseño.

---

## 💼 Enfoque profesional

La gestión del tablero no es pasiva.

Implica:

* Observación constante del flujo
* Toma de decisiones basada en datos
* Ajuste continuo del sistema

👉 El rol no es administrar tareas, sino gestionar el sistema de trabajo.

---

## 🔥 Insight clave

> El problema no es cuánto trabaja el equipo…
> sino cómo fluye ese trabajo.

---

## ✅ Conclusión

La simulación demuestra que:

* Sin control de WIP, el sistema colapsa
* Sin foco en finalización, no hay entrega de valor
* Sin métricas, no hay mejora real

👉 Kanban no funciona sin gestión activa del flujo.
