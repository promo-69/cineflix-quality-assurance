# Test Case ID

TC-CPOS-006

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Validar teléfono.

---

## Objetivo

Verificar que el sistema valide el formato del número de teléfono al registrar un nuevo cliente.

---

## Precondiciones

- Usuario autenticado.
- Cliente no existente.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-11111114 |
| Nombre | Ana |
| Apellido | Ruiz |
| Teléfono | abcdefgh |

---

## Pasos

1. Buscar cédula no existente.
2. Completar formulario con un teléfono en formato inválido (letras).
3. Hacer clic en "Registrar y Continuar".

---

## Resultado esperado

Mensaje de error indicando que el formato del teléfono no es válido (solo números, máximo 11 dígitos).

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

/docs/07-evidence/backoffice/candystore/TC-CPOS-006/

---

## Observaciones

Versión 1.0 — 13/07/2026
