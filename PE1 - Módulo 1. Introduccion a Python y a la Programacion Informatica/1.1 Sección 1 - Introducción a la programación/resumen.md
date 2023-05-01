# 1.1.1 ¿Cómo funciona un programa de computadora?

Las computadoras contemporáneas **solo pueden evaluar los resultados de operaciones muy fundamentales**, como sumar o dividir, pero pueden hacerlo muy rápido y pueden repetir estas acciones prácticamente cualquier cantidad de veces. Esto quiere decir, que para realizar casi cualquier accion, **se le debe instruir previamente a la computadora**.

# 1.1.2 Lenguajes naturales vs lenguajes de programación.

Las computadoras también tienen su propio lenguaje, llamado **lenguaje máquina**, el cual responde sólo a un conjunto predeterminado de comandos conocidos.

Un conjunto completo de comandos conocidos se llama **lista de instrucciones**, a veces abreviada **IL** (por sus siglas en inglés).

Cada día se crean nuevas palabras y desaparecen las viejas. Estos lenguajes se llaman **lenguajes naturales**.

# 1.1.3 ¿Qué compone a un lenguaje?

Podemos decir que cada lenguaje (máquina o natural, no importa) consta de los siguientes elementos:

- Alfabeto: Un conjunto de **símbolos** utilizados para formar palabras de un determinado lenguaje (por ejemplo, el alfabeto latino para el inglés, el alfabeto cirílico para el ruso, el kanji para el japonés, y así sucesivamente).

- Léxico: (también conocido como diccionario) un conjunto de **palabras** que el lenguaje ofrece a sus usuarios (por ejemplo, la palabra "computadora" proviene del diccionario en inglés, mientras que "cmoptrue" no; la palabra "chat" está presente en los diccionarios de inglés y francés, pero sus significados son diferentes)

- Sintaxis: un conjunto de **reglas** (formales o informales, escritas o interpretadas intuitivamente) utilizadas para precisar si una determinada cadena de palabras forma una **oración válida** (por ejemplo, "Soy una serpiente" es una frase sintácticamente correcta, mientras que "Yo serpiente soy una" no lo es)

- Sémantica: un conjunto de **reglas** que determinan **si una frase tiene sentido** (por ejemplo, "Me comí una dona" tiene sentido, pero "Una dona me comió" no lo tiene)

# 1.1.4 Lenguaje máquina vs. lenguaje de alto nivel.

**El IL es, de hecho, el alfabeto de un lenguaje máquina**. Este es el conjunto de símbolos más simple y primario que podemos usar para dar comandos a una computadora. Es la lengua materna de la computadora.

Estos lenguajes a menudo se denominan **lenguajes de programación de alto nivel**. Son al menos algo similares a los naturales en que usan símbolos, palabras y convenciones legibles para los humanos. Estos lenguajes permiten a los humanos expresar comandos a las computadoras que son mucho más complejos que los que ofrecen las IL.

Un programa escrito en un lenguaje de programación de alto nivel se denomina **código fuente** ( en contraste con el código máquina ejecutado por las computadoras). Del mismo modo, el archivo que contiene el código fuente se denomina **archivo fuente**.

# 1.1.5 Compilación vs. Interpretación.

Hay dos formas diferentes de transformar un programa de un lenguaje de programación de alto nivel a un lenguaje de máquina:

- **Compilación**: El programa fuente se traduce una vez (sin embargo, este acto debe repetirse cada vez que se modifique el código fuente) al obtener un archivo (por ejemplo, un .exe si el código está destinado a ejecutarse en MS Windows) que contiene el código máquina. Ahora se puede distribuir el archivo en todo el mundo; el programa que realiza esta traducción se llama **compilador** o **traductor**.

- **Interpretación**: Tú o cualquier usuario del código puede traducir el programa fuente cada vez que se debe ejecutar. El programa que realiza este tipo de transformación se denomina **intérprete**, ya que interpreta el código cada vez que se pretende ejecutar. También significa que no puedes simplemente distribuir el código fuente tal cual, porque el usuario final también necesita el intérprete para ejecutarlo.

# 1.1.6 ¿Qué hace el intérprete?

El intérprete lee el código fuente de la forma habitual en la cultura occidental: de arriba a abajo y de izquierda a derecha. Hay algunas excepciones: se cubrirán más adelante en el curso.

En primer lugar, el intérprete verifica si todas las líneas posteriores son correctas (utilizando los cuatro aspectos cubiertos anteriormente).

Si el compilador encuentra un error, finaliza el trabajo inmediatamente. El único resultado en este caso es un mensaje de error. El intérprete te informará dónde se encuentra el error y qué lo causó. Sin embargo, estos mensajes pueden ser engañosos, ya que el intérprete no puede seguir tus intenciones exactas y puede detectar errores a cierta distancia de sus causas reales.

# 1.1.7 Compilación vs. Interpretación – Ventajas y Desventajas

## Ventajas.

Compilación.

- La ejecución del código traducido suele ser más rápida.
- Solo el usuario debe tener el compilador, el usuario final puede usar el código sin él.
- El código traducido se almacena usando lenguaje máquina, como es muy difícil de entender, es probable que tus propios inventos y trucos de programación sigan siendo tu secreto.

Interpretación.

- Puedes ejecutar el código tan pronto como lo completes, no hay fases adicionales de traducción.

- El código se almacena usando un lenguaje de programación, no un lenguaje máquina; esto significa que se puede ejecutar en computadoras que usan diferentes lenguajes máquina; no compila tu código por separado para cada arquitectura diferente.

## Desventajas.

Compilación

- La compilación en sí puede ser un proceso que consume mucho tiempo, es posible que no puedas ejecutar su código inmediatamente después de realizar una modificación.
- Debes tener tantos compiladores como plataformas de hardware donde desees que se ejecute tu código.

Interpretación.

- No esperes que la interpretación acelere tu código a alta velocidad: tu código compartirá el poder de la computadora con el intérprete, por lo que no puede ser realmente rápido.
- Tanto tu como el usuario final deben tener el intérprete para ejecutar tu código.

## ¿Qué significa todo esto para ti?

- Python es un **lenguaje interpretado**. Esto significa que hereda todas las ventajas y desventajas descritas. Por supuesto, agrega algunas de sus características únicas a ambos conjuntos.
- Si deseas programar en Python, necesitarás el **intérprete de Python**. No podrás ejecutar tu código sin él. Afortunadamente, **Python es gratuito**. Esta es una de sus ventajas más importantes.
- Por razones históricas, los lenguajes diseñados para ser utilizados en la interpretación a menudo se denominan **lenguajes de scripting**, mientras que la fuente los programas codificados con ellos se denominan **scripts**. Bien, conozcamos a Python.
