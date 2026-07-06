# Roles and Responsibilities

## Objetivo

Este documento define los roles y responsabilidades de los integrantes involucrados en el proceso de aseguramiento de la calidad (QA) del proyecto **Cineflix**.

La correcta definición de responsabilidades permite establecer un flujo de trabajo claro durante la planificación, ejecución y seguimiento de las pruebas, facilitando la comunicación entre los miembros del equipo y asegurando la trazabilidad de los defectos identificados durante el desarrollo.

---

# Flujo General del Proceso de QA

```text
Desarrollo
      │
      ▼
Implementación de funcionalidades
      │
      ▼
Validación funcional
      │
      ▼
Reporte de incidencias
      │
      ▼
Corrección
      │
      ▼
Re-testing
      │
      ▼
Pruebas de regresión
      │
      ▼
Aprobación
```

---

# Roles del Proyecto

## Equipo de Desarrollo

### Responsabilidades

- Implementar nuevas funcionalidades.
- Corregir los defectos reportados durante las pruebas.
- Mantener la estabilidad del sistema.
- Garantizar el cumplimiento de los requerimientos funcionales y reglas de negocio.
- Realizar pruebas básicas antes de entregar una funcionalidad al proceso de validación.

### Participación durante QA

El equipo de desarrollo atiende las incidencias reportadas por el equipo de pruebas, realiza las correcciones correspondientes y notifica cuando la funcionalidad se encuentra lista para su validación nuevamente.

---

## Analista de Quality Assurance (QA)

### Responsabilidades

- Diseñar escenarios de prueba.
- Elaborar casos de prueba.
- Ejecutar pruebas funcionales.
- Ejecutar pruebas exploratorias.
- Validar la corrección de defectos (Re-testing).
- Ejecutar pruebas de regresión.
- Documentar evidencias.
- Registrar incidencias detectadas.
- Actualizar la documentación de QA.

### Participación durante QA

El analista de QA actúa como responsable de verificar que las funcionalidades implementadas cumplen con los requerimientos definidos antes de su aprobación.

---

## Equipo Backend

### Responsabilidades

- Implementar la lógica de negocio.
- Mantener la estabilidad de la API REST.
- Corregir incidencias relacionadas con servicios, validaciones o persistencia de datos.
- Garantizar la disponibilidad de los endpoints necesarios para las aplicaciones cliente.

### Participación durante QA

Durante las actividades de validación funcional, el equipo Backend brinda soporte para la resolución de incidencias relacionadas con la API y despliega las correcciones necesarias en el ambiente de pruebas.

---

## Equipo Frontend

### Responsabilidades

- Implementar la interfaz de usuario.
- Integrar los servicios de la API.
- Corregir incidencias relacionadas con la experiencia del usuario.
- Garantizar la correcta navegación entre módulos.

### Participación durante QA

El equipo Frontend realiza ajustes derivados de las observaciones registradas durante la ejecución de las pruebas funcionales.

---

## Coach XP / Responsable Funcional

### Responsabilidades

- Definir los requerimientos funcionales.
- Resolver dudas relacionadas con las reglas de negocio.
- Validar que las funcionalidades implementadas cumplan con los objetivos del proyecto.
- Aprobar cambios funcionales cuando sea necesario.

---

# Responsabilidades durante el Ciclo de Vida del Defecto

| Actividad | Desarrollo | QA | Coach XP |
|-----------|:----------:|:--:|:-------------:|
| Identificación del defecto | | QA | |
| Registro del defecto | | QA | |
| Análisis del defecto | Desarrollo | QA | |
| Corrección | Desarrollo | | |
| Despliegue al ambiente de QA | Desarrollo | | |
| Re-testing | | QA | |
| Pruebas de regresión | | QA | |
| Aprobación final | | QA | Coach XP |

---

# Flujo de Comunicación

Durante el desarrollo del proyecto se adoptó un proceso de comunicación continua entre los integrantes del equipo.

Cuando un defecto era identificado durante la validación de una funcionalidad, este era comunicado directamente al responsable del módulo correspondiente para su análisis y corrección. Una vez implementada la solución, la funcionalidad era desplegada nuevamente en el ambiente de pruebas para ejecutar el proceso de **Re-testing** y, posteriormente, las pruebas de regresión necesarias.

Si bien en las primeras etapas del proyecto gran parte de estas incidencias fueron comunicadas de forma directa sin una documentación formal, en la etapa actual se consolida toda la información dentro del presente repositorio con el objetivo de mantener la trazabilidad de las pruebas y de los defectos detectados.

---

# Matriz RACI

| Actividad | QA | Frontend | Backend | Product Owner |
|-----------|:--:|:--------:|:-------:|:-------------:|
| Elaborar escenarios de prueba | R | C | C | A |
| Diseñar casos de prueba | R | C | C | A |
| Preparar datos de prueba | R | C | C | |
| Ejecutar pruebas funcionales | R | | | |
| Ejecutar pruebas exploratorias | R | | | |
| Registrar defectos | R | | | |
| Analizar defectos | C | R | R | |
| Corregir defectos | | R | R | |
| Desplegar correcciones | | C | R | |
| Ejecutar Re-testing | R | | | |
| Ejecutar regresión | R | | | |
| Aprobar funcionalidad | C | | | A |

**Leyenda**

- **R (Responsible):** Responsable directo de ejecutar la actividad.
- **A (Accountable):** Responsable de la aprobación o decisión final.
- **C (Consulted):** Participa proporcionando información o apoyo técnico.
- **I (Informed):** Es informado sobre el avance o resultado de la actividad.

---

# Consideraciones

El proceso de aseguramiento de calidad implementado en **Cineflix** siguió un enfoque iterativo alineado con la metodología de desarrollo adoptada por el equipo.

Durante el desarrollo, las actividades de validación funcional se realizaron de forma continua conforme se implementaban nuevas funcionalidades. Esto permitió identificar y corregir incidencias tempranamente mediante una comunicación constante entre los equipos de Frontend, Backend y QA.

En la etapa actual del proyecto, correspondiente a la penúltima entrega, se consolida la documentación formal del proceso de pruebas con el propósito de establecer una base documental que facilite la trazabilidad, el mantenimiento del sistema y futuras actividades de evolución o automatización de pruebas.

Nota: Las actividades de QA fueron asumidas por integrantes del equipo de desarrollo (tanto el equipo de frontend como el de backend), especialmente en las etapas iniciales, mediante validaciones funcionales y reportes directos de incidencias. Posteriormente, estas actividades comenzaron a formalizarse con la creación de este repositorio y de la documentación asociada.
---

# Historial de Cambios

| Versión | Fecha | Descripción |
|---------|------|-------------|
| 1.0 | 2026 | Creación inicial del documento de roles y responsabilidades. |