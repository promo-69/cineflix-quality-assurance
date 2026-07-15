# TC-BUS-005 – Verificar que las imágenes se visualicen correctamente

## Test Case ID

TC-BUS-005

---

## Módulo

Business

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar que las imágenes se visualicen correctamente

---

## Objetivo

Verificar que las dos imágenes del módulo Business ("Experiencia Cineflix" y "Cineflix Popcorn") carguen completamente, se rendericen con sus dimensiones correctas, sin íconos de imagen rota y con sus efectos hover funcionales.

---

## Precondiciones

- Navegador web actualizado.
- Conexión a internet disponible.
- URL /business accesible.

---

## Datos de prueba

- Ruta: /business
- Imagen 1: group-people-cinema.webp (alt="Experiencia Cineflix")
- Imagen 2: cinema-stuff-around-popcorn-heart.webp (alt="Cineflix Popcorn")

---

## Pasos

1. Abrir el navegador y navegar a /business.
2. Verificar que la imagen "Experiencia Cineflix" (group-people-cinema.webp) cargue correctamente.
3. Verificar que la imagen se muestre con sus dimensiones: altura responsive (h-56 sm:h-72 md:h-96 max-h-[320px] md:max-h-[420px]) y ancho completo.
4. Pasar el cursor sobre la imagen y verificar que se aplique el efecto hover.
5. Hacer clic en "Términos y Condiciones" y verificar que no se visualicen imágenes adicionales.
6. Hacer clic en "Marketing Empresarial" y verificar que no se visualicen imágenes.

---

## Resultado esperado

Ambas imágenes se cargan completamente sin errores (sin íconos de imagen rota). La imagen "Experiencia Cineflix" se muestra con bordes redondeados, borde semitransparente y sombra. El efecto hover de escala funciona al pasar el cursor. La imagen "Cineflix Popcorn" se muestra con opacidad que sube al hacer hover.

---

## Resultado obtenido

Cumple con la descripción dada en el resultado esperado.

---

## Estado

- Pass

---

## Prioridad

- Baja

---

## Severidad

- Media

---

## Evidencia

---

## Observaciones

- Ninguna