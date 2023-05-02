# 2.1.1 Tu primer programa

Observa la línea de código de abajo:

    print("¡Hola, Mundo!")

Como puedes ver, el primer programa consta de las siguientes partes:

La palabra print;
Un paréntesis de apertura;
Una comilla;
Una línea de texto: ¡Hola, Mundo!;
Otra comilla;
Un paréntesis de cierre.
Cada uno de los elementos anteriores juega un papel muy importante en el

La palabra _**print**_ que puedes ver aquí es el **nombre de una función**. Eso no significa que dondequiera que aparezca esta palabra, será siempre el nombre de una función. El significado de la palabra proviene del contexto en el cual se haya utilizado la palabra.

Una función (en este contexto) es una parte separada del código de computadora el cual es capaz de:

- **Causar algún efecto** (por ejemplo, enviar texto a la terminal, crear un archivo, dibujar una imagen, reproducir un sonido, etc.); esto es algo completamente inaudito en el mundo de las matemáticas.

- **Evaluar un valor** (por ejemplo, la raíz cuadrada de un valor o la longitud de un texto dado) y **devolverlo como el resultado de la función**, esto es lo que hace que las funciones de Python sean parientes de los conceptos matemáticos.

## ¿De dónde provienen las funciones?

- De **Python mismo**: La función print es una de este tipo; dicha función es un valor agregado de Python junto con su entorno (está **integrada**); no tienes que hacer nada especial (por ejemplo, pedirle a alguien algo) si quieres usarla.

- De **módulos**: Llamados complementos, algunos de los módulos vienen con Python, otros pueden requerir una instalación por separado - cual sea el caso, todos deben estar conectados explícitamente con el código (te mostraremos cómo hacer esto pronto).

- De tu **código**: Puedes **escribirlas tú mismo**, colocando tantas funciones como desees y necesites dentro de su programa para hacerlo más simple, claro y elegante.

El nombre de la función debe ser **significativo** (el nombre de la función print es evidente) imprime en la terminal.

Si vas a utilizar alguna función ya existente, no podrás modificar su nombre, pero cuando comiences a escribir tus propias funciones, debes considerar cuidadosamente la elección de nombres.

# 2.1.3 Argumentos de funciones

Como se dijo anteriormente, una función puede tener:

- Un efecto;
- Un resultado.

También existe un tercer componente de la función, muy importante - el o los argumento(s).

Las funciones matemáticas usualmente toman un argumento. por ejemplo, sen(x) toma una x, que es la medida de un ángulo.

Las funciones de Python, por otro lado, son más versátiles. Dependiendo de las necesidades individuales, pueden aceptar cualquier cantidad de argumentos - tantos como sea necesario para realizar sus tareas. Nota: Cuando dijimos _cualquier número_, eso incluye el cero - algunas funciones de Python no necesitan ningún argumento.

A pesar del número de argumentos necesarios o proporcionados, las funciones de Python demandan fuertemente la presencia de **un par de paréntesis** - el de apertura y de cierre, respectivamente.

Si deseas entregar uno o más argumentos a una función, colócalos **dentro de los paréntesis**. Si vas a utilizar una función que no tiene ningún argumento, aún tiene que tener los paréntesis.

Nota: para distinguir las palabras comunes de los nombres de funciones, coloca un **par de paréntesis vacíos** después de sus nombres, incluso si la función correspondiente requiere uno o más argumentos. Esta es una medida estándar.

## Una cadena como el argumento de la función print()

El único argumento entregado a la función print() en este ejemplo es una cadena:

    print("¡Hola, Mundo!")

Como puedes ver, la **cadena está delimitada por comillas** - de hecho, las comillas forman la cadena, recortan una parte del código y le asignan un significado diferente.

Casi cualquier cosa que ponga dentro de las comillas se tomará de manera literal, no como código, sino como **datos**.

# 2.1.4 Invocación de funciones

El nombre de la función (_**print**_ en este caso) junto con los paréntesis y los argumento(s), forman la **invocación de la función**.

    print("¡Hola, Mundo!")

## ¿Qué sucede cuando Python encuentra una invocación como la que está a continuación?

    function_name(argument)

Veamos:

- Primero, Python comprueba si el nombre especificado es **legal** (explora sus datos internos para encontrar una función existente del nombre; si esta búsqueda falla, Python aborta el código).

- En segundo lugar, Python comprueba si los requisitos de la función para el número de argumentos **le permiten invocar** la función de esta manera (por ejemplo, si una función específica exige exactamente dos argumentos, cualquier invocación que entregue solo un argumento se considerará errónea y abortará la ejecución del código).

- Tercero, Python **deja el código por un momento** y salta dentro de la función que se desea invocar; por lo tanto, también toma los argumento(s) y los pasa a la función.

- Cuarto, la función **ejecuta el código**, provoca el efecto deseado (si lo hubiera), evalúa el (los) resultado(s) deseado(s) y termina la tarea;

- Finalmente, Python **regresa al código** (al lugar inmediatamente después de la invocación) y reanuda su ejecución.

# 2.1.5 LAB Trabajando con la función print()

## Escenario

El comando print(), el cual es una de las directivas más sencillas de Python, simplemente imprime una línea de texto en la pantalla.

En tu primer laboratorio:

- Utiliza la función print() para imprimir la linea ¡Hola, Mundo! en la pantalla. Usa comillas dobles alrededor de la cadena.

- Habiendo hecho eso, usa la función print() nuevamente, pero esta vez imprime tu nombre.

- Elimina las comillas dobles y ejecuta tu código. Mira la reacción de Python. ¿Qué tipo de error arroja?

