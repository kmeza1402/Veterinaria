# Pruebas Backend

## Arquitectura

- Web sin SQL: Sí
- Web sin MySqlConnection: Sí
- Negocios usa Datos: Sí
- Datos usa MySql.Data: Sí

## Reglas

- Cliente con Mascotas: no se elimina (ReglaNegocioException)
- Mascota con Consultas: no se elimina (ReglaNegocioException)
- Fecha futura: validada en MascotaNegocio

## Consultas parametrizadas

- ClienteDatos: Sí
- MascotaDatos: Sí

## Correcciones realizadas

- Clientes/Eliminar y Mascotas/Eliminar: la carga de datos del OnPost se movió dentro del try para que una falla de MySQL no genere una página 500.