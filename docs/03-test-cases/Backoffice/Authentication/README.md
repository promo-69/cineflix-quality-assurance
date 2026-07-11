# Authentication - Manual Test Cases

## Información General

Módulo: Authentication
Componente: Frontend Backoffice
Versión: v1.0
Responsable: Equipo QA - Nombre:

Última actualización: XX/07/2026

---

# Objetivo

Validar el correcto funcionamiento del proceso de autenticación y autorización del Backoffice de Cineflix, verificando que únicamente usuarios autorizados puedan acceder al sistema, que cada rol visualice únicamente los módulos permitidos y que las acciones disponibles respeten la matriz de permisos definida.

---

# Alcance

Este documento contempla pruebas funcionales y no funcionales relacionadas con:

- Login.
- Validación de credenciales.
- Persistencia de sesión.
- Logout.
- Protección de rutas.
- Roles.
- Permisos.
- Restricción de acciones.
- Manejo de sesiones expiradas.
- Accesibilidad.
- Responsive.

No forman parte del alcance:

- Registro de usuarios.
- Recuperación de contraseña.
- Gestión de usuarios.

Datos de Prueba: (05-test-data/UserData.md)


## Functional Testing

# Login

TC-AUTH-001 – Iniciar sesión correctamente como Super Administrador.
TC-AUTH-002 – Iniciar sesión correctamente como Gerente General.
TC-AUTH-003 – Iniciar sesión correctamente como Gerente de Sucursal Barquisimeto.
TC-AUTH-004 – Iniciar sesión correctamente como Gerente de Sucursal Caracas.
TC-AUTH-005 – Iniciar sesión correctamente como Cajero.
TC-AUTH-006 – Iniciar sesión correctamente como Operador (Usher).

# Validaciones del formulario
TC-AUTH-007 – Validar correo obligatorio.
TC-AUTH-008 – Validar contraseña obligatoria.
TC-AUTH-009 – Validar formato correcto del correo.
TC-AUTH-010 – Validar longitud mínima de contraseña.
TC-AUTH-011 – Impedir espacios en blanco únicamente.
TC-AUTH-012 – Eliminar espacios iniciales y finales del correo.
TC-AUTH-013 – Permitir pegar credenciales.
TC-AUTH-014 – Validar botón habilitado únicamente cuando los datos sean válidos.

# Credenciales inválidas
TC-AUTH-015 – Correo inexistente.
TC-AUTH-016 – Contraseña incorrecta.
TC-AUTH-017 – Correo vacío.
TC-AUTH-018 – Contraseña vacía.
TC-AUTH-019 – Ambos campos vacíos.
TC-AUTH-020 – Usuario cliente intentando acceder al Backoffice.

# Por cada cliente
TC-AUTH-021 – Usuario deshabilitado.
TC-AUTH-022 – Usuario eliminado.
TC-AUTH-023 – Error del servidor durante autenticación.

# Manejo de sesión
TC-AUTH-029 – Mantener sesión después de recargar la página.
TC-AUTH-030 – Restaurar sesión válida.
TC-AUTH-031 – Redireccionar al Login cuando el token expire.
TC-AUTH-032 – Invalidar sesión al cerrar sesión.
TC-AUTH-033 – Invalidar sesión al eliminar token manualmente.
TC-AUTH-034 – No permitir volver mediante botón "Atrás" después del logout.

# Logout
TC-AUTH-035 – Cerrar sesión correctamente.
TC-AUTH-036 – Limpiar almacenamiento local.
TC-AUTH-037 – Redireccionar al Login.
TC-AUTH-038 – Invalidar todas las rutas privadas.

# Protección de rutas
TC-AUTH-039 – Acceder a una ruta protegida sin autenticación.
TC-AUTH-040 – Redireccionar automáticamente al Login.
TC-AUTH-041 – Acceder mediante URL manual estando autenticado.
TC-AUTH-042 – Acceder mediante URL manual sin permisos.

## Roles y Permisos (RBAC)

# Super Administrador
TC-AUTH-043 – Visualizar todos los módulos.
TC-AUTH-044 – Acceder a todas las rutas.
TC-AUTH-045 – Ejecutar todas las acciones CRUD.
TC-AUTH-046 – Visualizar todos los botones.

# Gerente General
TC-AUTH-047 – Visualizar únicamente módulos autorizados.
TC-AUTH-048 – No visualizar módulos restringidos.
TC-AUTH-049 – Ejecutar únicamente acciones permitidas.

