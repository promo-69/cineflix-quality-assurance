# PurchaseHistory - Manual Test Cases

## Información General

Módulo: PurchaseHistory
Componente: Frontend App Mobile
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---
## Objetivo

Validar el correcto funcionamiento del módulo Purchase History, permitiendo al cliente consultar todas las compras realizadas dentro de Cineflix, visualizando información detallada de cada transacción, incluyendo boletos adquiridos, productos de confitería asociados, información de la función, código QR generado, fecha de compra y puntos de fidelización obtenidos.

Además, se busca garantizar que la información mostrada corresponda exactamente con la orden procesada durante el flujo de compra, manteniendo consistencia entre los módulos de Payment y Loyalty.

---

# Alcance

Las pruebas documentadas para este módulo comprenden la validación de:

- Acceso al historial de compras.
- Visualización de compras realizadas.
- Visualización del detalle de una compra.
- Información de tickets.
- Información de confitería.
- Visualización del QR.
- Validación del estado de compra.
- Información de puntos obtenidos.
- Integración con backend.
- Manejo de compras sin historial.
- Responsive.
- Accesibilidad.

No forman parte del alcance:

- Modificación de compras.
- Cancelación de compras.
- Reembolso.
- Administración del historial.


## Functional Testing

# Acceso al módulo
TC-PH-001 – Acceder correctamente a Purchase History desde el perfil del usuario.
TC-PH-002 – Verificar que solamente usuarios autenticados puedan acceder.
TC-PH-003 – Mantener sesión activa al ingresar.
TC-PH-004 – Cargar correctamente la información del usuario.

# Visualización del historial
TC-PH-006 – Mostrar todas las compras realizadas.
TC-PH-007 – Mostrar compras ordenadas por fecha descendente.
TC-PH-008 – Mostrar la compra más reciente primero.
TC-PH-009 – Mostrar múltiples compras correctamente.
TC-PH-010 – Mostrar historial vacío cuando no existen compras.
TC-PH-011 – Mostrar mensaje informativo sin compras.
TC-PH-012 – Mostrar correctamente el estado de cada compra.

# Información general de compra
TC-PH-013 – Mostrar número de orden.
TC-PH-014 – Mostrar fecha de compra.
TC-PH-015 – Mostrar hora de compra.
TC-PH-016 – Mostrar estado de compra.
TC-PH-017 – Mostrar monto total.
TC-PH-018 – Mostrar moneda correctamente.
TC-PH-019 – Mostrar información consistente con Payment.

# Detalle de compra de boletos
TC-PH-020 – Acceder al detalle de una compra.
TC-PH-021 – Mostrar película adquirida.
TC-PH-022 – Mostrar poster de película.
TC-PH-023 – Mostrar sucursal.
TC-PH-024 – Mostrar sala.
TC-PH-025 – Mostrar fecha de función.
TC-PH-026 – Mostrar hora de función.
TC-PH-027 – Mostrar cantidad de boletos.
TC-PH-028 – Mostrar tipo de entradas adquiridas.

# Información de asientos
TC-PH-029 – Mostrar asientos adquiridos.
TC-PH-030 – Mostrar fila correctamente.
TC-PH-031 – Mostrar número de asiento.
TC-PH-032 – Mostrar múltiples asientos.
TC-PH-033 – Validar correspondencia con Seat Selection.

# Información de confitería
TC-PH-034 – Mostrar productos adquiridos.
TC-PH-035 – Mostrar cantidad comprada.
TC-PH-036 – Mostrar precio individual.
TC-PH-037 – Mostrar subtotal de productos.
TC-PH-038 – Mostrar fecha de retiro.
TC-PH-039 – Validar retiro únicamente el día indicado.
TC-PH-040 – Mostrar compra sin confitería correctamente.

## Código QR

# Visualización
TC-PH-041 – Mostrar QR asociado a la compra.
TC-PH-042 – Permitir visualizar QR.
TC-PH-043 – Mostrar QR solamente para compras completadas.
TC-PH-044 – Ocultar QR en compras fallidas.

# Validación QR
TC-PH-045 – Generar QR válido.
TC-PH-046 – Permitir escaneo del QR.
TC-PH-047 – Mostrar información correcta al escanear.
TC-PH-048 – Relacionar QR con la orden correcta.
TC-PH-049 – Validar que QR no pertenezca a otro usuario.
TC-PH-050 – Validar QR duplicado.
TC-PH-051 – Validar QR alterado.
TC-PH-052 – Validar QR expirado.

# Fidelización y CinePuntos
TC-PH-053 – Mostrar puntos obtenidos por compra.
TC-PH-054 – Mostrar puntos obtenidos por película.
TC-PH-055 – Mostrar puntos obtenidos por consumo de confitería.
TC-PH-056 – Validar acumulación después de compra.
TC-PH-057 – Comparar puntos con módulo Loyalty.
TC-PH-058 – Mostrar correctamente el nivel del usuario después de compra.

