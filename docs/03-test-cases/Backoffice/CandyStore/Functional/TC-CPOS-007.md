# Test Case ID

TC-CPOS-007

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Registrar correctamente al cliente.

---

## Objetivo

Verificar que el sistema registre correctamente al cliente con todos los campos completos y muestre confirmación.

---

## Precondiciones

- Usuario autenticado.
- Cliente no existente.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-11111115 |
| Nombre | Pedro |
| Apellido | Sánchez |
| Teléfono | 04141112233 |
| Correo | pedro@test.com |
| Género | Masculino |

---

## Pasos

1. Buscar cédula no existente.
2. Completar todos los campos del formulario con datos válidos.
3. Hacer clic en "Registrar y Continuar".

---

## Resultado esperado

El sistema registra al cliente exitosamente. Muestra los datos del cliente y avanza al catálogo de productos.

---

## Resultado obtenido

Cliente registrado exitosamente con todos los campos. Los datos se muestran correctamente en el card de confirmación. Avanza al catálogo de productos.

---

## Estado

Pass

---

## Prioridad

Alta

---

## Severidad

Alta

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-007/

---

## Observaciones

Versión 1.0 — 13/07/2026
