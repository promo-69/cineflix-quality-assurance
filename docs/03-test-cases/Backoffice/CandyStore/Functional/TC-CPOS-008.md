# Test Case ID

TC-CPOS-008

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Asociar automáticamente la compra al nuevo cliente.

---

## Objetivo

Verificar que al registrar un nuevo cliente, la sesión de compra quede asociada correctamente a ese cliente.

---

## Precondiciones

- Usuario autenticado.
- Cliente no existente.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-11111116 |
| Nombre | Laura |
| Apellido | Díaz |

---

## Pasos

1. Buscar y registrar un nuevo cliente.
2. Agregar un producto al carrito.
3. Avanzar al pago.
4. Verificar en el resumen de venta que el cliente asociado sea el recién registrado.

---

## Resultado esperado

La compra queda asociada al cliente recién registrado. El nombre del cliente aparece en el resumen de venta.

---

## Resultado obtenido

Pendiente

---

## Estado

Not Executed

---

## Prioridad

Alta

---

## Severidad

Media

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-008/

---

## Observaciones

Versión 1.0 — 13/07/2026
