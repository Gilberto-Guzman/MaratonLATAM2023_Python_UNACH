# 2.2.1 Literales - los datos en sí mismos.

**Un literal se refiere a datos cuyos valores están determinados por el literal mismo.**

Y esta es la pista: 123 es un literal, y c no lo es.

Se utilizan literales **para codificar datos y ponerlos dentro del código.** Ahora mostraremos algunas convenciones que se deben seguir al utilizar Python.

    print("2")
    print(2)

A través de este ejemplo, encuentras dos tipos diferentes de literales:

- Una **cadena**, la cual ya conoces,
- Y un número **entero**, algo completamente nuevo.

La función print() los muestra exactamente de la misma manera - Sin embargo, internamente, la memoria de la computadora los almacena de dos maneras completamente diferentes - La cadena existe como eso solo una cadena - una serie de letras.

El número es convertido a una representación máquina (una serie de bits). La función print() es capaz de mostrar ambos en una forma legible para humanos.

# 2.2.2 Enteros.

Se puede afirmar que todos los números manejados por las computadoras modernas son de dos tipos:

- Enteros, es decir, aquellos que no tienen una parte fraccionaria.
- Y números punto-flotantes (o simplemente flotantes), los cuales contienen (o son capaces de contener) una parte fraccionaría.

La característica del valor numérico que determina el tipo, rango y aplicación se denomina el **tipo**.

Si se codifica un literal y se coloca dentro del código de Python, la forma del literal determina la representación (tipo) que Python utilizará para almacenarlo en la memoria.

Es claro que la separación hace que sea más fácil de leer, especialmente cuando el número tiene demasiados dígitos. Sin embargo, Python no acepta estas cosas, está **prohibido**. ¿Qué es lo que Python permite?. El uso de **guion bajo** en los literales numéricos.\*

Por lo tanto, el número se puede escribir ya sea así: 11111111, o como sigue: 11_111_111.

**Nota** \*Python 3.6 ha introducido el guion bajo en los literales numéricos, permitiendo colocar un guion bajo entre dígitos y después de especificadores de base para mejorar la legibilidad. Esta característica no está disponible en versiones anteriores de Python.

¿Cómo se codifican los números negativos en Python? Como normalmente se hace, agregando un signo de **menos**. Se puede escribir: -11111111, o -11_111_111.

Los números positivos no requieren un signo positivo antepuesto, pero es permitido, si se desea hacer. Las siguientes líneas describen el mismo número: +11111111 y 11111111.

# Números octales y hexadecimales.

Existen dos convenciones adicionales en Python que no son conocidas en el mundo de las matemáticas. El primero nos permite utilizar un número en su representación **octal**.

Si un número entero esta precedido por un código 0O o 0o (cero-o), el número será tratado como un valor octal. Esto significa que el número debe contener dígitos en el rango del [0..7] únicamente.

0o123 es un número **octal** con un valor (decimal) igual a 83.

La función print() realiza la conversión automáticamente. Intenta esto:

    print(0o123)

La segunda convención nos permite utilizar números en **hexadecimal**. Dichos números deben ser precedidos por el prefijo 0x o 0X (cero-x).

0x123 es un número **hexadecimal** con un valor (decimal) igual a 291. La función print() puede manejar estos valores también. Intenta esto:

    print(0x123)

# 2.2.3 Flotantes.

Ahora es tiempo de hablar acerca de otro tipo, el cual esta designado para representar y almacenar los números que (como lo diría un matemático) tienen una parte decimal no vacía.

Son números que tienen (o pueden tener) una parte fraccionaria después del punto decimal, y aunque esta definición es muy pobre, es suficiente para lo que se desea discutir.

Cuando se usan términos como dos y medio o menos cero punto cuatro, pensamos en números que la computadora considera como números punto-flotante:

    2.5
    -0.4

Nota: dos punto cinco se ve normal cuando se escribe en un programa, sin embargo si tu idioma nativo prefiere el uso de una coma en lugar de un punto, se debe asegurar que **el número no contenga comas**.

Pero no hay que olvidar esta sencilla regla - se puede omitir el cero cuando es el único dígito antes del punto decimal.

En esencia, el valor 0.4 se puede escribir como:

.4

Por ejemplo: el valor de 4.0 puede ser escrito como:

4.

Esto no cambiará su tipo ni su valor.

# Enteros vs Flotantes

El punto decimal es esencialmente importante para reconocer números punto-flotantes en Python.

Observa estos dos números:

    4
    4.0

Se puede pensar que son idénticos, pero Python los ve de una manera completamente distinta.

4 es un número **entero** mientras que 4.0 es un número **punto-flotante**.

El punto decimal es lo que determina si es flotante.

Por otro lado, no solo el punto hace que un número sea flotante. Se puede utilizar la letra e.

Cuando se desea utilizar números que son muy pequeños o muy grandes, se puede implementar la **notación científica**.

Por ejemplo, la velocidad de la luz, expresada en metros por segundo. Escrita directamente se vería de la siguiente manera: 300000000.

Para evitar escribir tantos ceros, los libros de texto emplean la forma abreviada, la cual probablemente hayas visto: 3 x 108.

Se lee: tres por diez elevado a la octava potencia.

En Python, el mismo efecto puede ser logrado de una manera similar - observa lo siguiente:

    3E8

La letra E (también se puede utilizar la letra minúscula e - proviene de la palabra **exponente**) la cual significa por diez a la n potencia.

Nota:

- El **exponente** (el valor después de la E) debe ser un valor entero;
- La **base** (el valor antes de la E) puede ser un valor entero o flotante.

# Codificando Flotantes

Veamos ahora como almacenar números que son muy pequeños (en el sentido de que están muy cerca del cero).

