# Candy Store - Manual Test Cases

## Información General

Módulo: Candy Store
Componente: Frontend Web
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Candy Store, verificando que los usuarios puedan consultar el catálogo de productos de confitería disponible por sucursal, visualizar la información de cada producto y agregar artículos al proceso de compra de forma correcta.

Las pruebas contemplan la visualización del catálogo, el filtrado por sucursal, la disponibilidad de productos, las restricciones de autenticación, la navegación hacia el flujo de compra y la correcta experiencia de usuario en dispositivos móviles y de escritorio.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Consulta del catálogo de confitería.
- Filtrado de productos por sucursal.
- Disponibilidad de productos.
- Visualización de información.
- Navegación hacia el flujo de compra.
- Restricciones de autenticación.
- Gestión del carrito de confitería.
- Responsive Design.
- Accesibilidad.
- Integración con Backend.

No forman parte del alcance:

- Procesamiento de pagos.
- Confirmación de compra.
- Emisión de comprobantes.
- Generación de boletos.
- Validación de métodos de pago.


## Functional Testing
# Acceso al módulo
TC-CAN-001 – Acceder correctamente al módulo Candy Store.
TC-CAN-002 – Verificar que el catálogo cargue correctamente.
TC-CAN-003 – Verificar que la pantalla no presente errores durante la carga.
TC-CAN-004 – Verificar comportamiento cuando no existen productos registrados.
TC-CAN-005 – Verificar comportamiento cuando la API responde correctamente.

# Consulta del catálogo
TC-CAN-006 – Visualizar todos los productos disponibles.
TC-CAN-007 – Verificar que cada producto muestre su imagen.
TC-CAN-008 – Verificar nombre del producto.
TC-CAN-009 – Verificar precio.
TC-CAN-010 – Verificar disponibilidad.
TC-CAN-011 – Verificar categoría del producto.
TC-CAN-012 – Verificar descripción del producto.
TC-CAN-013 – Verificar orden correcto del catálogo.

# Filtrado por sucursal
TC-CAN-014 – Seleccionar una sucursal correctamente.
TC-CAN-015 – Mostrar únicamente productos disponibles para la sucursal seleccionada.
TC-CAN-016 – Cambiar de sucursal.
TC-CAN-017 – Actualizar automáticamente el catálogo al cambiar la sucursal.
TC-CAN-018 – Mantener la sucursal seleccionada durante la navegación.
TC-CAN-019 – Verificar comportamiento cuando una sucursal no posee productos.
TC-CAN-020 – Verificar comportamiento cuando la sucursal deja de estar disponible.

# Filtrado por categoría
TC-CAN-021 – Mostrar únicamente Combos.
TC-CAN-022 – Mostrar únicamente Cotufas.
TC-CAN-023 – Mostrar únicamente Bebidas.
TC-CAN-024 – Mostrar únicamente Dulces.
TC-CAN-025 – Mostrar únicamente Snacks.
TC-CAN-026 – Cambiar entre categorías.
TC-CAN-027 – Mostrar todos los productos nuevamente.
TC-CAN-028 – Mantener la categoría seleccionada después de cambiar de sucursal.

# Visualización del producto
TC-CAN-029 – Visualizar imagen correctamente.
TC-CAN-030 – Imagen inexistente.
TC-CAN-031 – Imagen dañada.
TC-CAN-032 – Precio correctamente formateado.
TC-CAN-033 – Producto sin imagen.
TC-CAN-034 – Nombre muy largo.
TC-CAN-035 – Descripción muy extensa.
TC-CAN-036 – Producto agotado.

# Agregar productos
TC-CAN-037 – Agregar un producto al carrito.
TC-CAN-038 – Agregar múltiples unidades del mismo producto.
TC-CAN-039 – Agregar diferentes productos.
TC-CAN-040 – Incrementar cantidad.
TC-CAN-041 – Disminuir cantidad.
TC-CAN-042 – Eliminar un producto del carrito.
TC-CAN-043 – Vaciar completamente el carrito.
TC-CAN-044 – Verificar actualización automática del subtotal.
TC-CAN-045 – Verificar actualización del contador del carrito.

# Restricciones de autenticación
TC-CAN-046 – Intentar agregar productos sin iniciar sesión.
TC-CAN-047 – Mostrar mensaje indicando que debe iniciar sesión.
TC-CAN-048 – Redireccionar al Login desde el mensaje de autenticación.
TC-CAN-049 – Regresar correctamente al módulo después del Login.
TC-CAN-050 – Mantener el producto seleccionado después de autenticarse.

