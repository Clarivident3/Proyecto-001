# ID
- UC - 011

# Caso de uso
- Modificar grupo

## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses:
- El profesor tiene el interés de modificar los datos de un grupo

## Breve descripción
El profesor puede modificar los datos que ingresó inicialmente al registrar un grupo, es decir, materia, identificador, semestre y horario.

## Precondiciones
- El profesor tiene por lo menos un grupo asignado

## Flujo normal de eventos

1. El profesor selecciona la opción modificar, en el grupo correspondiente
2. El sistema muestra la información del grupo
3. El profesor selecciona el dato que desea modificar (Materia, ID, Semestre, Horario)
4. El profesor ingresa el nuevo dato en el campo seleccionado
6. El sistema muestra un mensaje con el resultado de la operación 

## Subflujo-1: En el caso de que el profesor seleccione ID u Horario (paso 3)

1. El profesor ingresa el nuevo dato en el campo seleccionado
2. El sistema verifica que los datos ingresados no se repitan en ningún otro grupo
   1. En caso de no repetirse: Los datos del grupo se modifican exitosamente
   2. En caso de repetirse: Los datos del grupo no se modifican
3. El flujo continua en el paso 6