- Luego, elimina los paréntesis, vuelve a colocar las comillas dobles y ejecuta tu código nuevamente. ¿Qué tipo de error arroja esta vez?

- Experimenta todo lo que puedas. Cambia las comillas dobles a comillas simples, usa múltiples funciones print() en la misma línea, y luego en diferentes líneas. Mira qué pasa.

  # Solución Muestra

  print("¡Hola, Python!")

  # print("Greg")

  # print(Greg)

  # print"Greg"

  # print('Greg')

  # print("Greg") print("Python")

  # ...</sampleSolution>

# 2.1.6 La función print() y su efecto, argumentos, y valores retornados.

Hay que responder a tres preguntas importantes lo antes posible:

**1. ¿Qué efecto tiene la función print()?**

El efecto es muy útil y muy espectacular. La función:

- Toma sus argumentos (puede aceptar más de un argumento y también puede aceptar menos de un argumento).

- Los convierte a un formato legible si es necesario (como puedes sospechar, las cadenas no requieren esta acción, ya que la cadena ya es legible).

- Y envía los datos resultantes al dispositivo de salida (normalmente la consola); en otras palabras, todo lo que pongas en la función print() se aparecerá en tu pantalla.

No es de extrañar entonces que, de ahora en adelante, utilices print() muy intensamente para ver los resultados de sus operaciones y evaluaciones.

**2. ¿Qué argumentos espera print()?**

Cualquiera. Pronto te mostraremos que print() puede operar con prácticamente todos los tipos de datos que ofrece Python. Cadenas, números, caracteres, valores lógicos, objetos - cualquiera de estos se puede pasar con éxito a print().

**3. ¿Qué valor devuelve la función print()?**

Ninguno. Su efecto es suficiente.

# 2.1.7 Instrucciones.

La sintaxis de Python es bastante específica en esta área. A diferencia de la mayoría de los lenguajes de programación, Python requiere que **no haya más de una instrucción por línea**.

Una línea puede estar vacía (por ejemplo, puede no contener ninguna instrucción) pero no debe contener dos, tres o más instrucciones. Esto está estrictamente prohibido.

Nota: Python hace una excepción a esta regla - permite que una instrucción se extienda por más de una línea (lo que puede ser útil cuando el código contiene construcciones complejas).

Vamos a expandir el código un poco, puedes verlo en el editor. Ejecútalo y observa lo que aparece en la consola.

    print("La Witsi Witsi Araña subió a su telaraña.")
    print("Vino la lluvia y se la llevó.")

Esta es una buena oportunidad para hacer algunas observaciones:

- El programa **invoca a la función print() dos veces**, y puedes ver dos líneas separadas en la consola - esto significa que print() comienza su salida desde una nuevalínea cada vez que comienza su ejecución; puedes cambiar este comportamiento, pero también puedes usarlo a tu favor.

- Cada invocación de print() contiene una cadena diferente, como su argumento, y el contenido de la consola lo refleja - esto significa que **las instrucciones en el código se ejecutan en el mismo orden** en el que se han colocado en el archivo fuente; no se ejecuta ninguna instrucción posterior hasta que se completa la anterior (hay algunas excepciones a esta regla, pero puede ignorarlas por ahora.)

Hemos cambiado un poco el ejemplo - hemos agregado una invocación vacía de la función print(). La llamamos vacía porque no hemos entregado ningún argumento a la función.

Puedes verlo en la ventana del editor. Ejecuta el código.

¿Qué sucede?

    print("La Witsi Witsi Araña subió a su telaraña.")
    print()
    print("Vino la lluvia y se la llevó.")

Como puedes ver, la invocación vacía de print() no está tan vacía como podrías haber esperado - genera una línea vacía o (esta interpretación también es correcta) genera una nuevalínea.

Esta no es la única forma de producir una **nuevalínea** en la consola de salida. Ahora le mostraremos otra manera.

# 2.1.8 Caracteres de escape y nueva línea en Python

Hemos modificado el código de nuevo. Obsérvalo con cuidado.

Hay dos cambios muy sutiles - hemos insertado un par extraño de caracteres dentro del texto. Se ven así: \n.

    print("La Witsi Witsi Araña\nsubió a su telaraña.")
    print()
    print("Vino la lluvia\ny se la llevó.")

Curiosamente, mientras **puedes ver dos caracteres, Python ve uno.**

La barra invertida (\) tiene un significado muy especial cuando se usa dentro de cadenas - se llama **carácter de escape**.

La palabra _escape_ debe entenderse específicamente - significa que la serie de caracteres en la cadena se escapa por un momento (un momento muy breve) para introducir una inclusión especial.

En En otras palabras, la barra invertida no significa nada en sí misma, sino que es solo una especie de anuncio de que el siguiente carácter después de la barra invertida también tiene un significado diferente.

La la letra n colocada después de la barra invertida proviene de la palabra _newline_.

Tanto la barra invertida como n forman un símbolo especial llamado **un carácter de nuevalínea**, que insta a la consola a iniciar una **nuevalínea de salida**.

Como se puede observar, aparecen dos nuevas líneas en la canción infantil, en los lugares donde se ha utilizado \n.

Esta convención tiene dos consecuencias importantes:

1. Si deseas colocar solo una barra invertida dentro de una cadena, no olvides su naturaleza de escape - tienes que duplicarla. Por ejemplo, una invocación como esta provocará un error:

print("\")

mientras que esta no lo hará:

print("\\")

2. No todos los pares de escape (la barra invertida junto con otro carácter) significan algo.

# 2.1.9 Usando múltiples argumentos.
