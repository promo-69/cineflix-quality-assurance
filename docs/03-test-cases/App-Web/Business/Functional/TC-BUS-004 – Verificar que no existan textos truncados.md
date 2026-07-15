# TC-BUS-004 – Verificar que no existan textos truncados

## Test Case ID

TC-BUS-004

---

## Módulo

Business

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar que no existan textos truncados

---

## Objetivo

Verificar que todos los textos de las tres pestañas se muestren completos sin truncamiento, sin mostrar "..." por desbordamiento de contenedor, y que párrafos largos como los de Términos y Condiciones o tarjetas de beneficios no se corten visualmente.

---

## Precondiciones

- Navegador web actualizado.
- Conexión a internet disponible.
- URL accesible.
- Resolución de pantalla: 1920x1080.

---

## Datos de prueba

- Ruta: https://frontend-web-teal-five.vercel.app/business
- Dispositivo: Desktop (1920x1080)
- Textos a revisar: párrafos introductorios, cláusulas de Términos, tarjetas de beneficios

---

## Pasos

1. Abrir el navegador y navegar a /business.
2. En "Sobre Nosotros", revisar que los párrafos introductorios se muestren completos.
3. Revisar que las tarjetas de beneficios ("Todo a un Toque", "CinePuntos", "Calidad Premium") no tengan texto cortado.
4. Hacer clic en "Términos y Condiciones".
5. Revisar que cada cláusula (PRIMERA a SÉPTIMA) muestre su contenido completo.
6. Verificar que el texto introductorio en itálica antes de las cláusulas se muestre completo.
7. Hacer clic en "Marketing Empresarial".
8. Revisar que el párrafo descriptivo y el bloque de contacto se muestren sin truncamiento.

---

## Resultado esperado

Todos los textos de las tres pestañas se visualizan completamente, sin truncamiento ni recorte por desbordamiento del contenedor. Los párrafos largos se ajustan al ancho disponible pero mantienen la totalidad de su contenido visible.

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

- Baja

---

## Evidencia

---

## Observaciones

- Ninguna