# Compra de confitería
TC-CAN-051 – Iniciar compra únicamente de productos de confitería.
TC-CAN-052 – Verificar navegación hacia el flujo de compra.
TC-CAN-053 – Verificar navegación hacia la compra mixta (boletos + confitería).
TC-CAN-054 – Verificar que el botón "Compra Mixta" esté disponible.
TC-CAN-055 – Verificar que el carrito conserve los productos seleccionados al cambiar al flujo de compra mixta.
TC-CAN-056 – Verificar que el usuario pueda continuar comprando boletos después de agregar productos de confitería.


## Information Testing
TC-CAN-057 – Validar nombres de productos.
TC-CAN-058 – Validar precios.
TC-CAN-059 – Validar formato monetario.
TC-CAN-060 – Validar ortografía.
TC-CAN-061 – Validar descripción.
TC-CAN-062 – Validar disponibilidad.
TC-CAN-063 – Validar nombres de categorías.
TC-CAN-064 – Validar mensajes de error.
TC-CAN-065 – Validar mensajes de éxito.
TC-CAN-066 – Validar información de la sucursal seleccionada.

## Navigation Testing
TC-CAN-067 – Acceder desde el menú principal.
TC-CAN-068 – Cambiar entre categorías.
TC-CAN-069 – Cambiar entre sucursales.
TC-CAN-070 – Navegar al Login cuando no existe autenticación.
TC-CAN-071 – Regresar desde Login.
TC-CAN-072 – Navegar hacia Compra Mixta.
TC-CAN-073 – Regresar desde Compra Mixta.
TC-CAN-074 – Mantener filtros durante la navegación.

## Integration Testing
TC-CAN-075 – Obtener catálogo correctamente desde Backend.
TC-CAN-076 – Obtener productos por sucursal.
TC-CAN-077 – Obtener categorías.
TC-CAN-078 – API responde HTTP 200.
TC-CAN-079 – API responde HTTP 404.
TC-CAN-080 – API responde HTTP 500.
TC-CAN-081 – Timeout del servidor.
TC-CAN-082 – Catálogo vacío.
TC-CAN-083 – Producto eliminado durante la consulta.
TC-CAN-084 – Producto agotado mientras el usuario navega.
TC-CAN-085 – Error al agregar un producto al carrito.
TC-CAN-086 – Error de autenticación (401).
TC-CAN-087 – Token expirado durante la operación.

## Accessibility Testing
TC-CAN-088 – Navegación mediante teclado.
TC-CAN-089 – Orden del foco.
TC-CAN-090 – Contraste adecuado.
TC-CAN-091 – Lectura mediante lector de pantalla.
TC-CAN-092 – Texto alternativo en imágenes.
TC-CAN-093 – Etiquetas accesibles para botones.
TC-CAN-094 – Tamaño adecuado de botones táctiles.
TC-CAN-095 – Escalado del texto al 200%.
TC-CAN-096 – Navegación sin utilizar mouse.

## Responsive Testing
TC-CAN-097 – Visualización Desktop.
TC-CAN-098 – Visualización Laptop.
TC-CAN-099 – Visualización Tablet.
TC-CAN-100 – Visualización Mobile.
TC-CAN-101 – Cambio entre orientación vertical y horizontal.
TC-CAN-102 – Adaptación de tarjetas de productos.
TC-CAN-103 – Adaptación del selector de sucursales.
TC-CAN-104 – Adaptación del filtro por categorías.
TC-CAN-105 – Verificar ausencia de scroll horizontal.
TC-CAN-106 – Correcta visualización del carrito en dispositivos móviles.

## UI / UX Testing
TC-CAN-107 – Consistencia de colores institucionales.
TC-CAN-108 – Consistencia tipográfica.
TC-CAN-109 – Correcta alineación de tarjetas.
TC-CAN-110 – Espaciado uniforme entre productos.
TC-CAN-111 – Indicadores visuales al agregar productos.
TC-CAN-112 – Feedback visual durante la carga del catálogo.
TC-CAN-113 – Indicador visual para productos agotados.
TC-CAN-114 – Claridad de los mensajes mostrados al usuario.
TC-CAN-115 – Fluidez del recorrido hacia el proceso de compra.