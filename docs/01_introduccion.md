# 1. Introducción General

En el ámbito del desarrollo de software y la ingeniería de datos, el almacenamiento persistente, la integridad y la disponibilidad de la información son pilares fundamentales. La presente práctica tiene como objetivo principal guiar y documentar el proceso formal de descarga, instalación, configuración y verificación de dos de los Sistemas Gestores de Bases de Datos Relacionales (RDBMS) más utilizados en la industria: **MySQL / SQL Server** y **PostgreSQL**.

* Preparar el entorno de desarrollo local cumpliendo con los requisitos de hardware y software requeridos.
* Ejecutar la instalación limpia de los motores de bases de datos seleccionados.
* Configurar parámetros críticos del sistema: asignación de puertos de escucha (`3306`, `1433`, `5432`), definición de codificación de caracteres (`UTF-8`) y establecimiento de credenciales para los usuarios administradores (`root` y `postgres`).
* Instalar y vincular las interfaces gráficas de usuario (GUI) correspondientes para la gestión visual de las bases de datos.
* Validar el correcto levantamiento de los servicios del sistema operativo mediante pruebas de conexión y ejecución de sentencias SQL elementales.

---

Un Sistema Gestor de Bases de Datos (SGBD o RDBMS) es un conjunto de herramientas de software que permite a los usuarios definir, crear, mantener y controlar el acceso a la base de datos de manera estructurada.

A diferencia del almacenamiento en archivos planos o soluciones no controladas, un RDBMS proporciona:
1. **Propiedades ACID (Atomicidad, Consistencia, Aislamiento y Durabilidad):** Garantizan que las transacciones en la base de datos se ejecuten de forma fiable y segura, evitando pérdidas de datos o inconsistencias ante fallos del sistema.
2. **Control de Concurrencia:** Permite que múltiples usuarios y aplicaciones accedan y modifiquen los datos simultáneamente sin interferir entre sí.
3. **Seguridad y Control de Acceso:** Implementa esquemas de permisos granulares por usuario y rol, protegiendo información sensible.
4. **Optimización de Consultas:** Mediante el uso del lenguaje estructurado **SQL (Structured Query Language)** e índices optimizados, los motores pueden procesar volúmenes masivos de datos en milisegundos.

---

[⬅️ Regresar al Índice Principal](../README.md) | [Siguiente: Instalación de SQL ➡️](02_instalacion_sql.md)
