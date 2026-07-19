# Test Case ID

TC-EMP-001

---

## Módulo

Employees (Backoffice)

---

## Categoría

Functional

---

## Nombre del Caso

Registrar un empleado con todos los campos obligatorios correctamente.

---

## Objetivo

Verificar que el sistema permita registrar un nuevo empleado completando todos los campos obligatorios.

---

## Precondiciones

- Usuario autenticado como SUPER_ADMIN o Gerente General.
- Módulo Personal accesible desde el menú.

---

## Datos de prueba

| Campo | Valor |
|-------|-------|
| Cédula | V-22333444 |
| Nombre | Roberto |
| Apellido | Castillo |
| Cargo | Cajero |
| Sucursal | Sambil Barquisimeto |
| Fecha de inicio | 15/07/2026 |
| Salario base | 250.00 |
| Correo | roberto@cineflix.com |
| Contraseña | Test1234* |
| Rol | Cajero |

---

## Pasos

1. Acceder al Backoffice e iniciar sesión.
2. Navegar a `/admin/personal` desde el menú "Empleados".
3. Seleccionar la pestaña "Empleados".
4. Hacer clic en "Añadir Empleado".
5. Completar todos los campos con los datos de prueba.
6. Hacer clic en "Registrar".

---

## Resultado esperado

El empleado se registra exitosamente. Aparece en el listado de empleados activos con sus datos correctos.

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

Crítica

---

## Evidencia

/docs/07-evidence/backoffice/employees/TC-EMP-001/

---

## Observaciones

Versión 1.0 — 13/07/2026
