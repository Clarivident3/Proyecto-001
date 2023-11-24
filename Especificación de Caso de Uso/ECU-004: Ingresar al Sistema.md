# ID
- UC - 004

# Caso de uso
- Ingresar al Sistema

## Actores
- Usuarios

## Tipo
- Primario

## Partes interesadas e intereses:
- Usuarios

## Breve descripción
El caso de uso muestra como ingresar al sistema

## Precondiciones
1. El sistema esta instalado y en funcionamiento
2. El usuario esta dado de alta ademas tiene usuario y contraseña
   
## Flujo normal de eventos
1. El usuario abre la aplicación.
2. La pantalla de inicio de sesión se presenta al usuario.
3. El usuario ingresa su nombre de usuario y contraseña.
4. El sistema valida las credenciales ingresadas.
5. Si las credenciales son válidas, el usuario accede al sistema.
6. Se carga la interfaz principal del usuario con las funciones y datos asociados.

## Subflujo-1

- Recuperación de Contraseña:
  1. El usuario selecciona la opción de "Olvidé mi contraseña".
  2. El sistema solicita la dirección de correo electrónico asociada a la cuenta.
  3. El sistema envía un enlace de restablecimiento de contraseña al correo electrónico proporcionado.
  4. El usuario sigue el enlace y establece una nueva contraseña.


## Excepciones
- Credenciales Inválidas:
     1. Si las credenciales ingresadas no son válidas, se muestra un mensaje de error.
     2. Se brinda la opción de intentar nuevamente o recuperar la contraseña.

- Problemas de Conexión:
  1. Si hay problemas de conexión durante el inicio de sesión, se muestra un mensaje indicando la dificultad de conexión.
  2. Se sugiere intentar nuevamente más tarde y, si persisten los problemas, contactar al soporte técnico.
