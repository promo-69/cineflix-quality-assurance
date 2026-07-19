# Test Case ID

TC-CPOS-012

---

## Módulo

CandyStore (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Mostrar mensaje cuando el cliente no exista.

---

## Objetivo

Verificar que el sistema muestre un mensaje claro al buscar una cédula no registrada y ofrezca la opción de registrar un nuevo cliente.

---

## Precondiciones

- Usuario autenticado.
- La cédula a buscar no está registrada en el sistema.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-99999999 |

---

## Pasos

1. Acceder al módulo Candy Store.
2. Ingresar la cédula V-99999999.
3. Hacer clic en "Buscar".

---

## Resultado esperado

El sistema muestra el mensaje "Cliente no encontrado" y despliega el formulario de registro con los campos obligatorios.

---

## Resultado obtenido

El sistema mostró correctamente el formulario de registro con los campos obligatorios (Nombre, Apellido, Teléfono, Correo) al no encontrar la cédula V-99999999.

---

## Estado

Pass

---

## Prioridad

Media

---

## Severidad

Baja

---

## Evidencia

/docs/07-evidence/backoffice/candystore/TC-CPOS-012/

---

## Observaciones

Versión 1.0 — 13/07/2026
