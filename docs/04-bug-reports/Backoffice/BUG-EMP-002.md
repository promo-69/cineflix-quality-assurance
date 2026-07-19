# Bug ID

BUG-EMP-002

---

## Título

La lista de empleados no se actualiza automáticamente al registrar uno nuevo.

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

- Usuario en la lista de empleados.
- Se acaba de registrar un nuevo empleado exitosamente.

---

## Pasos para reproducir

1. Acceder a `/admin/personal` > pestaña "Empleados".
2. Clic en "Añadir Empleado".
3. Registrar un nuevo empleado con datos válidos.
4. Al cerrar el modal, observar la lista.

---

## Resultado esperado

El nuevo empleado aparece inmediatamente en la lista sin necesidad de refrescar.

---

## Resultado obtenido

La lista no se actualiza. Es necesario refrescar la página (F5) para ver el nuevo empleado.

---

## Frecuencia

Siempre

---

## Evidencia

/docs/07-evidence/backoffice/employees/BUG-EMP-002/

---

## Estado

Closed (Corregido)

---

## Responsable

Frontend

---

## Observaciones

Corregido en `personalPage.jsx`. El modal de "Añadir Empleado" estaba en el padre (`personalPage.jsx`) con `onClose={closeModal}` que no refrescaba. Ahora al cerrar con `shouldRefresh=true` se incrementa `refreshKey` forzando remount del componente `Employees`.
