# TC-BUS-010 – Verificar que la pantalla cargue sin errores visuales

## Test Case ID

TC-BUS-010

---

## Módulo

Business

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar que la pantalla cargue sin errores visuales

---

## Objetivo

Verificar que al acceder a /business la página cargue completamente sin pantalla blanca, sin parpadeos, sin errores de consola visibles y sin elementos rotos. El fondo púrpura oscuro (#231640) debe renderizarse correctamente.

---

## Precondiciones

- Navegador web actualizado.
- Conexión a internet disponible.
- URL /business accesible.

---

## Datos de prueba

- Ruta: /business
- Fondo esperado: #231640 (púrpura oscuro)
- Dispositivo: Desktop (1920x1080)

---

## Pasos

1. Abrir el navegador y navegar a /business.
2. Observar la carga de la página durante 3 segundos.
3. Verificar que no aparezca pantalla blanca durante la carga.
4. Verificar que el fondo de la página sea el color púrpura oscuro correcto (#231640).
5. Abrir la consola del navegador (F12) y verificar que no existan errores críticos en consola relacionados con la renderización.
6. Verificar que el Header se muestre correctamente con fondo #2A154B.
7. Verificar que el contenido principal cargue sin elementos rotos.

---

## Resultado esperado

La página carga sin pantalla blanca, sin parpadeos y sin errores visibles. El fondo púrpura oscuro (#231640) se aplica correctamente. El Header se muestra con su fondo #2A154B. No aparecen errores críticos en la consola del navegador relacionados con la renderización de la página.

---

## Resultado obtenido

Cumple con la descripcion dada en el resultado esperado.

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

- screenshot-01
---

## Observaciones

- Ninguna
