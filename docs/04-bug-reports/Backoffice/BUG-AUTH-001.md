## BUG-AUTH-001

## Sesiòn activa luego de cerrar sesión

Al establecer una sesión dentro de la plataforma, cuando cierras sesión y se busca entrar desde otra sesión, aparece sesión activa

---

## Módulo
Authentication

---

## Tipo
Seguridad

---

## Prioridad
- Media

---

## Severidad
- Alta

---

## Ambiente
Producción

---

## Versión

Vr. 1

---

## Reportado por

Mary Sofía Pérez

---

## Fecha

16-07-2026

---

## Precondiciones

- Cerrar sesión desde el botón de "Cerrar sesión" y volver a tratar de iniciar sesión

---

## Pasos para reproducir

1. Loguearse primero con alguna de las cuentas disponibles
2. Cerrar sesión de dicha cuenta
3. Volver a loguearse con la misma u otra cuenta

---

## Resultado esperado

Cerrar la sesión antes activa, y permitirme iniciar otra sesión.

---

## Resultado obtenido

Al cerrar sesión y trato volver a iniciar sesión con la misma u otra cuenta, no se cierra bien la sesión mostrando "sesión activa"

---

## Frecuencia
- Siempre

---

## Evidencia

EVI-BUG-AUTH-001

---

## Estado
- Open

---

## Responsable
Javier

---

## Observaciones

Ninguna.