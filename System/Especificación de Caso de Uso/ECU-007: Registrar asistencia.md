
# ID
- UC - 007

# Caso de uso
- Registrar Asistencia

## Actores
- Porofesor
- Alumnos

## Tipo
- Primario

## Partes interesadas e intereses:
- Profesor y a los alumnos les interesa ya que es el metodo con el que se tomara asistencia

## Breve descripción
El caso de uso muestra como se registrara la asistencia mediante la lectura NFC de las tarjetas de Movilidad Integrada de la CDMX

## Precondiciones
1. El profesor debe estar dado de alta en el sistema
2. El Alumno debe estar dado de alta en el sistema con su tarjeta

## Flujo normal de eventos
1. El Profesor Inicia Sesion en el sistema 
2. El profesor selecciona la opción "Registrar Asistencia" desde la interfaz principal.
3. El sistema activa la función de lectura NFC para la asistencia.
4. Los alumnos acercan la tarjeta de Movilidad Integrada de la CDMX al celular.
5. El sistema lee la tarjeta y registra la asistencia del alumno.
6. Se muestra una confirmación visual de la asistencia registrada.
7. Se mandara la asistencia a una base de datos para generar el informe.

## Subflujo-1
Registro Manual de Asistencia:
1. En caso de falla en la lectura NFC, el profesor puede optar por registrar la asistencia manualmente.
2. Ingresa el identificador único del alumno o selecciona al alumno de una lista.
3. Confirma la asistencia y el sistema actualiza la base de datos.


## Excepciones
arjeta No Reconocida:

1. Si la tarjeta NFC no es reconocida, se muestra un mensaje de error.
2. Se ofrece la opción de intentar nuevamente o usar el registro manual.
