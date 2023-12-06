# ID
- UC - 001

# Caso de uso
- Registro de grupo

## Actores
- Profesor

## Tipo
- Primario

## Partes interesadas e intereses:
- El profesor tiene el interés de registrar un nuevo grupo para sus cursos.

## Breve descripción
El profesor puede llevar a cabo el proceso de registro de un nuevo grupo en el sistema, con la opción de asignar alumnos que ya se encuentren registrados, garantizando un sistema eficiente y en tiempo real.

## Disparador
El profesor accede a la funcionalidad "Registrar Nuevo Grupo" en la aplicación.

## Flujo normal de eventos
1. El profesor navega a la sección de registro de grupos.
2. Ingresa el nombre de la materia correspondiente al nuevo grupo.
3. Especifica el número de grupo que identificará a la clase.
4. Define el horario de la materia.
5. El sistema realiza validaciones para asegurar la integridad de la información ingresada.
6. Se verifica que no existan otros registros con el mismo número de grupo.
7. Se verifica la disponibilidad del horario, evitando conflictos con grupos ya existentes.
8. La información del nuevo grupo se almacena de manera segura en la base de datos.
9. Se presentan al profesor los detalles completos del grupo recién registrado.
10. El sistema emite un mensaje de confirmación para informar al profesor sobre el éxito de la operación.

## Subflujo-1: En el caso de que se encuentre otro registro con el mismo numero de grupo
1. Mostrar un mensaje de error al profesor que indique que ya existe un grupo con el mismo número.
2. Ofrecer al profesor la opción de modificar el número del grupo. Si el profesor opta por modificar el número, el caso de uso retoma el flujo normal en el paso 3. Si el profesor decide no hacer cambios, el caso de uso finaliza.

## Subflujo-2 En el caso de que no exista disponibilidad de horario para el registro del nuevo grupo
1. Mostrar un mensaje de error al profesor que indique que no hay horarios disponibles para el registro del nuevo grupo.
2. Ofrecer al profesor la opción de ajustar el horario del grupo. Si el profesor opta por ajustar el horario, el caso de uso se reinicia desde el paso 5. Si el profesor decide no ajustar el horario, el caso de uso finaliza.
Excepciones

## Postcondiciones 

- En el caso de que el profesor no tenga horarios disponibles para registrar un nuevo grupo, el sistema podría realizar las siguientes acciones:

- Mostrar un mensaje de error al profesor que indique que no tiene horarios disponibles.

- Ofrecer al profesor la opción de gestionar los horarios antes de continuar.
