# ID
- UC - 012

# Caso de uso
- Cambio de tarjeta

## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses:
- El profesor tiene el interés de cambiar la tarjeta asignada a un alumno.

## Breve descripción
El profesor puede cambiar la tarjeta que está asignada a los datos de un alumno cuando éste lo solicite, por pérdida o por alguna otra razón. Para esto, el sistema transfiere los datos a la nueva tarjeta y elimina del registro a la anterior.

## Precondiciones

- El profesor debe tener por lo menos a un alumno asignado en alguno de sus cursos

## Flujo normal de eventos
1. El sistema despliega la lista de alumnos asignados al profesor
2. El profesor selecciona la opción “Cambiar tarjeta” en el alumno que desea
4. El profesor escanea la nueva tarjeta de Movilidad Integrada del alumno 
5. El sistema verifica que el  ID de la tarjeta no exista en el registro
6. El sistema muestra un mensaje indicando el resultado de la operación

## Subflujo-1: En el caso de que el ID de la tarjeta nueva ya se encuentre en el registro (paso 5)

1. El sistema no realiza el cambio de tarjeta
2. El flujo continua en el paso 6

## Subflujo-3: En el caso de que el ID de la tarjeta nueva no se encuentre en el registro (paso 5)

1. El sistema transfiere los datos de la tarjeta asignada a la nueva tarjeta
2. El sistema asigna la nueva tarjeta al registro del alumno correspondiente
3. El flujo continua en el paso 6


## Postcondiciones 

En caso del subflujo 3, el sistema eliminará los datos de la tarjeta anterior de forma permanente, reemplazandolos por los de la nueva tarjeta proporcionada 
