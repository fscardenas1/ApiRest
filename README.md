# ApiRest
# API de Gestión de Tareas

Esta es una API simple para gestionar una lista de tareas utilizando Spring Boot y Spring Data JPA.

## Cómo acceder a la API

La API se ejecuta en `http://localhost:8080`. Asegúrate de que tu aplicación Spring Boot esté en funcionamiento antes de realizar solicitudes.

## Endpoints

### Obtener todas las tareas

- Método: GET
- URL: `/api/tasks`

### Obtener una tarea por ID

- Método: GET
- URL: `/api/tasks/{id}`
- Ejemplo: `/api/tasks/1`

### Crear una nueva tarea

- Método: POST
- URL: `/api/tasks`
- Cuerpo: JSON con los datos de la tarea (name, description, date, status)

### Actualizar una tarea existente

- Método: PUT
- URL: `/api/tasks/{id}`
- Cuerpo: JSON con los nuevos datos de la tarea (name, description, date, status)
- Ejemplo: `/api/tasks/1`

### Eliminar una tarea

- Método: DELETE
- URL: `/api/tasks/{id}`
- Ejemplo: `/api/tasks/1`

## Ejemplos de Solicitudes

### Obtener todas las tareas

### Crear una nueva tarea

POST /api/tasks
Content-Type: application/json

{
"name": "Nueva tarea",
"description": "Descripción de la nueva tarea",
"date": "2023-08-21",
"status": "Pendiente"
}

### Actualizar una tarea existente

PUT /api/tasks/1
Content-Type: application/json

{
"name": "Tarea actualizada",
"description": "Descripción actualizada",
"date": "2023-08-22",
"status": "En progreso"
}


## Notas

- Asegúrate de tener tu aplicación Spring Boot en ejecución antes de realizar las solicitudes.
- Los campos como `name`, `description`, `date` y `status` deben ajustarse según las necesidades del proyecto.