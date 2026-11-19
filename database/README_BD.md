# Base de datos Veterinaria

## Orden de ejecución
1. 00_crear_bd.sql
2. 01_datos_prueba.sql
3. 02_pruebas.sql

## Importante
La base de datos local NO se sincroniza automáticamente con GitHub.
GitHub conserva los scripts SQL. Cada integrante puede reconstruir
la misma base ejecutando los archivos en el orden indicado.

ADVERTENCIA:
00_crear_bd.sql contiene DROP DATABASE IF EXISTS Veterinaria.
Al ejecutarlo se elimina la base local Veterinaria y se crea nuevamente.

## Practica 6
- `03_verificacion_p6.sql`: consultas para revisar los datos.
- No crea la base. Se usa despues de las pruebas Web.

## Practica 7

Archivo agregado:

- `04_verificacion_final_p7.sql`

Finalidad:
comprobar el estado final de la base durante las pruebas de aceptacion,
incluyendo las 9 tablas, sus PK, sus FK y las reglas de integridad referencial.

Orden recomendado:

1. 00_crear_bd.sql
2. 01_datos_prueba.sql
3. 02_pruebas.sql
4. 03_verificacion_p6.sql
5. 04_verificacion_final_p7.sql

Nota: `00_crear_bd.sql` elimina y reconstruye la base local.

## Verificación final

Resultado de `04_verificacion_final_p7.sql`:

- 9 tablas: cliente, consulta, detalle_receta, mascota, medicamento, receta, rol, usuario, veterinario.
- 9 claves primarias y 8 llaves foráneas.
- Todas las llaves foráneas con UPDATE CASCADE y DELETE RESTRICT.
- Max conserva su consulta; PRUEBA P7 y PixelP7 devuelven 0 filas.

## Respaldo final

Archivo:
`backups/respaldo_veterinaria_p7.sql`

Estado:
generado después de aprobar P7, desde la base oficial de aceptación.

Restauración:
- si el dump incluye CREATE DATABASE, ejecutarlo directamente;
- si no lo incluye, ejecutar antes `00_crear_bd.sql`.

Importante: cargar los scripts desde Workbench o con
`--default-character-set=utf8mb4`; si no, los acentos se guardan dañados.
