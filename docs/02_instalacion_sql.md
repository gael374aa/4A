# Instalación y configuración de MySQL Server 8

## Paso 1: Inicio de la instalación

Abre el ejecutable del instalador para iniciar el asistente de bienvenida de MySQL Server.

Esta pantalla confirma la versión del software que vas a instalar y asegura que el sistema cumple con los requisitos iniciales.

Haz clic en **Next**.

### Imagen

<div align="center">
  <img src="../assets/images/mySQL/1. Bienvenida a la instalacion de MySQL Server.png" alt="" width="50%">
</div>
---

## Paso 2: Aceptación de términos y licencias

Lee el acuerdo de licencia de usuario final (*End-User License Agreement - EULA*), el cual establece las condiciones legales de uso de MySQL Community Server.

Marca la casilla:

**I accept the terms in the License Agreement**

Después, haz clic en **Next**.

### Imagen

![Acuerdo de licencia de usuario final](imagenes/02-licencia-mysql.png)

---

## Paso 3: Selección del tipo de instalación

Elige la modalidad de instalación que deseas utilizar.

### Typical

Instala las características más comunes del motor de base de datos y las utilidades estándar.

Es la opción recomendada para la mayoría de los entornos de desarrollo local.

### Custom

Permite elegir manualmente qué componentes instalar y cambiar las rutas de instalación.

### Complete

Instala todas las características disponibles del paquete.

Para esta instalación, selecciona **Typical** y haz clic en **Next**.

### Imagen

![Selección del tipo de instalación](imagenes/03-tipo-instalacion.png)

---

## Paso 4: Ejecución del proceso de instalación

El asistente procederá a copiar los binarios, ejecutables de línea de comandos y librerías del sistema en el directorio de programas.

La ubicación puede ser similar a:

```text
C:\Program Files\MySQL\MySQL Server 8.0\
