# Test Case ID

TC-CPOS-043

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Pago en efectivo (Bolívares).

---

## Objetivo

Verificar que el sistema procese correctamente un pago en efectivo en bolívares desde el módulo Candy Store.

---

## Precondiciones

- Cliente identificado.
- Productos agregados al carrito.
- Sesión de compra activa.

---

## Datos de prueba

Producto: Refresco Mediano ($2.50). Método: Efectivo.

---

## Pasos

1. Agregar productos al carrito.
2. Hacer clic en "PROCESAR PAGO".
3. Seleccionar método "Efectivo" (o mantener el default).
4. Verificar que el monto coincida con el total del carrito.
5. Ingresar número de referencia (ej: 1234567890).
6. Hacer clic en "Confirmar Venta".

---

## Resultado esperado

El sistema muestra "Procesando Pago" y luego el evento `payment_completed` confirma la venta exitosa. El carrito se limpia.

---

## Resultado obtenido

El pago se procesó correctamente. Se mostró el spinner "Procesando Pago", luego la pantalla de "¡Venta Exitosa!" vía WebSocket. El monto coincidió exactamente con el total.

---

## Estado

Pass

---

## Prioridad

Crítica

---

## Severidad

Crítica

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-043/

---

## Observaciones

Se corrigió bug donde el monto del pago no coincidía con el total (BUG-CPOS-002). El pago ahora usa el mismo flujo que venta de boletos: `amountVes` + `vesCurrencyId` + `bypass`. Versión 1.0 — 13/07/2026.
