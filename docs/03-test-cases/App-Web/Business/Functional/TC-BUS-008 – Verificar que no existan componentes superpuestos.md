# TC-BUS-008 – Verificar que no existan componentes superpuestos

## Test Case ID

TC-BUS-008

---

## Módulo

Business

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar que no existan componentes superpuestos

---

## Objetivo

Verificar que no exista superposición de texto sobre imágenes, de un componente sobre otro, ni del Header/Footer sobre el contenido principal en ninguna de las pestañas del módulo Business/Empresa.

---

## Precondiciones

- Navegador web actualizado.
- Conexión a internet disponible.
- URL /business accesible.

---

## Datos de prueba

- Ruta: /business
- Dispositivo: Desktop (1920x1080)
- Pestañas a revisar: Sobre Nosotros, Marketing Empresarial, Términos y Condiciones

---

## Pasos

1. Abrir el navegador y navegar a /business.
2. Verificar que el Header/Cabecera no se superponga sobre el contenido de la página al hacer scroll.
3. Verificar que la imagen "Experiencia Cineflix" no se superponga con los párrafos adyacentes.
4. Verificar que las tarjetas de beneficios no se superpongan entre sí.
5. Hacer clic en "Marketing Empresarial" y verificar que el contenido no tenga superposiciones.
6. Hacer clic en "Términos y Condiciones" y verificar que las cláusulas no se superpongan.
7. Verificar que el Footer/Pie de página no se superponga con el contenido de la tab activa.

---

## Resultado esperado

Ningún componente visual se superpone con otro. Las imágenes están contenidas dentro de sus bordes, el texto no se solapa con imágenes adyacentes, las tarjetas mantienen su espacio y el Header/Footer no interfieren con el contenido principal.

---

## Resultado obtenido

Cumple con la descripción dada en el resultado esperado.

---

## Estado

- Pass

---

## Prioridad

- Media

---

## Severidad

- Baja

---

## Evidencia

---

## Observaciones

- Ninguna