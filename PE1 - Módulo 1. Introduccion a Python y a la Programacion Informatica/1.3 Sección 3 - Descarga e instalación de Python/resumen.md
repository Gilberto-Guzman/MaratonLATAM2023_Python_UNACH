# 1.3.1 Comienza tu viaje con Python

## Cómo obtener Python y cómo llegar a usarlo

Esta sección es opcional, ya que a lo largo del curso podrá iniciar, probar y experimentar con todos sus programas de Python en **Edube Interactive TM**, el entorno de programación que tenemos. integrado con la plataforma de aprendizaje y estos recursos de estudio. Aún así, si puedes descargar e instalar Python en tu máquina local, lo recomendamos enfáticamente.

- **Windows**: https://www.python.org/downloads/
  **Linux**: sudo apt install python
- Nota: Si usas linux, es posible que ya tengas preinstalado linux, para comprobarlo utiliza este comando: python --version

# 1.3.2 Cómo descargar, instalar y configurar Python

Si eres un **usuario de Windows**, utiliza el archivo .exe descargado y sigue todos los pasos. Deja las configuraciones predeterminadas que el instalador sugiere por ahora, con una excepción: observa la casilla de verificación denominada **Agregar Python 3.x a PATH** y selecciónala.

Si eres un **usuario de macOS**, es posible que ya se haya preinstalado una versión de Python 2 en tu computadora, pero como estaremos trabajando con Python 3, aún deberás descargar e instalar el archivo .pkg correspondiente desde el sitio de Python.

# 1.3.3 Comenzando tu trabajo con Python

Para comenzar tu trabajo, necesitas las siguientes herramientas:

- Un **editor** que te ayudará a escribir el código (debe tener algunas características especiales, no disponibles en herramientas simples); este editor dedicado te dará más que el equipo estándar del sistema operativo.

- Una **consola** en la que puedas ejecutar tu código recién escrito y detenerlo por la fuerza cuando se sale de control.

- Una herramienta llamada **depurador**, capaz de ejecutar tu código paso a paso y te permite inspeccionarlo en cada momento de su ejecución.

Además de sus muchos componentes útiles, la instalación estándar de Python 3 contiene una aplicación muy simple pero extremadamente útil llamada IDLE.
**IDLE** es un acrónimo de: Integrated Development and Learning Environment (Desarrollo Integrado y Entorno de Aprendizaje).

# 1.3.4 Tu primer programa antes de tu primer programa...

El primer paso es crear un nuevo archivo fuente y llenarlo con el código. Haz clic en _File_ en el menú del IDLE y selecciona _New File_.

Haz clic en _File_ (en la nueva ventana), luego haz clic sobre _Save as_ ... , selecciona una carpeta para el nuevo archivo (el escritorio es un buen lugar para tus primeros intentos de programación) y elige un nombre para el nuevo archivo.

Ahora solo coloca una línea en tu ventana de editor recién abierta y con nombre.

La línea se ve así:

    print("Hisssssss...")

Guarda el archivo (File -> Save) y ejecuta el programa (Run -> Run Module).

# 1.3.5 Cómo estropear y arreglar tu código

- El **traceback** (que es la ruta que recorre el código a través de diferentes partes del programa; puedes ignorarlo por ahora, ya que está vacío en un código tan simple).

- La **ubicación del error** (el nombre del archivo que contiene el error, el número de línea y el nombre del módulo); nota: el número puede ser engañoso, ya que Python suele mostrar el lugar donde notó por primera vez los efectos del error, no necesariamente el error en sí.

- El **contenido de la línea errónea**; nota: la ventana del editor de IDLE no muestra números de línea, pero muestra la ubicación actual del cursor en la esquina inferior derecha; utilízalo para localizar la línea errónea en un código fuente largo.

- El **nombre del error** y una breve explicación.

Experimenta con crear nuevos archivos y ejecutando tu código. Intenta mostrar un mensaje diferente en la pantalla, por ejemplo, roar!, miau, o incluso tal vez un oink!. Intenta estropear y corregir tu código - mira qué sucede.
