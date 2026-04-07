# 🧱 Diseño de Tablero Kanban — Gestión de Flujo en Producto Digital

## 🎯 Objetivo

Diseñar un sistema Kanban orientado a la **gestión de flujo end-to-end**, permitiendo:

* Visualizar el trabajo desde la idea hasta producción
* Controlar la carga de trabajo (WIP)
* Identificar cuellos de botella
* Mejorar la predictibilidad de entrega

Este diseño está pensado para su implementación en:

* Jira
* Azure DevOps

---

## 🧩 Contexto del caso

Se aplica sobre el desarrollo de una:

👉 **Aplicación de aprendizaje de inglés para niños de 3 a 8 años**

### Problema inicial

* Flujo de trabajo no visible
* Acumulación de tareas en testing
* Alta variabilidad en tiempos de entrega
* Equipos trabajando en múltiples tareas simultáneamente

👉 Resultado:

* Bajo throughput
* Lead Time elevado
* Baja predictibilidad

---

## 🧠 Decisión de diseño

Se define un flujo Kanban que:

* Representa el proceso real (no ideal)
* Incorpora validaciones de calidad explícitas
* Permite medir cada etapa del flujo
* Facilita la gestión basada en métricas

---

## 🔄 Flujo del tablero

```text
Backlog → Ready → Development → Code Review → Testing → QA → Release → Done
```

👉 Cada columna representa un estado del sistema, no solo una actividad.

---

## 📌 Definición de columnas y propósito

### 🧩 Backlog

* Contiene iniciativas priorizadas (épicas/features)
* Fuente de demanda del sistema

👉 No forma parte del flujo activo

---

### 🟡 Ready

* Historias refinadas y priorizadas
* Cumplen Definition of Ready (DoR)

👉 Punto de entrada al sistema Kanban

---

### 🔵 Development

* Construcción de funcionalidad
* Generación de valor inicial

👉 Riesgo: sobrecarga de trabajo (WIP alto)

---

### 🟣 Code Review

* Validación técnica
* Control de calidad de código

👉 Previene deuda técnica

---

### 🟠 Testing

* Validación funcional
* Pruebas integradas

👉 Punto crítico del flujo (frecuente cuello de botella)

---

### 🟢 QA

* Validación de negocio
* Aseguramiento de calidad final

👉 Reduce defectos en producción

---

### 🚀 Release

* Preparación de despliegue
* Validación final técnica

---

### ✅ Done

* Funcionalidad en producción
* Cumple Definition of Done (DoD)

👉 Genera valor real al usuario

---

## ⚙️ Principios de diseño aplicados

### 1. Visualización end-to-end

El flujo cubre desde la solicitud hasta la entrega en producción.

👉 Permite medir Lead Time completo

---

### 2. Control de calidad integrado

Se separan explícitamente:

* Code Review
* Testing
* QA

👉 Evita trasladar defectos aguas abajo

---

### 3. Gestión del flujo, no de tareas

El tablero está diseñado para:

* Limitar trabajo en progreso
* Priorizar finalización sobre inicio

👉 Principio aplicado:
**“Stop starting, start finishing”**

---

### 4. Preparación para métricas

El diseño permite medir:

* Lead Time
* Cycle Time
* Throughput
* WIP por etapa

👉 Base para mejora continua

---

## 📋 Ejemplo de trabajo real (Jira / Azure DevOps)

### 🎮 Feature: Juego de vocabulario interactivo

#### 🧩 Historia

**Título:** Reproducción de audio en palabras

**Objetivo de negocio:**
Mejorar aprendizaje mediante estímulo auditivo

**Criterios de aceptación:**

* Audio reproducible al tocar palabra
* Latencia < 1 segundo
* Compatible con dispositivos móviles

**Tareas técnicas:**

* Integración API de audio
* Desarrollo componente UI
* Manejo de eventos táctiles

---

## 🔒 Políticas clave del tablero

* No iniciar trabajo si WIP está lleno
* Priorizar tareas bloqueadas
* Toda historia debe cumplir DoR para entrar
* Toda historia debe cumplir DoD para salir

---

## 🔍 Ejemplo de comportamiento del sistema

### Situación detectada

* Testing alcanza su límite WIP
* Development continúa iniciando tareas

👉 Impacto:

* Aumento del Cycle Time
* Acumulación de trabajo
* Flujo inestable

---

## 🛠️ Ajustes derivados del diseño

* Reducción de WIP en Development
* Redistribución de capacidad hacia Testing
* Priorización de tareas en progreso

---

## 📈 Impacto del diseño

* Reducción del Lead Time
* Mejora en la estabilidad del flujo
* Mayor predictibilidad de entrega
* Disminución de cuellos de botella

---

## 🔗 Conexión con el sistema Kanban

Este diseño habilita directamente:

* 📊 `metricas_flujo.md` → medición del desempeño
* 📊 `cumulative_flow_explicado.md` → análisis de flujo
* 🔄 `simulacion_flujo_trabajo_jira.md` → operación real
* 🛠️ `politicas_wip.md` → control del sistema

👉 El diseño no es estático: evoluciona con datos.

---

## 💼 Enfoque profesional

Este tablero no es solo una visualización:

Es una herramienta de **gestión de delivery**, que permite:

* Tomar decisiones basadas en flujo
* Optimizar la capacidad del equipo
* Alinear desarrollo con valor de negocio

---

## 🔥 Insight clave

> Un buen tablero Kanban no refleja cómo trabaja el equipo…
> revela cómo debería gestionar su flujo.

---

## ✅ Conclusión

El diseño del tablero es la base del sistema Kanban.

Define cómo fluye el trabajo, cómo se mide y cómo se mejora.

👉 Sin un diseño adecuado, no hay gestión de flujo.
