# Test Case Template

Este documento define el formato estándar utilizado para documentar todos los casos de prueba del proyecto Cineflix.

Todos los casos de prueba deberán seguir esta estructura para garantizar consistencia, trazabilidad y facilidad de mantenimiento.

---

# Estructura

## Test Case ID

TC-HOME-005

---

## Módulo

Home

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar carga del Home con usuario autenticado.

---

## Objetivo

Verificar la carga inicial del home cuando el usuario ha iniciado sesion

---

## Precondiciones

- Tener instalada la aplicacion
- El usuario debe estar registrado en la plataforma 

---

## Datos de prueba

correo: jenniferamirez2211@gmail.com
contraseña: xxxxxxxxxxx

## Pasos

1. Instalar la aplicación.
2. Abrir aplicacion.
3. Presionar boton de Ingresar
4. Iniciar sesion
5. Navegar hasta el home

---

## Resultado esperado

El sistema carga correctamente el home que conforman el home una vez que el usuario ha iniciado sesion

---

## Resultado obtenido

Al autenticarse y navegar desde el login hasta el home se cargan correctamente cada uno de los componentes 

---

## Estado

- Pass

---

## Prioridad

- Media

---

## Severidad

- Media

---

## Evidencia

/docs/evidence/mobile/home/TC-HOME-005/home-logged.jpg

---

## Observaciones

Se observo un correcto renderizado en la visualizacion del home cuando el usuario se encuentra autenticado
