 # Arquitectura

## Veterinaria.Web
Interfaz y Razor Pages. No contiene SQL
ni conexiones a MySQL.

## Veterinaria.Negocios
Reglas y validaciones.

## Veterinaria.Datos
ADO.NET y MySQL.

## Veterinaria.Entidades
Modelos compartidos (Cliente, Mascota).

## Flujo

Web
↓
Negocios
↓
Datos
↓
MySQL

## Ejemplo: eliminar un Cliente

1. El usuario pulsa Eliminar en la página de Clientes.
2. La página Web llama a ClienteNegocio.Eliminar(id).
3. Negocios pregunta a ClienteDatos si el cliente tiene mascotas.
4. Si tiene mascotas, lanza ReglaNegocioException.
5. La página Web muestra el mensaje al usuario.
6. Si no tiene mascotas, ClienteDatos ejecuta el DELETE en MySQL.

## Ejemplo: eliminar una Mascota

1. La página Web llama a MascotaNegocio.Eliminar(id).
2. Negocios pregunta a MascotaDatos si la mascota tiene consultas.
3. Si tiene consultas, lanza ReglaNegocioException.
4. Si no tiene consultas, MascotaDatos ejecuta el DELETE en MySQL.

## Manejo de errores

- Reglas de negocio: ReglaNegocioException, con un mensaje
  entendible para el usuario.
- Errores técnicos: se registran con Debug.WriteLine y al
  usuario se le muestra un mensaje amigable, sin detalles.