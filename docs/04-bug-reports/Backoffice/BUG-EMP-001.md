# Bug ID

BUG-EMP-001

---

## Título

No se muestra notificación de éxito/error al registrar un empleado.

---

## Módulo

Employees (Backoffice)

---

## Tipo

UX

---

## Prioridad

Media

---

## Severidad

Media

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

- Usuario autenticado con permisos de empleados.
- Formulario "Añadir Empleado" abierto.

---

## Pasos para reproducir

1. Acceder a `/admin/personal` > pestaña "Empleados".
2. Clic en "Añadir Empleado".
3. Completar todos los campos obligatorios correctamente.
4. Clic en "Registrar".

---

## Resultado esperado

Aparece un toast o mensaje confirmando "Empleado registrado exitosamente".

---

## Resultado obtenido

El modal se cierra sin mostrar ningún mensaje de confirmación ni de error. El usuario no sabe si la operación fue exitosa hasta que refresca la lista.

---

## Frecuencia

Siempre

---

## Evidencia

/docs/07-evidence/backoffice/employees/BUG-EMP-001/

---

## Estado

Closed (Corregido)

---

## Responsable

Frontend

---

## Observaciones

Corregido en `personalPage.jsx`. Se agregó `refreshKey` state y se pasó `key={refreshKey}` al componente `Employees`. Al cerrar el modal con `shouldRefresh=true`, se incrementa `refreshKey` forzando remount y refresco de lista.
