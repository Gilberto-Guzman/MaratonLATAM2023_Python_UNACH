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

    print("Greg")

    print(Greg)

    print"Greg"

    print('Greg')

    print("Greg") print("Python")

    ...</sampleSolution>

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

# 2.1.8 Caracteres de escape y nueva línea en Python.

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

También vale la pena intentar alimentar a la función print() con más de un argumento.

    print("La Witsi Witsi Araña" , "subió" , "a su telaraña.")

Hay una invocación de la función print(), pero contiene **tres argumentos**. Todos ellos son cadenas.

Los argumentos están **separados por comas**. Los hemos rodeado de espacios para hacerlos más visibles, pero no es realmente necesario, y no lo haremos más.

En este caso, las comas al separar los argumentos juega un papel completamente diferente al de la coma dentro de la cadena. El primero es parte de la sintaxis de Python, mientras que el segundo está diseñado para mostrarse en la consola.

La función print() invocada con más de un argumento los **muestra todos en una sola línea**.
La función print() **pone un espacio entre los argumentos de salida** por iniciativa propia.

# 2.1.10 Argumentos posicionales.

Ahora que sabes un poco sobre las costumbres de la función print(), te mostraremos cómo cambiarlas.

Deberías poder predecir la salida sin ejecutar el código en el editor.

    print("Mi nombre es", "Python.")
    print("Monty Python.")

La forma en que estamos pasando los argumentos a la función print() es la más común en Python, y se llama **la forma posicional**. Este nombre proviene del hecho de que el significado del argumento está dictado por su posición (por ejemplo, el segundo argumento se mostrará después del primero, no al revés).

# 2.1.11 Argumentos de palabra clave.

El mecanismo se llama **argumentos de palabras clave**. El nombre proviene del hecho de que el significado de estos argumentos se toma no de su ubicación (posición) sino de la palabra especial (palabra clave) utilizada para identificarlos.

La función print() tiene dos argumentos de palabra clave que puedes usar para tus propósitos. El primero se llama end.

    print("Mi nombre es", "Python.", end=" ")
    print("Monty Python.")

Para usarlo, es necesario conocer algunas reglas:

- Un argumento de palabra clave consta de tres elementos: una **palabra clave** se identifica el argumento (end aquí); un **signo de igual** (=); y un **valor** asignado a ese argumento.
- Cualquier argumento de palabra clave debe colocarse **después del último argumento posicional** (esto es muy importante).

Y ahora es el momento de intentar algo más difícil.

Si miras con atención, verás que hemos usado el argumento end, pero la cadena que se le asignó está vacía (no contiene ningún carácter).

¿Qué sucederá ahora? Ejecuta el programa en el editor para averiguarlo.

    print("Mi nombre es ", end="")
    print("Monty Python.")

Como el argumento end se ha establecido a nada, la función print() tampoco genera nada, una vez que se han agotado sus argumentos posicionales.

El **argumento de palabra clave** que puede hacer esto se denomina sep (como en separador).

Mira el código en el editor, y ejecútalo.
print("Mi", "nombre", "es", "Monty", "Python.", sep="-")

Ambos argumentos de palabra clave pueden **mezclarse en una invocación**, como aquí en la ventana del editor.

    print("Mi", "nombre", "es", sep="\_", end="_")
    print("Monty", "Python.", sep="_", end="\*\n")

# 2.1.12 LAB La función print() y sus argumentos.

# Escenario

Modifica la primera línea de código en el editor, usando las palabras claves reservadas sep y end, para que se obtenga la salida esperada. Emplea dos funciones print() en el editor.

No cambies nada en la segunda invocación del print().
print("Programming","Essentials","in", sep="\*\*\*", end="...")
print("Python")

# 2.1.13 LAB Dando formato a la salida.

# Escenario

Te recomendamos encarecidamente que juegues con el código que hemos escrito para y realiza algunos (quizás incluso destructivos) cambios. Siéntete libre de modificar cualquier parte del código, pero hay una condición - aprende de tus errores y saca tus propias conclusiones.

Intenta:

- Minimizar el número de invocaciones de la función print() insertando \n en las cadenas.

- Hacer que la flecha sea el doble de grande (pero mantener las proporciones)