# Filtros y búsqueda
TC-PH-059 – Filtrar por fecha.
TC-PH-060 – Filtrar compras recientes.
TC-PH-061 – Limpiar filtros.
TC-PH-062 – Mostrar resultados correctos.

# Manejo de errores
TC-PH-069 – Mostrar error cuando backend no responde.
TC-PH-070 – Mostrar mensaje cuando falla carga.
TC-PH-071 – Permitir reintentar carga.
TC-PH-072 – Manejar sesión expirada.

# Descarga PDF
TC-PH-135 – Mostrar botón "Descargar comprobante PDF" en compras completadas.
TC-PH-136 – Ocultar botón en compras fallidas.
TC-PH-137 – Ocultar botón en compras canceladas.
TC-PH-138 – Descargar PDF asociado a la compra seleccionada.
TC-PH-139 – Validar que descargue el PDF correcto.
TC-PH-140 – Validar que una compra no pueda descargar el PDF de otra.
TC-PH-141 – Permitir descargar múltiples comprobantes.
TC-PH-142 – Mantener disponible el PDF aunque haya pasado tiempo desde la compra.
TC-PH-143 – Mostrar indicador de carga durante generación.
TC-PH-144 – Mostrar mensaje cuando la descarga falla.
TC-PH-145 – Permitir reintentar descarga.


## Information Testing
TC-PH-073 – Validar nombre de película.
TC-PH-074 – Validar sucursal.
TC-PH-075 – Validar sala.
TC-PH-076 – Validar fecha.
TC-PH-077 – Validar horario.
TC-PH-078 – Validar asientos.
TC-PH-079 – Validar tipos de entrada.
TC-PH-080 – Validar productos de confitería.
TC-PH-081 – Validar precios.
TC-PH-082 – Validar monedas.
TC-PH-083 – Validar número de orden.
TC-PH-084 – Validar puntos generados.
TC-PH-085 – Validar información del QR.
TC-PH-086 – Validar mensajes.
TC-PH-087 – Validar ortografía.

# Validación del PDF desde Purchase History
TC-PH-146 – Validar formato PDF.
TC-PH-147 – Validar apertura correcta.
TC-PH-148 – Validar contenido del documento.
TC-PH-149 – Validar información del cliente.
TC-PH-150 – Validar información de la compra.
TC-PH-151 – Validar productos de confitería.
TC-PH-152 – Validar tickets.
TC-PH-153 – Validar puntos generados.
TC-PH-154 – Validar QR incluido.
TC-PH-155 – Validar que el QR del PDF sea igual al mostrado en pantalla.
TC-PH-156 – Validar que el QR pueda escanearse desde el PDF.
TC-PH-157 – Validar existencia del botón descarga PDF.
TC-PH-158 – Validar texto del botón.
TC-PH-159 – Validar mensajes asociados a descarga.
TC-PH-160 – Validar nombre del archivo generado.

## Navigation Testing
TC-PH-088 – Abrir detalle de compra.
TC-PH-089 – Regresar al listado.
TC-PH-090 – Visualizar QR desde detalle.
TC-PH-091 – Navegar hacia Home.


## Integration Testing
TC-PH-095 – Obtener historial del usuario.
TC-PH-096 – Obtener detalles de compra.
TC-PH-097 – Obtener información del ticket.
TC-PH-098 – Obtener QR asociado.
TC-PH-099 – Obtener productos asociados.
TC-PH-100 – Obtener puntos generados.
TC-PH-101 – Integración con Payment.
TC-PH-102 – Integración con Loyalty.
TC-PH-103 – Integración con Ticket Generator.
TC-PH-104 – Integración con Candy Inventory.
TC-PH-105 – Respuesta HTTP 200.
TC-PH-106 – HTTP 400.
TC-PH-107 – HTTP 401.
TC-PH-108 – HTTP 403.
TC-PH-109 – HTTP 404.
TC-PH-110 – HTTP 500.
TC-PH-111 – Timeout.


## Accessibility Testing
TC-PH-113 – Orden correcto del foco.
TC-PH-114 – Lectura mediante lector de pantalla.
TC-PH-115 – Etiquetas accesibles.
TC-PH-116 – Descripción del QR accesible.
TC-PH-117 – Botones con nombres claros.
TC-PH-118 – Contraste adecuado.
TC-PH-119 – Escalado de texto.


## Responsive Testing

# Tablet
TC-PH-123 – Vista vertical.
TC-PH-124 – Vista horizontal.

# Mobile
TC-PH-125 – Pantallas pequeñas.
TC-PH-126 – Pantallas grandes.
TC-PH-127 – Cambio orientación.

# Componentes
TC-PH-128 – Adaptación tarjetas de compra.
TC-PH-129 – Adaptación detalle.
TC-PH-130 – Adaptación QR.
TC-PH-131 – Adaptación botones.
TC-PH-132 – Adaptación textos largos.
TC-PH-133 – Ausencia de scroll horizontal.
TC-PH-134 – Correcta interacción táctil.