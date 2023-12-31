# ID

- UC - 005

# Caso de uso

- Borrar tarjeta

## Actores

- Profesor

## Tipo

- Secundario

## Partes interesadas e intereses:

- Profesor: Interesado en borrar la información de una tarjeta de estudiante del sistema de asistencia.

## Breve descripción

Permite al profesor borrar la información de una tarjeta de estudiante del sistema de asistencia.

## Disparador

El profesor selecciona la opción "Borrar tarjeta" desde el menú principal de la aplicación.

## Precondiciones
- El profesor debe estar autenticado en el sistema.
- La tarjeta debe estar disponible para su borrado.

## Flujo normal de eventos

1. El profesor selecciona la opción "Borrar tarjeta" desde el menú principal de la aplicación.
2. El sistema activa la funcionalidad NFC para permitir la lectura de la tarjeta.
3. El profesor acerca la tarjeta NFC al dispositivo para permitir la lectura del código NFC.
4. El sistema verifica la validez de la tarjeta NFC.
5. El sistema confirma la operación de borrado.
6. La base de datos se actualiza para eliminar la asociación entre la tarjeta NFC y cualquier estudiante registrado.

## Subflujo-1: Tarjeta no asociada a ningún estudiante

1. El sistema detecta que la tarjeta no está asociada a ningún estudiante.
2. El sistema notifica al profesor que la tarjeta no está registrada.
3. El profesor tiene la opción de cancelar la operación.
4. Si se cancela la operación, no se realizan cambios en la base de datos.

## Postcondiciones:

- La información de la tarjeta NFC se elimina del sistema.
- La tarjeta NFC ya no se puede utilizar para registrar la asistencia de un estudiante.
