# Test Case Template

Este documento define el formato estándar utilizado para documentar todos los casos de prueba del proyecto Cineflix.

Todos los casos de prueba deberán seguir esta estructura para garantizar consistencia, trazabilidad y facilidad de mantenimiento.

---

# Estructura

## Test Case ID

TC-HOME-001

---

## Módulo

Home

---

## Categoría

- Functional

---

## Nombre del Caso

Acceder correctamente al home en mobile

---

## Objetivo

Verificar la carga inicial del home, permitiendo acceder sin problemas a la pagina principal que es la primera que ve el usuario

---

## Precondiciones

- Tener suficiente espacio de almacenamiento interno
- Usuario debe haber instalado previamente el apk de la aplicacion 

---

## Datos de prueba

N/A, no se requirieron datos para esta prueba en especifico

## Pasos

1. Instalar la aplicación.
2. Abrir aplicacion.
3. Hacer scroll.

---

## Resultado esperado

El sistema muestra correctamente la carga inicial del home sin problema

---

## Resultado obtenido

Al abrir la aplicacion muestra correctamente la pantalla inicial

---

## Estado

- Pass

---

## Prioridad

- Alta

---

## Severidad

- Alta

---

## Evidencia

/docs/evidence/mobile/home/TC-HOME-001/home-success1.jpg
/docs/evidence/mobile/home/TC-HOME-001/home-success2.jpg

---

## Observaciones

Al realizar la prueba inicial tanto de manera local como en produccion se observa un correcto renderizado, se puede acceder sin problema y muestra correctamente el home, sin entrar en detalles de componentes especificos del home los cuales seran contemplados en los proximos casos de pruebas. Se deja evidencia de la correcta actualizacion de la cartelera al añadir nuevas funciones
