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
2. El sistema desplega la lista de grupos a los que el profesor esta asignado
3. Selecciona el grupo que desea dar de baja
4. El sistema muestra la informacion del grupo y el boton "Dar de baja"
6. El sistema pregunta si esta seguro de dar de baja el grupo seleccionado
7. El sistema muestra un mensaje indicando el resultado de la operación

## Subflujo-1: En el caso de que el profesor acepte la operacion (paso 6)

1. El grupo es eliminado del sistema de asistencia
2. El flujo continua en el paso 7

## Subflujo-2: En el caso de que el profesor cancele la operacion (paso 6)

1. El flujo continua en el paso 2

## Postcondiciones 

- El grupo y todos los alumnos que lo conforman son eliminados del sistema.
  
