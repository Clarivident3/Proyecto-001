# ID
- UC - 006

# Caso de uso
- Borrar alumno

## Actores
- Profesor
  
## Tipo
- Secundario

## Partes interesadas e intereses:
- Profesor: Interesado en eliminar un registro de estudiante del sistema de asistencia.

## Breve descripción
Permite al profesor eliminar un registro de estudiante del sistema de asistencia.

## Disparador
El profesor selecciona la opción "Borrar alumno" desde el menú principal de la aplicación.

## Precondiciones
-El profesor debe estar autenticado en el sistema.
-El profesor debe haber iniciado sesión en la aplicación.
-El alumno debe estar registrado en el sistema.

## Flujo normal de eventos
1. El profesor selecciona la opción "Borrar alumno" desde el menú principal de la aplicación.
2. El sistema muestra una lista de todos los alumnos registrados.
3. El profesor selecciona el alumno que desea eliminar.
4. El sistema confirma la operación de borrado.
5. El sistema elimina el registro del alumno de la base de datos.

## Postcondiciones
- El registro del alumno se elimina de la base de datos.
- El alumno ya no se puede utilizar para registrar la asistencia.
