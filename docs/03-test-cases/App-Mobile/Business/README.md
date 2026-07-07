# Business - Manual Test Cases

## Información General

Módulo: Business
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Validar el correcto funcionamiento del módulo, verificando que la información institucional de Cineflix sea presentada de forma clara, consistente y accesible para los usuarios.

Las pruebas contemplan la correcta visualización del contenido, la navegación entre las diferentes secciones del módulo, el comportamiento responsive de la interfaz y el cumplimiento de criterios básicos de accesibilidad.

Dado que este módulo corresponde a una sección informativa y no posee integración con servicios backend, las actividades de prueba se centran en la experiencia del usuario y la correcta presentación del contenido.

---

# Alcance

Las pruebas documentadas en este módulo comprenden la validación de:

- Información corporativa.
- Información de marketing empresarial.
- Términos y condiciones.
- Navegación entre secciones.
- Correcta visualización del contenido.
- Consistencia visual.
- Accesibilidad.

No forman parte del alcance:

- Validaciones de Base de Datos.
- Consumo de API REST.
- Procesos de autenticación.
- Persistencia de información.
- Operaciones CRUD.


## Functional Testing

# Visualización General
TC-BUS-001 – Visualizar correctamente la pantalla Business - "Empresa".
TC-BUS-002 – Verificar que toda la información cargue completamente.
TC-BUS-003 – Verificar que no existan bloques de contenido vacíos.
TC-BUS-004 – Verificar que no existan textos truncados.
TC-BUS-005 – Verificar que las imágenes se visualicen correctamente.
TC-BUS-006 – Verificar que los íconos sean visibles.
TC-BUS-007 – Verificar que el contenido mantenga el orden establecido.
TC-BUS-008 – Verificar que no existan componentes superpuestos.
TC-BUS-009 – Verificar que el scroll funcione correctamente.
TC-BUS-010 – Verificar que la pantalla cargue sin errores visuales.

# Marketing Empresarial
TC-BUS-011 – Verificar la visualización del apartado Marketing Empresarial.
TC-BUS-012 – Verificar que todo el contenido sea visible.
TC-BUS-013 – Verificar la correcta organización de los párrafos.
TC-BUS-014 – Verificar la correcta visualización de imágenes asociadas.
TC-BUS-015 – Verificar que no existan espacios en blanco innecesarios

# Términos y Condiciones
TC-BUS-016 – Verificar la visualización del apartado Términos y Condiciones.
TC-BUS-017 – Verificar que el contenido sea completamente visible.
TC-BUS-018 – Verificar que las listas numeradas o con viñetas se muestren correctamente.
TC-BUS-019 – Verificar que el formato del texto sea consistente.
TC-BUS-020 – Verificar que los encabezados se distingan correctamente.

## Information Testing

# Contenido
TC-BUS-021 – Verificar ortografía del contenido.
TC-BUS-022 – Verificar gramática.
TC-BUS-023 – Verificar redacción.
TC-BUS-024 – Verificar consistencia del lenguaje utilizado.
TC-BUS-025 – Verificar uso correcto de mayúsculas.
TC-BUS-026 – Verificar uso correcto de signos de puntuación.
TC-BUS-027 – Verificar nombres de la empresa.
TC-BUS-028 – Verificar consistencia de la identidad corporativa.
TC-BUS-029 – Verificar números telefónicos.
TC-BUS-030 – Verificar direcciones de correo electrónico.
TC-BUS-031 – Verificar enlaces externos (Footer).
TC-BUS-032 – Verificar URLs mostradas (Footer).
TC-BUS-033 – Verificar información de contacto.
TC-BUS-034 – Verificar consistencia de logos e imágenes.

## Navigation Testing
TC-BUS-035 – Acceder al módulo desde el home.
TC-BUS-036 – Regresar correctamente a la pantalla anterior.
TC-BUS-037 – Navegar entre las diferentes secciones.
TC-BUS-038 – Verificar funcionamiento del scroll.
TC-BUS-039 – Verificar enlaces internos.
TC-BUS-042 – Verificar navegación utilizando el botón "Atrás".
TC-BUS-043 – Verificar navegación utilizando el menú principal.

## Responsive Testing

# Tablet
TC-BUS-046 – Visualización en tablet vertical.
TC-BUS-047 – Visualización en tablet horizontal.

# Mobile
TC-BUS-048 – Visualización en teléfonos pequeños.
TC-BUS-049 – Visualización en teléfonos grandes.
TC-BUS-050 – Cambio entre orientación vertical y horizontal.

# General
TC-BUS-051 – Verificar adaptación de imágenes.
TC-BUS-052 – Verificar adaptación del texto.
TC-BUS-053 – Verificar tamaño de botones.
TC-BUS-054 – Verificar márgenes.
TC-BUS-055 – Verificar espaciado entre componentes.
TC-BUS-056 – Verificar ausencia de scroll horizontal.
TC-BUS-057 – Verificar que ningún contenido quede oculto.


## Accessibility Testing

# Navegación
TC-BUS-058 – Navegación mediante teclado.
TC-BUS-059 – Orden correcto del foco.
TC-BUS-060 – Indicador visual del foco.

# Lectores de Pantalla
TC-BUS-061 – Lectura correcta de títulos.
TC-BUS-062 – Lectura correcta de párrafos.
TC-BUS-063 – Lectura correcta de enlaces.

# Contraste
TC-BUS-064 – Validar contraste entre texto y fondo.
TC-BUS-065 – Validar contraste de botones.
TC-BUS-066 – Validar contraste de enlaces.

# Multimedia
TC-BUS-067 – Verificar texto alternativo de imágenes.
TC-BUS-068 – Verificar accesibilidad de íconos.