Una constante de física denominada La Constante de Planck (denotada como h), de acuerdo con los libros de texto, tiene un valor de: **6.62607 x 10-34**.

Si se quisiera utilizar en un programa, se debería escribir de la siguiente manera:

6.62607E-34

Nota: el hecho de que se haya escogido una de las posibles formas de codificación de un valor flotante no significa que Python lo presentará de la misma manera.

Python podría en ocasiones elegir una notación diferente.

# 2.2.4 Cadenas

Las cadenas se emplean cuando se requiere procesar texto (como nombres de cualquier tipo, direcciones, novelas, etc.), no números.

Ya conoces un poco acerca de ellos, por ejemplo, que **las cadenas requieren comillas** así como los flotantes necesitan punto decimal.

Supongamos que se desea mostrar un muy sencillo mensaje:

Me gusta "Monty Python"

¿Cómo se puede hacer esto sin generar un error? Existen dos posibles soluciones.

La primera se basa en el concepto ya conocido del **carácter de escape**, el cual recordarás se utiliza empleando la **diagonal invertida**. La diagonal invertida puede también escapar de la comilla. Una comilla precedida por una diagonal invertida cambia su significado - no es un limitador, simplemente es una comilla. Lo siguiente funcionará como se desea:

    print("Me gusta \"Monty Python\"")

La segunda solución puede ser un poco sorprendente. Python puede utilizar **una apóstrofe en lugar de una comilla**. Cualquiera de estos dos caracteres puede delimitar una cadena, pero para ello se debe ser consistente.

Si se delimita una cadena con una comilla, se debe cerrar con una comilla.

Si se inicia una cadena con un apóstrofe, se debe terminar con un apóstrofe.

Este ejemplo funcionará también:

    print('Me gusta "Monty Python"')

Nota: en este ejemplo no se requiere nada de escapes.

# Codificando Cadenas.

Ahora, la siguiente pregunta es: ¿Cómo se puede insertar un apóstrofe en una cadena la cual está limitada por dos apóstrofes?

A estas alturas ya se debería tener una posible respuesta o dos.

Intenta imprimir una cadena que contenga el siguiente mensaje:

I'm Monty Python.

¿Sabes cómo hacerlo? Haz clic en Revisar a continuación para ver si tenías razón:

print('I\'m Monty Python.')
print("I'm Monty Python.")

Como se puede observar, la diagonal invertida es una herramienta muy poderosa - puede escapar no solo comillas, sino también apóstrofes.

Ya se ha mostrado, pero se desea hacer énfasis en este fenómeno una vez mas: **una cadena puede estar vacía** - puede no contener carácter alguno.

Una cadena vacía sigue siendo una cadena:

''
""

# 2.2.5 Valores Booleanos.

Para concluir con los literales de Python, existen dos más.

No son tan obvios como los anteriores y se emplean para representar un valor muy abstracto - **la veracidad**.

Cada vez que se le pregunta a Python si un número es más grande que otro, el resultado es la creación de un tipo de dato muy específico - **un valor booleano**.

El nombre proviene de George Boole (1815-1864), el autor de Las Leyes del Pensamiento, las cuales definen el **Álgebra Booleana** - una parte del álgebra que hace uso de dos valores: True y False, denotados como 1 y 0.

Python, es entonces, un reptil **binario**.

Estos dos valores booleanos tienen denotaciones estrictas en Python:

True
False

No se pueden cambiar - se deben tomar estos símbolos como son, incluso respetando **las mayúsculas y minúsculas**.

# 2.2.6 LAB Literales de Python - Cadenas.

Escenario
Escriba un fragmento de código de una línea, utilizando la función print(), así como los caracteres de nuevalínea y de escape, para que coincida con el resultado esperado que se muestra en la salida.

Salida Esperada
"Estoy"
""aprendiendo""
"""Python"""

# 2.2.7 RESUMEN DE SECCIÓN.

1. Los **literales** son notaciones para representar valores fijos en el código. Python tiene varios tipos de literales - es decir, un literal puede ser un número por ejemplo, 123), o una cadena (por ejemplo, "Yo soy un literal.").

2. El **sistema binario** es un sistema numérico que emplea 2 como su base. Por lo tanto, un número binario está compuesto por 0s y 1s únicamente, por ejemplo, 1010 es 10 en decimal.

Los sistemas de numeración Octales y Hexadecimales son similares pues emplean 8 y 16 como sus bases respectivamente. El sistema hexadecimal utiliza los números decimales más seis letras adicionales.

3. Los **enteros** (o simplemente **int**) son uno de los tipos numéricos que soporta Python. Son números que no tienen una parte fraccionaria, por ejemplo, 256, o -1 (enteros negativos).

4. Los números **punto-flotante** (o simplemente **flotantes**) son otro tipo numérico que soporta Python. Son números que contienen (o son capaces de contener) una parte fraccionaria, por ejemplo, 1.27.

5. Para codificar un apóstrofe o una comilla dentro de una cadena se puede utilizar el carácter de escape, por ejemplo, 'I\'m happy.', o abrir y cerrar la cadena utilizando un conjunto de símbolos distintos al símbolo que se desea codificar, por ejemplo, "I'm happy." para codificar un apóstrofe, y 'El dijo "Python", no "typhoon"' para codificar comillas.

6. Los valores booleanos son dos objetos constantes True y False empleados para representar valores de verdad en contextos numéricos 1 es True, mientras que 0 es False.

Extra

Existe un literal especial más utilizado en Python: el literal **None**. Este literal es llamado un objeto de NoneType, y puede ser utilizado para representar **la ausencia de un valor**. Pronto se hablará más acerca de ello.
