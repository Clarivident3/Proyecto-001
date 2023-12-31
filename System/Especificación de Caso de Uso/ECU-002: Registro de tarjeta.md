# ID
- UC - 002

# Caso de uso
- Registro de tarjeta.

## Actores
- Profesor

## Tipo
- Primario

## Partes interesadas e intereses:
- Profesor interesado en registrar una nueva tarjeta NFC en el sistema. 
 
## Breve descripción
Se describe el proceso mediante el cual un profesor registra tarjetas NFC para su uso en el sistema de asistencia, vinculándolas con estudiantes y sus respectivas materias.

## Disparador
El profesor accede a la funcionalidad "Registrar Tarjeta" en la aplicación.
## Precondiciones:
El profesor debe estar autenticado en el sistema.
La tarjeta debe estar disponible para su registro.

## Flujo normal de eventos
1.	El profesor selecciona la opción "Registro de Tarjeta" desde el menú principal de la aplicación.
2.	El sistema activa la funcionalidad NFC para permitir la lectura de la tarjeta.
3.	El profesor acerca la tarjeta al dispositivo para permitir la lectura del código NFC.
4.	El sistema verifica la validez de la tarjeta y su asociación con algún estudiante registrado.
5.	Si la tarjeta está asociada a un estudiante:
•	El sistema muestra la información del estudiante (nombre, materia, etc.).
•	El profesor confirma el registro de la tarjeta para ese estudiante.
•	Se registra la tarjeta en la base de datos del sistema como vinculada a ese estudiante.
6.	Si la tarjeta no está asociada a ningún estudiante:
•	El sistema notifica al profesor que la tarjeta no está registrada.
•	El profesor tiene la opción de asociar la tarjeta con un estudiante existente o de registrar a un nuevo estudiante.
•	Se actualiza la base de datos con la nueva asociación tarjeta-estudiante.

## Subflujo-1: La tarjeta no es válida
- Si la tarjeta no es válida o no puede ser leída, el sistema notifica al profesor con un mensaje de “error” y sugiere intentarlo nuevamente. 

## Subflujo-2: El profesor decide no asociar la tarjeta

- Si el profesor decide no asociar la tarjeta en este momento, puede cancelar la operación y regresar al menú principal. 

## Postcondiciones:
- La tarjeta queda registrada en el sistema y vinculada al estudiante correspondiente.
- En caso de asociar la tarjeta con un nuevo estudiante, se crea un nuevo registro de estudiante en el sistema.
