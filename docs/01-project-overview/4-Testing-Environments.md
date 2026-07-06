# Testing Environments

## Objetivo

Este documento describe los diferentes entornos utilizados durante el proceso de desarrollo y aseguramiento de la calidad (QA) del proyecto **Cineflix**, así como las características, restricciones y finalidad de cada uno de ellos.

La correcta utilización de estos ambientes permite validar nuevas funcionalidades, identificar defectos de forma temprana y garantizar que las pruebas se ejecuten en condiciones controladas sin afectar la información utilizada por el sistema principal.

---

# Arquitectura de Ambientes

El ecosistema de Cineflix se encuentra compuesto por múltiples aplicaciones que consumen una misma API REST.

```text
                 Frontend Web
                       │
                       │
               Frontend Backoffice
                       │
                       │
               Aplicación Móvil
                       │
                       ▼
                 API REST (Node.js)
                       │
          ┌────────────┴────────────┐
          │                         │
          ▼                         ▼
   Base de Datos               Servicios Externos
 (Producción / Pruebas)     (ImageKit, Gemini API)
```

---

# Ambientes Disponibles

Actualmente el proyecto dispone de dos ambientes para la API REST:

| Ambiente | Propósito | Estado |
|----------|-----------|--------|
| Producción | Información oficial utilizada por las aplicaciones del sistema. | Activo |
| Pruebas (QA) | Validación funcional, integración y ejecución de casos de prueba. | Activo |

---

# Ambiente de Producción

## Descripción

Corresponde al ambiente principal utilizado por las aplicaciones del ecosistema Cineflix.

Todas las operaciones realizadas sobre este entorno afectan la información oficial del sistema, por lo que únicamente debe utilizarse para la ejecución normal de la aplicación y para pruebas controladas que no comprometan la integridad de los datos.

### Características

- Base de datos principal.
- Información oficial del sistema.
- Utilizado por:
  - Frontend Web.
  - Backoffice.
  - Aplicación Móvil.
- Debe evitarse la ejecución de pruebas destructivas.

---

# Ambiente de Pruebas (QA)

## Descripción

El ambiente de pruebas fue habilitado con el objetivo de disponer de un entorno aislado para la ejecución de actividades de aseguramiento de calidad sin afectar la información del ambiente principal.

Este ambiente permite validar nuevas funcionalidades, ejecutar pruebas funcionales, realizar pruebas de integración y reproducir defectos reportados durante el desarrollo.

### Características

- Base de datos independiente.
- Información destinada exclusivamente para pruebas.
- Permite crear, modificar y eliminar registros sin comprometer los datos del ambiente principal.
- Utilizado durante la validación de nuevas funcionalidades y la ejecución de casos de prueba documentados.

---

# Aplicaciones que utilizan el ambiente de pruebas

Las siguientes aplicaciones pueden configurarse para consumir el ambiente de QA durante las actividades de validación:

| Aplicación | Uso |
|------------|-----|
| Frontend Web | Validación funcional y pruebas E2E. |
| Frontend Backoffice | Validación de procesos administrativos. |
| Aplicación Móvil | Validación funcional y pruebas de integración. |
| Herramientas de API (Postman / Bruno) | Ejecución manual de endpoints y pruebas exploratorias. |

---

# Tipos de Pruebas Ejecutadas

El ambiente de QA está destinado para la ejecución de las siguientes actividades:

- Pruebas funcionales.
- Pruebas exploratorias.
- Pruebas de integración.
- Validación de correcciones (Retesting).
- Pruebas de regresión.
- Pruebas de endpoints mediante Postman y Bruno.
- Pruebas End-to-End mediante Playwright (Web Backoffice y Cliente).
- Automatización futura mediante Maestro (Mobile).

---

# Datos de Prueba

El ambiente de QA utiliza información destinada exclusivamente para actividades de validación.

Entre los datos disponibles se incluyen:

- Usuarios de prueba.
- Películas.
- Funciones.
- Productos de confitería.
- Sucursales.
- Géneros.
- Eventos.
- Programas de fidelización.
- Suscripciones.
- Historiales de compra simulados.

Estos datos pueden ser modificados o reiniciados durante el proceso de pruebas cuando sea necesario.

---

# Consideraciones

Durante el desarrollo del proyecto, gran parte de las validaciones funcionales fueron realizadas directamente sobre un ambiente de pruebas, permitiendo detectar y corregir incidencias de forma iterativa junto al equipo de desarrollo.

Si bien muchos de estos hallazgos no fueron registrados formalmente durante las primeras etapas del proyecto, la implementación de este repositorio busca centralizar toda la documentación correspondiente al proceso de Quality Assurance, facilitando la trazabilidad de futuras pruebas, la ejecución de regresiones y el mantenimiento evolutivo del sistema.

---

# Buenas Prácticas

- Ejecutar pruebas destructivas únicamente sobre el ambiente de QA.
- No utilizar datos reales durante las actividades de validación.
- Verificar siempre el ambiente configurado antes de ejecutar pruebas.
- Mantener actualizados los datos de prueba cuando se incorporen nuevas funcionalidades.
- Registrar los defectos encontrados durante las pruebas para garantizar su seguimiento y posterior validación.

---

# Historial de Cambios

| Versión | Fecha | Descripción |
|---------|------|-------------|
| 1.0 | 2026 | Creación inicial del documento de entornos de prueba. |