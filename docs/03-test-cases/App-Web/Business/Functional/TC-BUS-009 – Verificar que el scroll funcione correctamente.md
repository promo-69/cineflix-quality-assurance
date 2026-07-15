# TC-BUS-009 – Verificar que el scroll funcione correctamente

## Test Case ID

TC-BUS-009

---

## Módulo

Business

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar que el scroll funcione correctamente

---

## Objetivo

Verificar que el scroll vertical funcione correctamente en las pestañas con contenido extenso ("Sobre Nosotros" y "Términos y Condiciones"), permitiendo al usuario desplazarse por todo el contenido sin perderse información.

---

## Precondiciones

- Navegador web actualizado.
- Conexión a internet disponible.
- URL /business accesible.
- La pantalla debe ser suficientemente pequeña para que el contenido exceda la altura visible (o usar devtools con viewport reducido).

---

## Datos de prueba

- Ruta: /business
- Dispositivo: Desktop (1920x1080)
- Pestañas con scroll extenso: Sobre Nosotros, Términos y Condiciones

---

## Pasos

1. Abrir el navegador y navegar a /business.
2. Verificar que la pestaña "Sobre Nosotros" esté activa.
3. Desplazarse hacia abajo usando la rueda del mouse o barra de scroll.
4. Verificar que el scroll llega hasta la imagen final "Cineflix Popcorn" y al Footer/Pie de página.
5. Desplazarse hacia arriba y verificar que se puede regresar al inicio.
6. Hacer clic en "Términos y Condiciones".
7. Desplazarse hacia abajo hasta la cláusula SÉPTIMA.
8. Verificar que el scroll permite llegar al final del contenido de Términos y Condiciones.
9. Hacer clic en "Marketing Empresarial".
10. Verificar que el contenido de Marketing Empresarial es visible sin necesidad de scroll (contenido corto).

---

## Resultado esperado

El scroll vertical funciona correctamente en las pestañas con contenido extenso. El usuario puede desplazarse desde el inicio hasta el final del contenido y viceversa. El Header/Cabecera se mantiene visible (sticky) mientras se hace scroll. La pestaña "Marketing Empresarial" no requiere scroll por su contenido breve.

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

---

## Observaciones

- Ninguna