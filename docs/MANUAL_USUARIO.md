# Manual de usuario

## Sistema de gestión veterinaria

Este manual describe el uso de los módulos de **Clientes** y **Mascotas** del sistema de gestión veterinaria.

## 1. Inicio

Al ingresar al sistema se muestra el panel principal del Centro Veterinario.

Desde esta pantalla se puede acceder a:

- **Clientes**: administración de propietarios.
- **Mascotas**: registro y consulta de mascotas.

También se puede utilizar la barra lateral para navegar entre las secciones disponibles:

- Inicio
- Clientes
- Mascotas
- Veterinarios
- Consultas
- Recetas

Los módulos de Veterinarios, Consultas y Recetas pueden mostrar un aviso de que se encuentran en preparación.

## 2. Consultar clientes

1. Seleccione **Clientes** en la barra lateral o desde la tarjeta de Clientes en Inicio.
2. El sistema mostrará una tabla con los clientes registrados.
3. La tabla presenta:
   - Nombre completo.
   - Teléfono.
   - Correo electrónico.
   - Acciones disponibles.
4. Cada cliente puede consultarse mediante las opciones **Ver**, **Editar**, **Mascotas** y **Eliminar**.

Si ocurre un problema de conexión o consulta, el sistema mostrará un mensaje de error.

## 3. Buscar cliente

1. Ingrese a la sección **Clientes**.
2. Escriba el texto de búsqueda en el campo **Buscar por nombre, teléfono o correo**.
3. Seleccione **Buscar**.
4. El sistema mostrará los clientes que coincidan con el texto ingresado.

La búsqueda puede coincidir con:

- Nombre.
- Apellido paterno.
- Apellido materno.
- Teléfono.
- Correo electrónico.

Para volver a consultar todos los clientes, seleccione **Limpiar**.

## 4. Registrar cliente

1. Ingrese a **Clientes**.
2. Seleccione **Nuevo cliente**.
3. Capture la información solicitada:
   - Nombre.
   - Apellido paterno.
   - Apellido materno.
   - Teléfono.
   - Correo electrónico.
   - Dirección.
4. Seleccione **Guardar**.

Los campos obligatorios son:

- Nombre.
- Apellido paterno.
- Teléfono.

Si falta información obligatoria, el sistema mostrará un mensaje de validación y no guardará el registro hasta corregirlo.

Para salir sin guardar, seleccione **Cancelar**.

## 5. Editar cliente

1. Ingrese a **Clientes**.
2. Localice el cliente que desea modificar.
3. Seleccione **Editar**.
4. Actualice los datos necesarios.
5. Seleccione **Guardar cambios**.

El identificador del cliente se conserva automáticamente. Para descartar los cambios, seleccione **Cancelar**.

## 6. Ver detalle de cliente

1. Ingrese a **Clientes**.
2. Localice el cliente.
3. Seleccione **Ver**.

La pantalla de detalle muestra:

- Nombre completo.
- Teléfono.
- Correo electrónico.
- Dirección.
- Mascotas asociadas al cliente, cuando existen.

Desde esta pantalla también están disponibles las opciones:

- **Ver Mascotas**: muestra las mascotas pertenecientes al cliente.
- **Editar**: permite modificar los datos del cliente.
- **Regresar**: vuelve al listado de clientes.

## 7. Ver mascotas de un cliente

Existen dos formas de consultar las mascotas de un cliente:

### Desde el listado de clientes

1. Ingrese a **Clientes**.
2. Localice al propietario.
3. Seleccione **Mascotas**.

### Desde el detalle del cliente

1. Abra el detalle del cliente mediante **Ver**.
2. Seleccione **Ver Mascotas**.

El sistema abrirá el listado de mascotas filtrado para mostrar únicamente las asociadas al cliente seleccionado.

## 8. Consultar / filtrar mascotas

1. Seleccione **Mascotas** en la barra lateral.
2. El sistema mostrará las mascotas registradas.
3. La tabla incluye:
   - Nombre.
   - Especie.
   - Raza.
   - Sexo.
   - Propietario.
   - Acciones disponibles.

Las mascotas se muestran ordenadas por nombre.

Para filtrar las mascotas por propietario, acceda desde la opción **Mascotas** de un cliente o desde **Ver Mascotas** en su detalle. El listado mostrará únicamente las mascotas de ese cliente.

Actualmente no existe un campo de búsqueda de texto independiente para filtrar mascotas por nombre, especie o raza.

## 9. Registrar mascota

1. Ingrese a **Mascotas**.
2. Seleccione **Nueva mascota**.
3. Capture la información solicitada:
   - Propietario.
   - Nombre.
   - Especie.
   - Raza.
   - Sexo.
   - Fecha de nacimiento.
   - Color.
   - Señas particulares.
4. Seleccione **Guardar**.

Los campos obligatorios son:

- Propietario.
- Nombre de la mascota.
- Especie.

La fecha de nacimiento no puede ser posterior a la fecha actual.

Si no existen clientes registrados, primero debe registrar un cliente. En ese caso, el botón **Guardar** permanece deshabilitado.

Para salir sin guardar, seleccione **Cancelar**.

## 10. Editar mascota

1. Ingrese a **Mascotas**.
2. Localice la mascota que desea modificar.
3. Seleccione **Editar**.
4. Actualice la información necesaria.
5. Seleccione **Guardar cambios**.

Se pueden modificar el propietario y los datos de la mascota. El identificador de la mascota se conserva automáticamente.

Para descartar los cambios, seleccione **Cancelar**.

## 11. Ver detalle de mascota

1. Ingrese a **Mascotas**.
2. Localice la mascota.
3. Seleccione **Ver**.

La pantalla de detalle muestra:

- Nombre.
- Propietario.
- Especie.
- Raza.
- Sexo.
- Fecha de nacimiento.
- Color.

Cuando no se registró una fecha de nacimiento o un color, el sistema muestra **No registrada** o **No registrado**, respectivamente.

Desde esta pantalla puede:

- Seleccionar **Editar** para modificar la mascota.
- Seleccionar **Regresar** para volver al listado.

## 12. Reglas de eliminación

Las eliminaciones requieren confirmación mediante una pantalla específica. Después de seleccionar **Eliminar**, revise el aviso y confirme la operación.

### Eliminar un cliente

Un cliente no puede eliminarse si tiene mascotas registradas.

Si se intenta eliminarlo en esas condiciones, el sistema mostrará el mensaje:

> No se puede eliminar el cliente porque tiene mascotas registradas.

Para eliminar el cliente, primero deben resolverse las mascotas asociadas según las reglas del sistema.

### Eliminar una mascota

Una mascota no puede eliminarse si tiene consultas registradas.

Si se intenta eliminarla en esas condiciones, el sistema mostrará el mensaje:

> No se puede eliminar la mascota porque tiene consultas registradas.

### Cancelar una eliminación

En cualquiera de las pantallas de confirmación, seleccione **Cancelar** para volver al listado sin eliminar el registro.

### Registros inexistentes

Si el registro solicitado ya no existe o el identificador no es válido, el sistema puede mostrar una página de recurso no encontrado o un mensaje de error.