- Duplica la flecha, colocando ambas flechas una al lado de la otra; nota: una cadena se puede multiplicar usando el siguiente truco: "string" \* 2 producirá "stringstring" (pronto contaremos más al respecto).

- Elimina cualquiera de las comillas y observe detenidamente la respuesta de Python; presta atención a dónde Python ve un error - ¿es este el lugar donde realmente existe el error?

- Haz lo mismo con algunos de los paréntesis.

- Cambia cualquiera de las palabras print por otra cosa, que difiera solo en mayúsculas y minúsculas (por ejemplo, Print) - qué sucede ahora?

- Reemplaza algunas de las comillas con apóstrofes; observa lo que sucede con cuidado.

# Sample Solution

    ###################
    print("original version:")
    ###################
    print("    *")
    print("   * *")
    print("  *   *")
    print(" *     *")
    print("***   ***")
    print("  *   *")
    print("  *   *")
    print("  *****")
    ###################
    print("with fewer 'print()' invocations:")
    ###################
    print("    *\n   * *\n  *   *\n *     *\n***   ***")
    print("  *   *\n  *   *\n  *****")
    ###################
    print("higher:")
    ###################
    print("        *")
    print("       * *")
    print("      *   *")
    print("     *     *")
    print("    *       *")
    print("   *         *")
    print("  *           *")
    print(" *             *")
    print("******     ******")
    print("     *     *")
    print("     *     *")
    print("     *     *")
    print("     *     *")
    print("     *     *")
    print("     *     *")
    print("     *******")
    ###################
    print("doubled:")
    ###################
    print("        *        "*2)
    print("       * *       "*2)
    print("      *   *      "*2)
    print("     *     *     "*2)
    print("    *       *    "*2)
    print("   *         *   "*2)
    print("  *           *  "*2)
    print(" *             * "*2)
    print("******     ******"*2)
    print("     *     *     "*2)
    print("     *     *     "*2)
    print("     *     *     "*2)
    print("     *     *     "*2)
    print("     *     *     "*2)
    print("     *     *     "*2)
    print("     *******     "*2)

# 2.1.14 RESUMEN DE SECCIÓN.

1. La función print() es una función integrada imprime/envía un mensaje específico a la pantalla/ventana de consola.

2. Las funciones integradas, al contrario de las funciones definidas por el usuario, están siempre disponibles y no tienen que ser importadas. Python 3.7.1 viene con 69 funciones incorporadas. Puedes encontrar su lista completa en orden alfabético en Python Standard Library. https://docs.python.org/3/library/functions.html

3. Para llamar a una función (invocación de función), debe utilizarse el nombre de la función seguido de un paréntesis. Puedes pasar argumentos a una función colocándolos dentro de los paréntesis. Se deben separar los argumentos con una coma, por ejemplo, print("¡Hola,", "Mundo!"). Una función print() "vacía" imprime una línea vacía a la pantalla.

4. Las cadenas de Python están delimitadas por comillas, por ejemplo, "Soy una cadena" (comillas dobles), o 'Yo soy una cadena, también' (comillas simples).

5. Los programas de computadora son colecciones de instrucciones. Una instrucción es un comando para realizar una tarea específica cuando se ejecuta, por ejemplo, para imprimir un determinado mensaje en la pantalla.

6. En las cadenas de Python la barra diagonal inversa (\) es un carácter especial que anuncia que el siguiente carácter tiene un significado diferente, por ejemplo, \n (el carácter de nuevalínea) comienza una nuevalínea de salida.

7. Los argumentos posicionales son aquellos cuyo significado viene dictado por su posición, por ejemplo, el segundo argumento se emite después del primero, el tercero se emite después del segundo, etc.

8. Los argumentos de palabra clave son aquellos cuyo significado no está dictado por su ubicación, sino por una palabra especial (palabra clave) que se utiliza para identificarlos.

9. Los parámetros end y sep se pueden usar para dar formato la salida de la función print(). El parámetro sep especifica el separador entre los argumentos emitidos. Por ejemplo, print("H", "E", "L", "L", "O", sep="-"), mientras que el parámetro end especifica que imprimir al final de la declaración de impresión.
