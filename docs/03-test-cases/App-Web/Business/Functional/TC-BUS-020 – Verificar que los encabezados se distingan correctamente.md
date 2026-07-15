# TC-BUS-020 – Verificar que los encabezados se distingan correctamente

## Test Case ID

TC-BUS-020

---

## Módulo

Business

---

## Categoría

- Functional

---

## Nombre del Caso

Verificar que los encabezados se distingan correctamente

---

## Objetivo

Verificar que los encabezados de cláusulas en Términos y Condiciones se distingan visualmente del cuerpo de texto mediante color, tamaño y peso de fuente, creando una jerarquía visual clara que facilite la lectura.

---

## Precondiciones

- Navegador web actualizado.
- Conexión a internet disponible.
- URL /business accesible.

---

## Datos de prueba

- Ruta: /business
- Tab: Términos y Condiciones
- Estilo encabezados: text-[#F6AD38] font-bold uppercase text-[11px] tracking-wider
- Estilo cuerpo: text-xs md:text-sm text-gray-300

---

## Pasos

1. Abrir el navegador y navegar a /business.
2. Hacer clic en la pestaña "Términos y Condiciones".
3. Verificar que "PRIMERA: OBJETO" se muestre en color dorado (#F6AD38), negrita y mayúsculas.
4. Verificar que el texto debajo de "PRIMERA: OBJETO" se muestre en gris y tamaño normal.
5. Repetir la verificación para "SEGUNDA: REGISTRO DEL USUARIO".
6. Repetir para "TERCERA: FINALIDAD Y TRATAMIENTO DE DATOS".
7. Repetir para "CUARTA: CONDICIONES DE COMPRA".
8. Repetir para "QUINTA: POLÍTICA DE CANCELACIÓN Y REEMBOLSO".
9. Repetir para "SEXTA: CLASIFICACIÓN Y ADMISIÓN".
10. Repetir para "SÉPTIMA: USO DEL PORTAL Y PROPIEDAD INTELECTUAL".
11. Verificar que el contraste entre encabezado y cuerpo sea suficiente para distinguir ambos niveles.

---

## Resultado esperado

Cada encabezado de cláusula se distingue claramente del cuerpo de texto mediante: color dorado (#F6AD38) y gris, texto en mayúsculas y  minúsculas, fuente en negrita y regular, y tamaño más pequeño y tamaño normal del cuerpo. La jerarquía visual permite identificar rápidamente cada cláusula.

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