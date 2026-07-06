# Technology Stack

## Objetivo

Este documento describe el stack tecnológico utilizado durante el desarrollo del ecosistema **Cineflix**, agrupando las tecnologías según su propósito dentro de la arquitectura del sistema y el proceso de aseguramiento de la calidad.

---

# Arquitectura General

| Capa | Tecnologías |
|-------|-------------|
| Frontend Web | React, JavaScript, Tailwind CSS |
| Frontend Backoffice | React, JavaScript, Tailwind CSS |
| Frontend Móvil | React Native, Expo, StyleSheet |
| Backend API | Node.js, Express, TypeScript |
| Base de Datos | PostgreSQL, Sequelize ORM |
| Servicios Externos | ImageKit, Gemini API,  |

---

# Frontend -------------------------------------------------------

## Cliente Web

| Tecnología | Propósito |
|------------|-----------|
| React | Desarrollo de la interfaz de usuario basada en componentes. |
| JavaScript | Lógica del cliente. |
| Tailwind CSS | Diseño responsive y estilos de la aplicación. |

---

## Backoffice

| Tecnología | Propósito |
|------------|-----------|
| React | Desarrollo del panel administrativo. |
| JavaScript | Manejo de la lógica del sistema. |
| Tailwind CSS | Diseño de la interfaz administrativa. |

---

## Aplicación Móvil

| Tecnología | Propósito |
|------------|-----------|
| React Native | Desarrollo multiplataforma para Android e iOS. |
| Expo | Gestión del entorno de desarrollo y compilación. |
| Tailwind CSS | Diseño de la interfaz móvil. |
| StyleSheet | Definición de estilos nativos para la interfaz móvil. |

---

# Backend

| Tecnología | Propósito |
|------------|-----------|
| Node.js | Entorno de ejecución del servidor. |
| Express | Framework para la construcción de la API REST. |
| TypeScript | Tipado estático y escalabilidad del backend. |
| Sequelize ORM | Comunicación entre la API y PostgreSQL mediante modelos. |
| PostgreSQL | Sistema gestor de base de datos relacional. |

---

# Servicios de Terceros

## ImageKit

Servicio utilizado para el almacenamiento, optimización y distribución de imágenes utilizadas por el sistema.

Uso principal:

- Películas
- Productos de confitería
- Imágenes de sucursales
- Eventos
- Otros

## Gemini API

Modelo de Inteligencia Artificial utilizado para implementar el asistente virtual de Cineflix.

Características:

- Capa gratuita.
- Respuestas contextuales.
- Integración mediante API REST.

---

# Herramientas para Desarrollo

| Herramienta | Uso |
|-------------|-----|
| Git | Control de versiones. |
| GitHub | Gestión del código fuente y colaboración. |
| GitHub Actions | Automatización de las pruebas antes de la integración con producción. |
| Postman | Validación manual de endpoints. |
| Bruno | Pruebas manuales de la API REST. |
| Swagger | Documentación e inspección de endpoints REST. |

---

# Herramientas de Testing

## Pruebas Unitarias

### Backend

| Herramienta | Uso |
|-------------|-----|
| Jest | Validación de controladores, servicios y reglas de negocio de la API REST. |

---

## Pruebas de Integración

### Frontend Web

| Herramienta | Uso |
|-------------|-----|
| Vitest | Ejecución de pruebas de integración de componentes React. |
| React Testing Library | Simulación del comportamiento del usuario sobre los componentes. |

---

### Aplicación Móvil

| Herramienta | Uso |
|-------------|-----|
| Jest | Ejecución de pruebas de integración. |
| React Native Testing Library | Validación de componentes y navegación de la aplicación móvil. |

---

## Pruebas End-to-End (E2E)

### Web

| Herramienta | Uso |
|-------------|-----|
| Playwright | Automatización de flujos completos del usuario en la aplicación web. |

---

### Mobile

| Herramienta | Uso |
|-------------|-----|
| Maestro | Automatización de recorridos funcionales en dispositivos móviles. |

---

## Pruebas de API

| Herramienta | Uso |
|-------------|-----|
| Postman | Validación manual de endpoints REST. |
| Bruno | Pruebas funcionales de la API mediante colecciones. |
| Swagger | Verificación del contrato de la API y documentación interactiva. |

---

# Resumen del Ecosistema Tecnológico

| Categoría | Tecnologías |
|-----------|-------------|
| Frontend Web | React, JavaScript, Tailwind CSS |
| Frontend Backoffice | React, JavaScript, Tailwind CSS |
| Mobile | React Native, Expo, StyleSheet |
| Backend | Node.js, Express, TypeScript |
| Base de Datos | PostgreSQL, Sequelize ORM |
| IA | Gemini API |
| Multimedia | ImageKit |
| Versionamiento | Git, GitHub |
| Testing Manual | Postman, Bruno, Swagger |
| Testing Automatizado | Jest, Vitest, React Testing Library, React Native Testing Library, Playwright, Maestro |