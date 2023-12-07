# ID
- UC - 010

# Caso de uso
- Dar de baja grupo

## Actores
- Profesor

## Tipo
- Secundario

## Partes interesadas e intereses:
- Profesor interesado en dar de baja un grupo del sistema de asistencia.

## Breve descripción
El profesor puede dar de baja a un grupo del sistema de asistencia una vez que el curso haya finalizado o por alguna causa extraordinaria. 

## Precondiciones

- El profesor tiene por lo menos un grupo asignado

## Flujo normal de eventos

1. El profesor selecciona "Dar de baja grupo"
2. El sistema despliega la lista de grupos a los que el profesor esta asignado
3. Selecciona el grupo que desea dar de baja
4. El sistema muestra la información del grupo
5. El sistema muestra el botón "Dar de baja"
6. El profesor selecciona la opcion "Dar de baja"
7. El sistema muestra un mensaje indicando que el grupo fue dado de baja exitosamente


## Subflujo-3: En el caso de que el profesor no tenga grupos asignados (paso 2)

1. El sistema muestra el mensaje "No existen grupos"

## Postcondiciones 

- El grupo y todos los alumnos que lo conforman son eliminados del sistema.
