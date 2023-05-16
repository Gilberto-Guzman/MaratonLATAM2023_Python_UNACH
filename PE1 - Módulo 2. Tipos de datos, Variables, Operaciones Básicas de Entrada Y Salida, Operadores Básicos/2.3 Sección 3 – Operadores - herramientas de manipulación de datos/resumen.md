# 2.3.1 Python como una calculadora.

Ahora, se va a mostrar un nuevo lado de la función print(). Ya se sabe que la función es capaz de mostrar los valores de los literales que le son pasados por los argumentos.

De hecho, puede hacer algo más. Observa el siguiente fragmento de código:

    print(2+2)

Deberías de ver el número cuatro. Tómate la libertad de experimentar con otros operadores.

Sin tomar esto con mucha seriedad, has descubierto que Python puede ser utilizado como una calculadora. No una muy útil, y definitivamente no una de bolsillo, pero una calculadora sin duda alguna.

Tomando esto más seriamente, nos estamos adentrado en el terreno de los **operadores** y **expresiones**.

# 2.3.2 Operadores Básicos.

Un **operador** es un símbolo del lenguaje de programación, el cual es capaz de realizar operaciones con los valores.

Se comenzará con los operadores que están asociados con las operaciones aritméticas más conocidas:

    +
    -
    *
    /
    //
    %
    **

El orden en el que aparecen no es por casualidad. Hablaremos más de ello cuando se hayan visto todos.

**Recuerda**: Cuando los datos y operadores se unen, forman juntos **expresiones**. La expresión más sencilla es el literal.

# Exponenciación.

Observa los ejemplos en la ventana del editor:

    print(2 ** 3)
    print(2 ** 3.)
    print(2. ** 3)
    print(2. ** 3.)

Nota: En los ejemplos, los dobles asteriscos están rodeados de espacios, no es obligatorio hacerlo pero hace que el código sea mas **legible**.

Los ejemplos muestran una característica importante de los **operadores numéricos** de Python.

Ejecuta el código y observa cuidadosamente los resultados que arroja. ¿Puedes observar algo?

**Recuerda**: Es posible formular las siguientes reglas con base en los resultados:

Cuando **ambos** ** argumentos son enteros, el resultado es entero, también;
Cuando **al menos un\*\* \*\* argumento es flotante, el resultado también es flotante.

Esta es una distinción importante que se debe recordar.

# Multiplicación.

Un símbolo de \* (asterisco) es un operador de **multiplicación**.

Ejecuta el código y revisa si la regla de entero vs flotante aún funciona.

    print(2 * 3)
    print(2 * 3.)
    print(2. * 3)
    print(2. * 3.)

# División.

Un símbolo de / (diagonal) es un operador de **división**.

El valor después de la diagonal es el **dividendo**, el valor antes de la diagonal es el **divisor**.

Ejecuta el código y analiza los resultados.

    print(6 / 3)
    print(6 / 3.)
    print(6. / 3)
    print(6. / 3.)

Deberías de poder observar que hay una excepción a la regla.

**El resultado producido por el operador de división siempre es flotante**, sin importar si a primera vista el resultado es flotante: 1 / 2, o si parece ser completamente entero: 2 / 1.

¿Esto ocasiona un problema? Sí, en ocasiones se podrá necesitar que el resultado de una división sea entero, no flotante.

Afortunadamente, Python puede ayudar con eso.

# División entera.

Un símbolo de // (doble diagonal) es un operador de división entera. Difiere del operador estándar / en dos detalles:

- El resultado carece de la parte fraccionaria, está ausente (para los enteros), o siempre es igual a cero (para los flotantes); esto significa que los resultados siempre son redondeados;
- Se ajusta a la regla entero vs flotante.

