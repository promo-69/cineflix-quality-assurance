# Test Case Template

Este documento define el formato estándar utilizado para documentar todos los casos de prueba del proyecto Cineflix.

Todos los casos de prueba deberán seguir esta estructura para garantizar consistencia, trazabilidad y facilidad de mantenimiento.

---

# Estructura

## Test Case ID

TC-HOME-002

---

## Módulo

Home

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar carga completa de todos los componentes

---

## Objetivo

Verificar la carga inicial de cada uno de los componentes que comprende el home en la aplicacion movil

---

## Precondiciones

- Tener instalada la aplicacion movil 

---

## Datos de prueba

N/A, no se requirieron datos para esta prueba en específico

## Pasos

1. Instalar la aplicación.
2. Abrir aplicacion.
3. Visualizar que se muestre seccion cartelera
4. Visualizar que se muestre seccion Proximos estrenos
5. Visualizar que se muestre seccion Eventos
6. Visualizar que se muestra menu de navegacion
7. Visualizar que se muestre seccion de recomendaciones

---

## Resultado esperado

El sistema carga correctamente cada uno de los componentes que conforman el home en la aplicacion movil

---

## Resultado obtenido

Al abrir la aplicacion carga correctamente el home constituido por las secciones: En Cartelera, Proximos estrenos, Eventos, boton de iniciar sesion y menu de navegacion inferior, no se observo o no esta contemplado la seccion de recomendaciones y anuncios publicitarios en el home como componente 

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

/docs/evidence/mobile/home/TC-HOME-002/home-success-vd.mp4

---

## Observaciones

Al realizar la prueba inicial tanto de manera local como en produccion se observa que se ejecuta correctamente la carga completa de cada uno de los componentes, el unico componente que no se comtemplo en este home es la seccion de recomendaciones cuando el usuario no esta logueado
