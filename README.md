📌 Sistema de Tareas

Este proyecto es una API REST desarrollada con Spring Boot que permite gestionar tareas, incluyendo operaciones básicas como crear, listar, actualizar y eliminar tareas.

🚀 Tecnologías utilizadas
Java
Spring Boot
Spring Data JPA
MySQL
Maven


🧩 Estructura del proyecto
El sistema está organizado en capas siguiendo el patrón MVC:

  📦 Modelo (Entity)
  Las clases de esta capa representan las tablas de la base de datos.
  
  Ejemplo:
  Tarea: contiene atributos como id, nombre, descripción, estado, etc.
  
  📦 Repositorio (Repository)
  Encargado de la comunicación con la base de datos mediante JPA.
  
  Ejemplo:
  TareaRepository: extiende de JpaRepository y permite realizar operaciones CRUD sin escribir SQL.
  
  📦 Servicio (Service)
  Aquí se encuentra la lógica del negocio.
  
  Ejemplo:
  TareaService: contiene métodos para guardar, actualizar, eliminar y consultar tareas.
  
  📦 Controlador (Controller)
  Expone los endpoints de la API.
  
  Ejemplo:
  TareaController: maneja las peticiones HTTP (GET, POST, PUT, DELETE).

  
🔄 Funcionamiento del sistema:
El flujo del sistema es el siguiente:

*El cliente realiza una petición HTTP (por ejemplo: GET /tareas)

*El controlador recibe la petición

*El servicio procesa la lógica

*El repositorio accede a la base de datos

*Se devuelve la respuesta al cliente
