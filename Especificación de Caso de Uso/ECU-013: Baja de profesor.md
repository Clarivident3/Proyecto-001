# ID
- UC - 013

# Caso de uso
- Baja de profesor

## Actores
- Administración Escolar

## Tipo
- Secundario

## Partes interesadas e intereses:
- La Administración escolar tiene el interés de dar de baja a un profesor del sistema.

## Breve descripción
La Administración escolar lleva a cabo el proceso de dar de baja a un profesor del sistema, esto cuando el profesor en cuestión cesa de sus funciones por cualquier motivo. 

## Precondiciones
- La facultad debe de contar con por lo menos un profesor dado de alta previamente en el sistema

## Flujo normal de eventos
1. El administrador inicia sesión en el sistema
2. Accede a la seccion de gestion de usuarios
3. El sistema despliega la lista de profesores existentes en el registro, ordenados alfabéticamente
4. El administrador selecciona al profesor que desea
5. El sistema despliega los datos del profesor seleccionado 
6. El administrador selecciona la opción “Dar de baja”
7. El sistema solicita confirmación del administrador
8. El sistema muestra el resultado de la operación 

## Subflujo-1: En el caso de que el administrador cancele la operación (paso 7)
1. El flujo continua en el paso 5

## Subflujo-2: En el caso de que el administrador confirme la operación (paso 7)
1. El sistema solicita la contraseña de inicio de sesión del administrador
2. Si la contraseña es correcta, se da de baja al profesor, eliminando todos sus datos del registro, así como los grupos que tiene asignados
3. Si la contraseña es incorrecta, se vuelve a solicitar hasta que sea ingresada correctamente
4. El flujo continua en el paso 8


## Postcondiciones 

- En caso del subflujo 2, el sistema eliminará todos los datos del profesor en cuestión. 
