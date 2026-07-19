# Test Case ID

TC-CPOS-009

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Buscar cliente por cédula.

---

## Objetivo

Verificar que el sistema permita buscar un cliente existente por su número de cédula y lo recupere correctamente.

---

## Precondiciones

- Cliente previamente registrado (ej. V-12345678 Carlos Pérez).
- Usuario autenticado.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-12345678 |

---

## Pasos

1. Acceder al módulo Candy Store.
2. Ingresar cédula V-12345678.
3. Hacer clic en "Buscar".

---

## Resultado esperado

El sistema encuentra al cliente y muestra sus datos: nombre, cédula, nivel de lealtad y puntos.

---

## Resultado obtenido

El sistema encontró al cliente V-12345678 (Carlos Pérez) y mostró sus datos correctamente: nombre, cédula y puntos de fidelidad.

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-009/

---

## Observaciones

El cliente V-12345678 fue registrado en TC-CPOS-001.
