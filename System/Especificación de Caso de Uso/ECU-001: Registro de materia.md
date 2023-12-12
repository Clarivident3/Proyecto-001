# ID
- UC - 001

# Caso de uso
- Registro de materia

## Actores
- Profesor

## Tipo
- Primario

## Partes interesadas e intereses:
- El profesor tiene el interés de registrar una nueva materia en el sistema

## Breve descripción
El profesor puede llevar a cabo el proceso de registro de una nueva materia en el sistema, con la opción de asignar alumnos que ya se encuentren registrados, garantizando un sistema eficiente.

## Disparador
El profesor accede a la funcionalidad "Registrar Nuevo materia" en la aplicación.

## Flujo normal de eventos
1. El profesor navega a la sección de registro de materias.
2. Ingresa el nombre de la materia correspondiente.
3. Especifica el nombre de materia que identificará a la clase.
4. Define el horario de la materia.
5. El sistema realiza validaciones para asegurar la integridad de la información ingresada.
6. Se verifica que no existan otros registros con el mismo nombre de materia.
7. Se verifica la disponibilidad del horario, evitando conflictos con materias ya existentes.
8. La información de la nueva materia se almacena de manera segura en la base de datos.
9. Se presentan al profesor los detalles completos de la materia recién registrado.
10. El sistema emite un mensaje de confirmación para informar al profesor sobre el éxito de la operación.

## Subflujo-1: En el caso de que se encuentre otro registro con el mismo nombre de materia
1. Mostrar un mensaje de error al profesor que indique que ya existe una materia con el mismo nombre.
2. Ofrecer al profesor la opción de modificar el nombre de la materia. Si el profesor opta por modificar el número, el caso de uso retoma el flujo normal en el paso 3. Si el profesor decide no hacer cambios, el caso de uso finaliza.

## Subflujo-2 En el caso de que no exista disponibilidad de horario para el registro de la nueva materia
1. Mostrar un mensaje de error al profesor que indique que no hay horarios disponibles para el registro de la nueva materia.
2. Ofrecer al profesor la opción de ajustar el horario de la materia. Si el profesor opta por ajustar el horario, el caso de uso se reinicia desde el paso 5. Si el profesor decide no ajustar el horario, el caso de uso finaliza.
Excepciones

## Postcondiciones 

- En el caso de que el profesor no tenga horarios disponibles para registrar una nueva materia, el sistema podría realizar las siguientes acciones:

- Mostrar un mensaje de error al profesor que indique que no tiene horarios disponibles.

- Ofrecer al profesor la opción de gestionar los horarios antes de continuar.