# Gerente de Sucursal
Realizar las pruebas para ambas sucursales.
TC-AUTH-050 – Visualizar únicamente información de su sucursal.
TC-AUTH-051 – No visualizar información de otras sucursales.
TC-AUTH-052 – CRUD únicamente sobre su sucursal.
TC-AUTH-053 – Restricción de reportes globales.
TC-AUTH-054 – Restricción de empleados de otra sucursal.

# Cajero (solamente venta de boletos y carameleria)
TC-AUTH-055 – Acceder únicamente a Venta de Boletos.
TC-AUTH-056 – Acceder únicamente a Caramelería.
TC-AUTH-057 – No visualizar módulos administrativos.
TC-AUTH-058 – No visualizar Finanzas.
TC-AUTH-059 – No visualizar Inventario.
TC-AUTH-060 – No visualizar Personal.

# Operador (Usher)
TC-AUTH-061 – Acceder únicamente a funciones autorizadas.
TC-AUTH-062 – No visualizar módulos administrativos.
TC-AUTH-063 – No visualizar Finanzas.
TC-AUTH-064 – No visualizar Reportes.

# Componentes protegidos
TC-AUTH-065 – Ocultar botones sin permisos.
TC-AUTH-066 – Deshabilitar botones restringidos.
TC-AUTH-067 – Mostrar botones únicamente con permiso.
TC-AUTH-068 – Ocultar acciones CRUD restringidas.
TC-AUTH-069 – Validar permisos dinámicos al cambiar de usuario.

# Cambios de rol
TC-AUTH-070 – Cerrar sesión e ingresar con otro rol.
TC-AUTH-071 – Actualizar permisos correctamente.
TC-AUTH-072 – No mantener permisos del usuario anterior. 

# Manejo de errores
TC-AUTH-073 – Error HTTP 400.
TC-AUTH-074 – Error HTTP 401.
TC-AUTH-075 – Error HTTP 403.
TC-AUTH-076 – Error HTTP 404.
TC-AUTH-077 – Error HTTP 500.
TC-AUTH-078 – Timeout del servidor.
TC-AUTH-079 – Sin conexión a Internet.


## Information Testing
TC-AUTH-080 – Validar título del Login.
TC-AUTH-081 – Validar placeholder del correo.
TC-AUTH-082 – Validar placeholder de contraseña.
TC-AUTH-083 – Validar mensajes de error.
TC-AUTH-084 – Validar mensajes de autenticación.
TC-AUTH-085 – Validar nombre del usuario autenticado.
TC-AUTH-086 – Validar nombre del rol.
TC-AUTH-087 – Validar ortografía.


## Navigation Testing
TC-AUTH-088 – Navegar al Dashboard después del Login.
TC-AUTH-089 – Navegar entre módulos permitidos.
TC-AUTH-090 – Impedir navegación a módulos restringidos.
TC-AUTH-091 – Mantener sesión durante la navegación.
TC-AUTH-092 – Redireccionar correctamente tras Logout.


## Integration Testing
TC-AUTH-093 – Obtener token correctamente.
TC-AUTH-094 – Obtener información del usuario.
TC-AUTH-095 – Obtener rol.
TC-AUTH-096 – Obtener permisos.
TC-AUTH-097 – Cargar menú según permisos.
TC-AUTH-098 – Validar autorización en cada petición.
TC-AUTH-099 – HTTP 200.
TC-AUTH-100 – HTTP 400.
TC-AUTH-101 – HTTP 401.
TC-AUTH-102 – HTTP 403.
TC-AUTH-103 – HTTP 404.
TC-AUTH-104 – HTTP 500.


## Accessibility Testing
TC-AUTH-105 – Navegación mediante teclado.
TC-AUTH-106 – Orden correcto del foco.
TC-AUTH-107 – Etiquetas accesibles.
TC-AUTH-108 – Lectura mediante lector de pantalla.
TC-AUTH-109 – Contraste adecuado.
TC-AUTH-110 – Escalado de texto.
TC-AUTH-111 – Interacción sin mouse.


## Responsive Testing
TC-AUTH-112 – Desktop Full HD.
TC-AUTH-113 – Laptop.
TC-AUTH-114 – Tablet vertical.
TC-AUTH-115 – Tablet horizontal.
TC-AUTH-116 – Mobile.
TC-AUTH-117 – Adaptación del formulario.
TC-AUTH-118 – Adaptación de mensajes.
TC-AUTH-119 – Adaptación del botón Login.
TC-AUTH-120 – Ausencia de scroll horizontal.