Ejecuta el ejemplo debajo y observa los resultados:

    print(6 // 3)
    print(6 // 3.)
    print(6. // 3)
    print(6. // 3.)

Como se puede observar, una división de entero entre entero da un **resultado entero**. Todos los demás casos producen flotantes.

Hagamos algunas pruebas mas avanzadas.

Observa el siguiente fragmento de código:

    print(6 // 4)
    print(6. // 4)

El resultado de la división entera siempre se redondea al valor entero inferior mas cercano del resultado de la división no redondeada.

Esto es muy importante: **el redondeo siempre va hacia abajo**.

    print(-6 // 4)
    print(6. // -4)

Nota: Algunos de los valores son negativos. Esto obviamente afectara el resultado. ¿Pero cómo?

El resultado es un par de dos negativos. El resultado real (no redondeado) es -1.5 en ambo casos. Sin embargo, los resultados se redondean. El **redondeo se hace hacia el valor inferior entero**, dicho valor es -2, por lo tanto los resultados son: -2 y -2.0.

Note  
La division entera también se le suele llamar en inglés **floor division**. Más adelante te cruzarás con este término.

# Residuo (módulo).

El siguiente operador es uno muy peculiar, porque no tiene un equivalente dentro de los operadores aritméticos tradicionales.

Su representación gráfica en Python es el símbolo de % (porcentaje), lo cual puede ser un poco confuso.

Piensa en el como una diagonal (operador de división) acompañado por dos pequeños círculos.

El resultado de la operación es el **residuo que queda de la división entera**.

En otras palabras, es el valor que sobra después de dividir un valor entre otro para producir un resultado entero.

Nota: el operador en ocasiones también es denominado **módulo** en otros lenguajes de programación.

Observa el fragmento de código – intenta predecir el resultado y después ejecútalo:

    print(14 % 4)

Como puedes observar, el resultado es dos. Esta es la razón:

- 14 // 4 da como resultado un 3 → esta es la parte entera, es decir el cociente;
- 3 \* 4 da como resultado 12 → como resultado de la multiplicación entre el cociente y el divisor;
- 14 - 12 da como resultado 2 → este es el residuo.

El siguiente ejemplo es un poco más complicado:

# Como no dividir.

Como probablemente sabes, la **división entre cero no funciona**.

**No** intentes:

Dividir entre cero;
Realizar una división entera entre cero;
Encontrar el residuo de una división entre cero.

# Suma.

El símbolo del operador de **suma** es el + (signo de más), el cual esta completamente alineado a los estándares matemáticos.

De nuevo, observa el siguiente fragmento de código:

    print(-4 + 4)
    print(-4. + 8)

# El operador de resta, operadores unarios y binarios.

El símbolo del operador de **resta** es obviamente - (el signo de menos), sin embargo debes notar que este operador tiene otra función - **puede cambiar el signo de un número**.

Esta es una gran oportunidad para mencionar una distinción muy importante entre operadores **unarios** y **binarios**.

En aplicaciones de resta, **el operador de resta espera dos argumentos**: el izquierdo (un **minuendo** en términos aritméticos) y el derecho (un **sustraendo**).

Por esta razón, el operador de resta es considerado uno de los operadores binarios, así como los demás operadores de suma, multiplicación y división.

Pero el operador negativo puede ser utilizado de una forma diferente - observa la ultima línea de código del siguiente fragmento:

    print(-4 - 4)
    print(4. - 8)
    print(-1.1)

Por cierto: también hay un operador + unario. Se puede utilizar de la siguiente manera:

    print(+2)

# 2.3.3 Operadores y sus prioridades.

Hasta ahora, se ha tratado cada operador como si no tuviera relación con los otros. Obviamente, dicha situación tan simple e ideal es muy rara en la programación real.

También, muy seguido encontrarás más de un operador en una expresión, y entonces esta presunción ya no es tan obvia.

Considera la siguiente expresión:

2 + 3 \* 5

Probablemente recordarás de la escuela que las **multiplicaciones preceden a las sumas**.

Seguramente recordarás que primero se debe multiplicar 3 por 5, mantener el 15 en tu memoria y después sumar el 2, dando como resultado el 17.

El fenómeno que causa que algunos operadores actúen antes que otros es conocido como la **jerarquía de prioridades**.

Python define la jerarquía de todos los operadores, y asume que los operadores de mayor jerarquía deben realizar sus operaciones antes que los de menor jerarquía.

Entonces, si se sabe que la \* tiene una mayor prioridad que la +, el resultado final debe de ser obvio.

# Operadores y sus enlaces.

El **enlace** de un operador determina el orden en que se computan las operaciones de los operadores con la misma prioridad, los cuales se encuentran dentro de una misma expresión.

La mayoría de los operadores de Python tienen un enlazado hacia la izquierda, lo que significa que el cálculo de la expresión es realizado de izquierda a derecha.

Este simple ejemplo te mostrará como funciona. Observa:

    print(9 % 6 % 2)

Existen dos posibles maneras de evaluar la expresión:

- De izquierda a derecha: primero 9 % 6 da como resultado 3, y entonces 3 % 2 da como resultado 1;
- De derecha a izquierda: primero 6 % 2 da como resultado 0, y entonces 9 % 0 causa **un error fatal**.

Ejecuta el ejemplo y observa lo que se obtiene:

    print(9 % 6 % 2)

El resultado debe ser 1. El operador tiene un enlazado del lado izquierdo. Pero hay una excepción interesante.

Repite el experimento, pero ahora con exponentes.

Utiliza este fragmento de código:

    print(2 ** 2 ** 3)

Los dos posibles resultados son:

2 ** 2 → 4; 4 ** 3 → 64
2 ** 3 → 8; 2 ** 8 → 256

Ejecuta el código, ¿Qué es lo que observas?

El resultado muestra claramente que **el operador de exponenciación utiliza enlazado del lado derecho**.

Esto contiene una excepción interesante. Si el operador de exponenciación usa el enlazado del lado derecho, ¿puedes adivinar el resultado del siguiente fragmento?

    print(-3 ** 2) print(-2 ** 3) print(-(3 ** 2))

-9
-8
-9

# Lista de prioridades.

Como eres nuevo a los operadores de Python, no se presenta por ahora una lista completa de las prioridades de los operadores.

En lugar de ello, se mostrarán solo algunos, y se irán expandiendo conforme se vayan introduciendo operadores nuevos.

Observa la siguiente tabla:

Prioridad Operador

1. \*\_
2. +, - (nota: los operadores unarios a la derecha del operador exponencial enlazan con mayor fuerza.) unario
3. \_, /, //, %
4. +, - binario

Nota: se han enumerado los operadores en orden **de la más alta (1) a la más baja (4) prioridad**.

Intenta solucionar la siguiente expresión:
print(2 \* 3 % 5)

# Operadores y paréntesis.

Por supuesto, se permite hacer uso de **paréntesis**, lo cual cambiará el orden natural del cálculo de la operación.

De acuerdo con las reglas aritméticas, **las sub-expresiones dentro de los paréntesis siempre se calculan primero**.

Se pueden emplear tantos paréntesis como se necesiten, y seguido son utilizados para **mejorar la legibilidad** de una expresión, aun si no cambian el orden de las operaciones.

Un ejemplo de una expresión con múltiples paréntesis es la siguiente:
print((5 _ ((25 % 13) + 100) / (2 _ 13)) // 2)

10.0

# 2.3.4 RESUMEN DE SECCIÓN.

# Puntos Clave

1. Una **expresión** es una combinación de valores (o variables, operadores, llamadas a funciones, aprenderás de ello pronto) las cuales son evaluadas y dan como resultado un valor, por ejemplo, 1 + 2.

2. Los **operadores** son símbolos especiales o palabras clave que son capaces de operar en los valores y realizar operaciones matemáticas, por ejemplo, el _ multiplica dos valores: x _ y.

3. Los operadores aritméticos en Python: + (suma), - (resta), _ (multiplicación), / (división clásica: regresa un flotante siempre), % (módulo: divide el operando izquierdo entre el operando derecho y regresa el residuo de la operación, por ejemplo, 5 % 2 = 1), ** (exponenciación: el operando izquierdo se eleva a la potencia del operando derecho, por ejemplo, 2 ** 3 = 2 _ 2 \* 2 = 8), // (división entera: retorna el número resultado de la división, pero redondeado al número entero inferior más cercano, por ejemplo, 3 // 2.0 = 1.0)

4. Un operador **unario** es un operador con solo un operando, por ejemplo, -1, o +3.

5. Un operador **binario** es un operador con dos operandos, por ejemplo, 4 + 5, o 12 % 5.

6. Algunos operadores actúan antes que otros, a esto se le llama - **jerarquía de prioridades**:

- El operador \*\* (exponencial) tiene la prioridad más alta;
- Posteriormente los operadores unarios + y - (nota: los operadores unarios a la derecha del operador exponencial enlazan con mayor fuerza, por ejemplo 4 \*\* -1 es igual a 0.25)
- Después \_, /, //, y %,
- Finalmente, la prioridad más baja: los operadores binarios + y -. 7. Las sub-expresiones dentro de paréntesis siempre se calculan primero, por ejemplo, 15 - 1 \_ ( 5 \*( 1 + 2 ) ) = 0.

7. Las sub-expresiones dentro de **paréntesis** siempre se calculan primero, por ejemplo, 15 - 1 _ ( 5 _( 1 + 2 ) ) = 0.

8. Los operadores de **exponenciación** utilizan **enlazado del lado derecho**, por ejemplo, 2 ** 2 ** 3 = 256.
