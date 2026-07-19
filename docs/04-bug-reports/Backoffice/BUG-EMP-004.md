# Bug ID

BUG-EMP-004

---

## Título

Al editar un empleado, el campo de sucursal no muestra la sucursal actualmente asignada.

---

## Módulo

Employees (Backoffice)

---

## Tipo

Funcional

---

## Prioridad

Alta

---

## Severidad

Alta

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

15/07/2026

---

## Precondiciones

- Empleado registrado con sucursal asignada (Andrés Mendoza → Sambil Barquisimeto).

---

## Pasos para reproducir

1. Ir a lista de empleados.
2. Clic en el ícono de lápiz (editar) de un empleado.
3. Observar el campo "Sucursal".

---

## Resultado esperado

La sucursal actual del empleado aparece preseleccionada en el dropdown.

---

## Resultado obtenido

El campo sucursal aparece sin selección (vacío). Los demás campos (cargo, salario, fecha inicio) sí se cargan correctamente.

---

## Frecuencia

Siempre

---

## Estado

Closed (Corregido)

---

## Responsable

Frontend

---

## Observaciones

## Observaciones

Dos problemas corregidos en `EditEmployeeModal.jsx`:
1. `getCinemas` devuelve `{ rows: [...] }`, no un array. Cambiado a `data?.data?.rows ?? data?.data ?? []`.
2. `employee.cinema` venía como número pero el select value espera string. Agregado `String()` en la carga del formulario.

También corregido mismo bug en `RegisterEmployeeModal.jsx`.
