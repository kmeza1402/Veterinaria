# Línea base — Práctica 7

## Equipo
- Frontend: Aidan Zazueta Medrano
- Backend: Kevin A. Meza Espinoza
- DBA: Carlos Alberto Jaime Mascareño

## Estado inicial
- Fecha: 18 de noviembre de 2026
- Commit de main: 0b97e45
- Compila: Sí
- Ejecuta: Sí
- MySQL: Sí
- Clientes: Sí
- Mascotas: Sí

## Problemas conocidos antes de corregir

- Las páginas Eliminar cargan datos fuera del try en OnPost.
- La página Mascotas/Editar muestra el título "Nueva Mascota".

## Estado final

- Compila: Sí
- Ejecuta: Sí
- MySQL: Sí
- Clientes: APROBADO
- Mascotas: APROBADO
- Matriz de aceptación: 21/21

## Problemas resueltos

- Las páginas Eliminar cargaban datos fuera del try en OnPost; se movió la carga dentro del try.
- Frontend: se corrigió el título de Mascotas/Editar ("Editar Mascota").
- Frontend: los mensajes de error ahora se ven en pantalla.
- Frontend: se ajustó el diseño responsivo (390 px, 768 px y escritorio).
- Frontend: se agregó el manual de usuario (docs/MANUAL_USUARIO.md).

## Problemas pendientes

- Ninguno dentro del alcance obligatorio.