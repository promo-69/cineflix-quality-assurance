# Bug ID

BUG-CPOS-001

---

## Título

Los tabs de categoría no filtran los productos en Candy Store.

---

## Módulo

CandyStore (Backoffice)

---

## Tipo

Funcional

---

## Prioridad

Alta

---

## Severidad

Alta

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

13/07/2026

---

## Precondiciones

- Cliente identificado.
- Catálogo de productos cargado.
- Productos con diferentes categorías (Drinks, Popcorn, Candies).

---

## Pasos para reproducir

1. Acceder al módulo Candy Store.
2. Identificar un cliente.
3. Hacer clic en el tab "Bebidas".
4. Observar los productos mostrados.

---

## Resultado esperado

Solo se muestran los productos de la categoría Drinks (Bebidas).

---

## Resultado obtenido

No se filtra ningún producto. Todos los tabs excepto "Todos" y "Combos" muestran el catálogo vacío porque los nombres de categoría en los tabs (`Palomitas`, `Bebidas`, `Dulces`) no coinciden con los valores asignados a los productos en el mapeo (`Popcorn`, `Drinks`, `Candies`).

---

## Frecuencia

Siempre

---

## Evidencia

/docs/07-evidence/backoffice/candystore/BUG-CPOS-001/

---

## Estado

Closed (Corregido)

---

## Responsable

Frontend

---

## Observaciones

Corregido en candyBar.jsx y Step3Confectionery.jsx. Las constantes CATEGORIES estaban en español pero el mapProduct asigna categorías en inglés. Se unificaron a inglés. Verificado fix — los tabs ahora filtran correctamente.
