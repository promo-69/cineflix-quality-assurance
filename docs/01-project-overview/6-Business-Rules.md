# Business Rules

## Información General

Proyecto: Cineflix
Versión: 1.1
Documento: Business Rules
Responsable: Equipo QA
Última actualización: 12/07/2026

---

# Objetivo

Documentar las reglas de negocio que gobiernan el funcionamiento del sistema Cineflix tanto para la plataforma Web Cliente, Aplicación Móvil, Backoffice y API REST.

Estas reglas representan restricciones funcionales, operacionales y de negocio que deberán cumplirse durante el desarrollo, pruebas y mantenimiento del sistema.

---

# Alcance

Las reglas aquí descritas aplican a:

- Web Cliente
- Aplicación Móvil
- Backoffice
- API REST

No incluyen reglas técnicas de infraestructura.

## Componente: Web Backoffice
# Modulo:

# Employees
- Al registrar un empleado, el correo utilizado para el mismo deberá ser creado por el negocio, esto no implica que el sistema haga un correo institucional.
- Se le deberá de facilitar a todo nuevo empleado los datos de acceso al sistema, esto implica el correo y contraseña.

# Billboard
- Toda película al registrarse, deberá iniciar en estado de Próximamente.
- Toda película en estado de Próximamente cambiará automáticamente a Cartelera (Estreno) en su fecha de estreno.
- Toda película permanecerá siete días en estado Cartelera (Estreno) antes de pasar al estado de Cartelera (Regular).


## Componente: Web Cliente y App Mobile

# Authentication:
- Todo usuario deberá autenticarse en el sistema utilizando un correo electronico y contraseña valida
- La contraseña debe de tener un minimo de 8 carácteres, y poseer por lo menos 1 carácter especial, 1 letra mayúsculas, y 1 número.
- Después de 5 intentos fallidos seguidos al intentar logearse el sistema debe de bloquear temporalmente la cuenta por 10min.
- El sistema únicamente permitirá el acceso a usuarios activos y verificados.

# CandyStore
- Todo producto o combo de confitería deberá de ser retirado en la sucursal seleccionada el mismo día de la compra.

# Home
- En el home únicamente se podran observar todas aquellas películas y eventos activos.
- Las películas en estado de proximamente no se mostraran en el carrusel principal de la página.
- Los eventos no se mostraran en el carrusel principal de la página.
- Toda aquella película o evento que este en estado fuera de cartelera no podrán visualizarse.

# Payment
- Los asientos, y en dado caso los artículos de confitería, permanecerán reservados durante diez minutos hasta finalizar el proceso de compra.
- Pasado el tiempo de los 10min sin la cancelación del monto de la orden de compra, se liberarán automaticamente los asientos y/o artículos seleccionados.
- Toda compra permitirá incluir boletos y productos de confitería dentro de una única orden.



# Profile:
- Toda modificación de información personal requiere la contraseña actual del usuario. Una vez realizada la modificación exitosamente, el sistema debe cerrar la sesión automáticamente y redirigir al Login para que el usuario vuelva a autenticarse con sus nuevos datos.

# Payment:
- Todo producto de confitería comprado debe retirarse el mismo día de la compra.
- Todo proceso de compra desde la seleccion de asientos hasta el pago de la orden debe de realizarse en un máximo de 10min.

# RoomRental
- Toda solicitud realizada por el cliente debe ser realizada con un minimo de 2 semanas de anticipación.