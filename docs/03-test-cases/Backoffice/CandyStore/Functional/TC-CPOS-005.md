# Test Case ID

TC-CPOS-005

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar correo electrónico.

---

## Objetivo

Verificar que el sistema valide el formato del correo electrónico al registrar un nuevo cliente.

---

## Precondiciones

- Usuario autenticado.
- Cliente no existente.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-11111113 |
| Nombre | María |
| Apellido | Gómez |
| Correo | correo-invalido |

---

## Pasos

1. Buscar cédula no existente.
2. Completar formulario con un correo en formato inválido.
3. Hacer clic en "Registrar y Continuar".

---

## Resultado esperado

Mensaje de error indicando que el formato del correo no es válido.

---

## Resultado obtenido

Pendiente

---

## Estado

Not Executed

---

## Prioridad

Media

---

## Severidad

Media

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-005/

---

## Observaciones

Versión 1.0 — 13/07/2026
