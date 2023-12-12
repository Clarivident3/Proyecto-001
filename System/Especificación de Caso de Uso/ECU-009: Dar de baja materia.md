# ID
- UC - 009

# Caso de uso
- Dar de baja materia

## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses:
- Profesor interesado en dar de baja una materia del sistema de asistencia.

## Breve descripción
El profesor puede dar de baja una materia del sistema de asistencia una vez que esta haya finalizado o por alguna causa extraordinaria. 

## Precondiciones

- El profesor tiene por lo menos una materia asignada

## Flujo normal de eventos

1. El profesor selecciona "Dar de baja materia"
2. El sistema despliega la lista de materias a las que el profesor esta asignado
3. El profesor selecciona la materia que desea dar de baja
4. El sistema muestra la información de la materia
6. El profesor selecciona la opcion "Dar de baja"
7. El sistema muestra un mensaje indicando que la materia fue dada de baja exitosamente


## Subflujo-1: En el caso de que el profesor no tenga materias asignadas (paso 2)

1. El sistema muestra el mensaje "No existen materias"

