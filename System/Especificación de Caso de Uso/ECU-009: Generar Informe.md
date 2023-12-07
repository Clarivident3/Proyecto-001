
# ID
- UC - 008

# Caso de uso
- Generar informe de asistencia

## Actores
- Porofesor

## Tipo
- Primario

## Partes interesadas e intereses:
- Profesor ya que le interesa generar informes de asistencia

## Breve descripción
El caso de uso muestra como se generan los reportes de asistencia.

## Precondiciones
1. El profesor debe estar dado de alta en el sistema.
2. El profesor debe haber accedido al sistema.

## Flujo normal de eventos
1. El usuario selecciona la opción "Generar Informe" desde la interfaz principal.
2. Se presenta un formulario o pantalla que permite al usuario especificar los criterios del informe, como el rango de fechas, el grupo, o el tipo de informe.
3. El usuario configura los criterios según sus necesidades.
4. El sistema realiza consultas a la base de datos para recuperar la información de asistencia relevante.
5. Se genera un informe basado en los criterios especificados.
6. El usuario puede visualizar el informe en la aplicación

## Subflujo-1
Previsualización del Informe
  1. Después de generar el informe, el usuario tiene la opción de previsualizarlo en la aplicación

 Selección de Criterios Detallados:
  1. El usuario puede seleccionar criterios detallados, como alumnos específicos, tipos de asistencia, o grupos particulares.
  2. Estos criterios permiten una personalización más específica del informe.

## Excepciones
Datos Insuficientes para el Informe
     1. Si los criterios especificados por el usuario no generan resultados, se muestra un mensaje indicando la falta de datos.
     2. Se sugiere al usuario ajustar los criterios y volver a intentar.

Error en la Generación del Informe
     1. Si ocurre un error durante la generación del informe, se muestra un mensaje de error.
     2. Se aconseja al usuario intentar nuevamente o contactar al soporte técnico.

Problemas de Previsualización:
     1. Si hay problemas al previsualizar el informe, se muestra un mensaje de advertencia.
