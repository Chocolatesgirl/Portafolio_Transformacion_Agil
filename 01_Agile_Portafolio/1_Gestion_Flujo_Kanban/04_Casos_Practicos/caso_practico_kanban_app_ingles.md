# 🧩 Caso Práctico: Implementación de Kanban en App de Inglés para Niños

## 🎯 Contexto

Se implementa un sistema Kanban para gestionar el desarrollo de una:

👉 **Aplicación de aprendizaje de inglés para niños de 3 a 8 años**

El producto tiene como objetivo:

* mejorar la retención de usuarios
* incrementar el engagement mediante experiencias interactivas
* potenciar el aprendizaje mediante audio, juegos y recompensas

---

## 👩‍💼 Rol y enfoque

En este escenario, el rol se enfoca en:

* gestionar el flujo de trabajo end-to-end
* estabilizar la operación del equipo
* implementar métricas para toma de decisiones
* alinear desarrollo con objetivos de producto

👉 El foco no está en gestionar tareas, sino en gestionar el sistema de trabajo.

---

## 🚨 Problema inicial

El equipo presentaba:

* sobrecarga de trabajo en Development
* acumulación en Testing y QA
* falta de visibilidad del estado real del flujo
* alta variabilidad en tiempos de entrega

👉 Resultado:

* Lead Time elevado
* Cycle Time inestable
* baja predictibilidad

---

## 🧠 Objetivo de la implementación

Diseñar un sistema Kanban que permita:

* visualizar el flujo de trabajo end-to-end
* limitar el trabajo en curso (WIP)
* reducir tiempos de entrega
* detectar y resolver bloqueos
* mejorar la predictibilidad

---

## 🧱 Diseño del flujo Kanban

Se definió el siguiente flujo:

```text
Backlog → Ready → Development → Code Review → Testing → QA → Release → Done
```

### Principios aplicados

* flujo continuo (sin dependencia de sprints rígidos)
* trabajo en unidades pequeñas
* políticas explícitas por columna
* gestión activa del flujo

👉 Este diseño se detalla en:
`../01_Diseño_Flujo/diseño_tablero_kanban.md`

---

## ⚙️ Implementación de WIP

Se establecieron límites por etapa:

| Columna     | WIP |
| ----------- | --- |
| Development | 3   |
| Code Review | 2   |
| Testing     | 2   |
| QA          | 2   |

### Decisión clave

Se prioriza **finalización sobre inicio de trabajo**.

👉 Esto permite reducir multitarea y estabilizar el flujo.

Más detalle en:
`../02_Operacion_Flujo/2_politicas_wip.md`

---

## 📊 Métricas utilizadas

Se incorporan métricas de flujo para gestión del sistema:

* **Lead Time** → tiempo total de entrega
* **Cycle Time** → eficiencia del equipo
* **Throughput** → capacidad de entrega
* **WIP** → carga del sistema

👉 Estas métricas se analizan en:
`../03_Metricas_y_Mejora/metricas_flujo.md`

---

## 🔍 Problema detectado (operación real)

Durante la operación del sistema:

👉 Se observa acumulación en **Testing**

### Impacto

* incremento del Cycle Time
* retrasos en entregas
* flujo inestable

👉 El sistema comienza a mostrar un cuello de botella claro.

---

## 🛠️ Decisiones tomadas

A partir de métricas y observación del flujo:

### 1. Control de entrada

* se restringe ingreso de nuevas tareas a Development

---

### 2. Enfoque en finalización

* priorización de tareas en progreso

---

### 3. Redistribución de capacidad

* developers apoyan Testing

---

### 4. Mejora técnica

* fortalecimiento de pruebas automatizadas

---

## 📈 Resultados obtenidos

* reducción del Cycle Time (~30%)
* flujo más estable
* menor acumulación de trabajo
* incremento del throughput
* mayor predictibilidad

---

## 📊 Impacto en el producto

* aumento del tiempo de uso por sesión
* mejora en experiencia de aprendizaje
* mayor interacción con funcionalidades
* feedback positivo de usuarios (niños y padres)

---

## 🔄 Mejora continua

El sistema evoluciona mediante:

* ajuste dinámico de WIP
* reducción del tamaño de historias
* identificación temprana de bloqueos
* uso continuo de métricas

👉 Kanban se utiliza como sistema de mejora continua.

---

## 🔗 Integración del sistema Kanban

Este caso conecta todos los componentes del módulo:

* 🧱 Diseño → estructura del flujo
* 🔄 Operación → comportamiento del sistema
* 🛠️ WIP → control de capacidad
* 📊 Métricas → toma de decisiones

👉 El valor está en la integración, no en cada elemento por separado.

---

## 💼 Enfoque profesional

Este caso refleja competencias en:

* gestión de delivery
* optimización de flujo
* liderazgo de equipos técnicos
* toma de decisiones basada en datos

---

## 🔥 Insight clave

> Mejorar la velocidad del equipo no depende de trabajar más rápido,
> sino de gestionar mejor el flujo de trabajo.

---

## ✅ Conclusión

La implementación de Kanban permitió transformar un sistema reactivo en un sistema:

👉 **estable, medible y predecible**

donde la entrega de valor se vuelve continua y sostenible.
