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

## Postcondiciones 

- En caso del subflujo 2, el sistema eliminará todos los datos del profesor en cuestión. 
