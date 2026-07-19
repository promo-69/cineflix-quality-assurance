# Test Case ID

TC-CPOS-001

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Registrar un cliente nuevo antes de iniciar la compra.

---

## Objetivo

Verificar que el sistema permita registrar correctamente a un nuevo cliente desde el módulo de Candy Store antes de iniciar una venta.

---

## Precondiciones

- Usuario autenticado con rol Cajero o superior.
- Servidor disponible.
- Módulo Candy Store accesible desde el menú principal.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-12345678 |
| Nombre | Carlos |
| Apellido | Pérez |
| Teléfono | 04141234567 |
| Correo | carlos@test.com |

---

## Pasos

1. Acceder al Backoffice e iniciar sesión.
2. Navegar al módulo Candy Store desde el menú lateral.
3. En el paso "Identificar Cliente", ingresar la cédula V-12345678 en el campo de búsqueda.
4. Al no encontrar al cliente, hacer clic en "Registrar".
5. Completar los campos obligatorios (Nombre, Apellido, Teléfono, Correo).
6. Hacer clic en "Registrar y Continuar".

---

## Resultado esperado

El sistema registra al nuevo cliente, lo asocia a la sesión de compra activa y avanza al catálogo de productos.

---

## Resultado obtenido

El sistema registró al cliente correctamente. Mostró los datos del cliente (nombre, cédula, puntos) y avanzó al catálogo de productos sin errores.

---

## Estado

Pass

---

## Prioridad

Alta

---

## Severidad

Crítica

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-001/

---

## Observaciones

Versión 1.0 — 13/07/2026
