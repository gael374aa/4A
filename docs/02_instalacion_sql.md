# 2. Instalación de SQL

En esta sección se detalla el procedimiento completo para la instalación, configuración y verificación del sistema gestor de bases de datos MySQL Server en un entorno Windows.

---

## 2.1 Requisitos previos del sistema

Antes de comenzar la instalación de MySQL Server, es fundamental verificar que el sistema cumpla con los requisitos mínimos y recomendados:

| Componente | Requisito Mínimo | Requisito Recomendado |
| :--- | :--- | :--- |
| **Sistema Operativo** | Windows 10 (64-bit) / Windows Server 2019 | Windows 11 (64-bit) / Windows Server 2022 |
| **Procesador (CPU)** | 1.0 GHz x86-64 bits | 2.0 GHz o superior (Multi-core) |
| **Memoria RAM** | 2 GB | 4 GB o superior |
| **Espacio en Disco** | 1.5 GB libres (instalación básica) | 5 GB o más (según el volumen de datos) |
| **Software Adicional** | Microsoft .NET Framework 4.5.2+ | Microsoft Visual C++ Redistributable 2019/2022 |
| **Privilegios** | Permisos de Administrador | Permisos de Administrador |

---

## 2.2 Descarga y ejecución del instalador

Obtenga el paquete de instalación oficial de MySQL (*MySQL Installer for Windows*) desde el sitio oficial de Oracle/MySQL y ejecute el archivo `.msi`.

### Paso 1: Bienvenida a la instalación de MySQL Server
Inicie el ejecutable del instalador. Se mostrará la pantalla de bienvenida al asistente de instalación de MySQL Server. Haga clic en **Next** para continuar.

<div align="center">

![Bienvenida a la instalación de MySQL Server](<../assets/images/mySQL/1. Bienvenida a la instalación de MySQL Server.png>)

</div>

---

### Paso 2: Acuerdo de licencia de usuario final
Lea los términos del acuerdo de licencia (GNU General Public License). Marque la casilla **"I accept the terms in the License Agreement"** y presione **Next**.

<div align="center">

![Acuerdo de licencia de usuario final](<../assets/images/mySQL/2. Acuerdo de licencia de usuario final.png.png>)

</div>

---

### Paso 3: Selección del tipo de instalación
Seleccione el tipo de instalación deseado (*Typical*, *Custom* o *Complete*). Para la mayoría de casos de desarrollo se recomienda la opción predeterminada. Haga clic en **Next**.

<div align="center">

![Selección del tipo de instalación](<../assets/images/mySQL/3. Selección del tipo de instalación,png.png>)

</div>

---

### Paso 4: Progreso de la instalación de MySQL Server
El instalador comenzará a extraer y desplegar todos los archivos necesarios en su sistema. Espere a que la barra de progreso finalice.

<div align="center">

![Progreso de la instalación de MySQL Server](<../assets/images/mySQL/4. Progreso de la instalación de MySQL Server.png.png>)

</div>

---

### Paso 5: Finalización del asistente de instalación
Una vez completada la copia de archivos, el asistente indicará que la fase inicial ha terminado. Marque la opción para iniciar la configuración de MySQL y haga clic en **Finish**.

<div align="center">

![Finalización del asistente de instalación](<../assets/images/mySQL/5. Finalización del asistente de instalación.png.png>)

</div>

---

## 2.3 Configuración de instancias, puertos y credenciales

En esta fase se establecen los parámetros del servidor de base de datos, incluyendo la ubicación de datos, puertos de red, contraseñas de administrador y el servicio de Windows.

### Paso 6: Bienvenida al configurador de MySQL
Se iniciará automáticamente el asistente de configuración del servidor MySQL (*MySQL Server Configuration Wizard*). Haga clic en **Next** para comenzar.

<div align="center">

![Bienvenida al configurador de MySQL](<../assets/images/mySQL/6. Bienvenida al configurador de MySQL,png.png>)

</div>

---

### Paso 7: Directorio de datos
Especifique la ruta donde se almacenarán las bases de datos y los archivos del sistema de MySQL (o mantenga el directorio predeterminado). Haga clic en **Next**.

<div align="center">

![Directorio de datos](<../assets/images/mySQL/7. Directorio de datos.png.png>)

</div>

---

### Paso 8: Tipo de servidor y red
Configure el perfil del servidor (*Development Machine*, *Server Machine*, etc.) y las opciones de red TCP/IP (puerto predeterminado `3306`). Haga clic en **Next**.

<div align="center">

![Tipo de servidor y red](<../assets/images/mySQL/8. Tipo de servidor y red,png.png>)

</div>

---

### Paso 9: Cuentas y roles
Establezca la contraseña para la cuenta del usuario superadministrador (`root`). Opcionalmente, añada cuentas de usuario adicionales definiendo sus roles y permisos. Haga clic en **Next**.

<div align="center">

![Cuentas y roles](<../assets/images/mySQL/9. Cuentas y roles.png.png>)

</div>

---

### Paso 10: Configuración del servicio de Windows
Configure el servidor de MySQL para que se ejecute como un Servicio de Windows. Especifique el nombre del servicio (por ejemplo, `MySQL`) y seleccione si debe iniciarse automáticamente al arrancar el sistema.

<div align="center">

![Configuración del servicio de Windows](<assets/images/mySQL/10. Configuración del servicio de Windows.png.png>)

</div>

---

### Paso 11: Permisos de archivos del servidor
Establezca los permisos de acceso e intangibilidad para los directorios y archivos creados por el servidor de MySQL. Haga clic en **Next**.

<div align="center">

![Permisos de archivos del servidor](<../assets/images/mySQL/11. Permisos de archivos del servidor.png.png>)

</div>

---

### Paso 12: Bases de datos de muestra
(Opcional) Seleccione si requiere incluir bases de datos de muestra para pruebas de aprendizaje (como Sakila o World). Haga clic en **Next**.

<div align="center">

![Bases de datos de muestra](<../assets/images/mySQL/12. Bases de datos de muestra.png.png>)

</div>

---

### Paso 13: Aplicación de la configuración
Haga clic en el botón **Execute** para guardar las configuraciones, escribir el archivo de configuración `my.ini` e iniciar el servicio MySQL.

<div align="center">

![Aplicación de la configuración](<../assets/images/mySQL/13. Aplicación de la configuración.png.png>)

</div>

---

## 2.4 Verificación del servicio y conexión inicial

Para finalizar el proceso, confirme que la instancia de MySQL se encuentra activa y que es posible conectarse al servidor.

### Paso 14: Configuración completada
Una vez aplicadas todas las tareas de configuración de manera exitosa, haga clic en **Finish** para cerrar el asistente.

<div align="center">

![Configuración completada](<../assets/images/mySQL/14. Configuración completada.png.png>)

</div>

---

### Comprobación de servicio y conexión inicial

1. **Verificar servicio en Windows:**
   - Presione `Win + R`, escriba `services.msc` y presione Enter.
   - Busque el servicio `MySQL` y asegúrese de que su estado indique **En ejecución** (*Running*).

<div align="center">

![Configuración completada](<../assets/images/mySQL/Servicios.png>)

</div>


2. **Conexión inicial por línea de comandos:**
   - Abra la consola de comandos (`cmd` o `PowerShell`).
   - Conéctese al servidor ejecutando el siguiente comando:
     ```bash
     mysql -u root -p
     ```
   - Ingrese la contraseña establecida en el **Paso 9**. Una vez autenticado, se desplegará el prompt `mysql>`, confirmando una conexión exitosa.
  
   
<div align="center">

![Configuración completada](<../assets/images/mySQL/Acceso.png>)

</div>

