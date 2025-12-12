# CRUD de Huéspedes (Java + Swing + MySQL)

Aplicación de escritorio hecha en Java Swing que permite gestionar huéspedes de un hotel usando operaciones CRUD conectadas a una base de datos MySQL.

Incluye:

* Insertar huéspedes

* Cargar huéspedes por su código

* Actualizar datos

* Eliminar registros

* Listar todos los huéspedes

* Validaciones básicas de campos

* Documentación JavaDoc integrada

# 🧱 Funcionalidades principales

✔ Insertar huésped  
✔ Cargar datos por código  
✔ Actualizar datos del huésped  
✔ Eliminar registro  
✔ Listar huéspedes (se muestran en la consola de Eclipse)  

Cada huésped contiene:

* codigoHuesped
* nombre
* apellidos
* direccion
* ciudad
* numTarjeta
* numHabitacion

# 🛠️ Tecnologías utilizadas

1. Java SE (Swing)

2. Eclipse IDE

3. MySQL 8

4. JDBC Connector (mysql-connector-j)

5. Patrón MVC (básico): Modelo + DAO + Vista

# 📁 Estructura del proyecto 
```
crud/ 
  ├── Huesped.java → Modelo 
  ├── DataHuesped.java → Acceso a datos (DAO) 
  ├── PantallaHuesped.java → Vista / Controlador (Swing)
```

# 📚 Añadir el driver JDBC en Eclipse

1. Descargar `mysql-connector-j.jar`  

2. En Eclipse → clic derecho al proyecto Properties → Java Build Path → Add External JARs  

3. Selecciona el `archivo .jar`

4. Aplicar y cerrar

Sin esto tendrás: No suitable driver found for `jdbc:mysql://...`

# ▶️ Cómo ejecutar

## Importar el proyecto en Eclipse

Verificar que la BD hotel existe

Ejecutar:

`crud.PantallaHuesped`

Aparecerá la ventana del CRUD.

# 🖥️ Uso de la interfaz Insertar

Rellena todos los campos

Clic en Insertar

Mensaje: Se insertó correctamente

Cargar

Clic en Cargar

Introduce el código

Si existe → se rellena el formulario

Si no → aviso de que no existe

Actualizar

Cargar un huésped

Modificar los campos

Clic en Actualizar

Eliminar

Clic en Eliminar

Introduce código

Si existe, se borra

Listar

Clic en Listar

Los huéspedes aparecerán en la consola de Eclipse.

Ejemplo:

1 - Ana Pérez - Hab: 101 2 - Juan López - Hab: 203

# 📝 JavaDoc

El proyecto incluye comentarios preparados para JavaDoc.

Generarlo:

En Eclipse: Project → Generate Javadoc...

Selecciona el proyecto

Ejecutar

Se generará documentación HTML.
