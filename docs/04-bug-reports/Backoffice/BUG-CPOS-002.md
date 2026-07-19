# Bug ID

BUG-CPOS-002

---

## Título

El monto del pago en Candy Store no coincide con el total del carrito, mostrando "excede el total".

---

## Módulo

CandyStore (Backoffice)

---

## Tipo

Funcional

---

## Prioridad

Crítica

---

## Severidad

Crítica

---

## Ambiente

Testing (Desarrollo)

---

## Versión

v1.0

---

## Reportado por

Alexis

---

## Fecha

13/07/2026

---

## Precondiciones

- Cliente identificado.
- Productos en el carrito con total > $0.
- Sesión de compra activa.

---

## Pasos para reproducir

1. Agregar productos al carrito en Candy Store.
2. Hacer clic en "PROCESAR PAGO".
3. Observar el mensaje de validación y el botón "Confirmar Venta".

---

## Resultado esperado

El monto del pago coincide exactamente con el total del carrito. El botón "Confirmar Venta" está habilitado.

---

## Resultado obtenido

El sistema mostraba "Los montos exceden el total por $X.XX" y el botón permanecía deshabilitado, a pesar de que el monto era correcto. Causa: el campo `amount` en el payload de pago era `undefined` (se usaba `p.amount` en vez de `p.amountVes`). Adicionalmente, la tolerancia de balance era muy estricta (0.01) y los cálculos VES/USD introducían errores de redondeo.

---

## Frecuencia

Siempre

---

## Evidencia

/docs/07-evidence/backoffice/candystore/BUG-CPOS-002/

---

## Estado

Closed (Corregido)

---

## Responsable

Frontend

---

## Observaciones

Correcciones aplicadas:
1. `candyBar.jsx handleConfirm`: `p.amount` → `p.amountVes` (mismo campo que sellTickets)
2. `Step4Payment.jsx`: tolerancia de balance de 0.01 → 1.0
3. Moneda unificada a `vesCurrencyId` como en sellTickets
4. `key={payment-${cartTotal}}` fuerza remount con valores frescos
