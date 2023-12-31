# ID
- UC - 004

# Caso de uso
- Registro de alumnos.

## Actores
- Profesor

## Tipo
- Primario

## Partes interesadas e intereses:
-	Profesor: Interesado en registrar a los estudiantes en el sistema de asistencia, así como gestionar altas, bajas y cambios de alumnos.
-	Estudiante: Interesado en que su tarjeta NFC para tomar asistencia sea registrada correctamente.

## Breve descripción
Registrar un estudiante en el sistema de asistencia utilizando una tarjeta NFC, con la capacidad de gestionar altas, bajas y cambios de alumnos.
## Disparador
El profesor accede a la funcionalidad "Registro de alumnos" en la aplicación.
## Precondiciones:
- El profesor debe estar autenticado en el sistema.
- La tarjeta debe estar disponible para su registro.


## Flujo normal de eventos
1.	El profesor selecciona la opción "Registro de Alumno" desde el menú principal de la aplicación.
2.	El sistema activa la funcionalidad NFC para permitir la lectura de la tarjeta.
3.	El profesor acerca la tarjeta NFC al dispositivo para permitir la lectura del código NFC.
4.	El sistema verifica la validez de la tarjeta NFC y su asociación con algún estudiante registrado.
5.	Si la tarjeta está asociada a un estudiante:
•	El sistema muestra la información del estudiante (nombre, grupo, numero de cuenta).
6.	El profesor tiene la opción de realizar los siguientes cambios:
-	Cambio de grupo: El profesor selecciona el nuevo grupo al que desea asignar al estudiante.
-	Alta de estudiante: El profesor introduce los datos del estudiante, como nombre, grupo, etc.
-	Baja de estudiante: El profesor confirma la baja del estudiante.
7.	Se actualiza la base de datos con los cambios realizados.
8.	Si la tarjeta no está asociada a ningún estudiante:
-	El sistema notifica al profesor que la tarjeta NFC no está registrada.
-	El profesor tiene la opción de asociar la tarjeta NFC con un estudiante existente o de registrar a un nuevo estudiante.
9.	Se actualiza la base de datos con la nueva asociación tarjeta-estudiante.
## Subflujo 1: Tarjeta no válida o no leída
1.	El sistema detecta que la tarjeta NFC no es válida o no puede ser leída.
2.	Se muestra un mensaje de "error" notificando al profesor sobre la situación.
3.	Se proporcionan sugerencias para intentar nuevamente, como acercar la tarjeta NFC de manera más precisa al dispositivo.
4.	El profesor tiene la opción de repetir el proceso o cancelar la operación.
## Subflujo-2: No asociar la tarjeta en este momento
1.	El profesor decide no asociar la tarjeta en el momento actual.
2.	Se le presenta la opción de cancelar la operación.
3.	El sistema confirma la cancelación y devuelve al profesor al menú principal de la aplicación.
4.	En caso de cancelación, no se realiza ningún cambio en la base de datos y la tarjeta no se vincula a ningún estudiante
## Subflujo-3: Gestionar cambios en grupos
1.	Si la tarjeta NFC está asociada a un estudiante y el profesor elige gestionar cambios en grupos, se presenta la opción de asignar el estudiante a un nuevo grupo.
2.	El profesor selecciona el nuevo grupo al que desea asignar al estudiante.
3.	La base de datos se actualiza con la nueva asignación de grupo para el estudiante.
## Postcondiciones:
1.	 Tarjeta NFC Asociada a Estudiante Existente:
- La tarjeta NFC queda registrada en el sistema.
-	Se vincula a un estudiante existente seleccionado por el profesor.
-	La base de datos se actualiza con la asociación de la tarjeta al estudiante.

2.	No se crea un nuevo registro de estudiante.
-	Tarjeta NFC No Asociada en el Momento:
-	El profesor decide no asociar la tarjeta NFC en el momento actual.
-	La operación se cancela y no se realiza ningún cambio en la base de datos.
-	La tarjeta NFC no se vincula a ningún estudiante.

3.	Tarjeta NFC Asociada a Estudiante Existente o Nuevo Estudiante:
-	La tarjeta no está asociada a ningún estudiante.
-	El profesor elige asociar la tarjeta a un estudiante existente o registrar a un nuevo estudiante.
-	Si asociada a un estudiante existente, se vincula a ese estudiante específico.
-	Si registrada con un nuevo estudiante, se crea un nuevo registro de estudiante en la base de datos.
-	La base de datos se actualiza con la nueva asociación tarjeta-estudiante.
