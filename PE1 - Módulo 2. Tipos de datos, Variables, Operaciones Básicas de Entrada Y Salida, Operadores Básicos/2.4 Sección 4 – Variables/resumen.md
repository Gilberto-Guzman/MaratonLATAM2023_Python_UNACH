# 2.4.1 Variables – cajas con forma de datos.

Python ayudará con ello. Python ofrece "cajas" (o "contenedores") especiales para este propósito, estas cajas son llamadas **variables** ‒ el nombre mismo sugiere que el contenido de estos contenedores puede variar en casi cualquier forma.

¿Cuáles son los componentes o elementos de una variable en Python?

- Un nombre.
- Un valor (el contenido del contenedor).

# 2.4.2 Nombres de Variables.

Si se desea **nombrar una variable**, se deben seguir las siguientes reglas:

- El nombre de la variable debe de estar compuesto por MAYÚSCULAS, minúsculas, dígitos, y el carácter \_ (guion bajo).
- El nombre de la variable debe comenzar con una letra.
- El carácter guion bajo es considerado una letra.
- Las mayúsculas y minúsculas se tratan de forma distinta (un poco diferente que en el mundo real - Alicia y ALICIA son el mismo nombre, pero en Python son dos nombres de variable distintos, subsecuentemente, son dos variables diferentes).
- El nombre de las variables no pueden ser igual a alguna de las palabras reservadas de Python (las palabras clave - explicará más de esto pronto).

Nota que la misma restricción aplica a los nombres de funciones.

Python no impone restricciones en la longitud de los nombres de las variables, pero eso no significa que un nombre de variable largo sea mejor que uno corto.

Python te permite usar no solo letras latinas sino también caracteres específicos de idiomas que usan otros alfabetos.

El PEP 8 -- Style Guide for Python Code recomienda la siguiente convención de nomenclatura para variables y funciones en Python:

https://peps.python.org/pep-0008/

- Los nombres de las variables deben estar en minúsculas, con palabras separadas por guiones bajos para mejorar la legibilidad (por ejemplo, var, my_variable)

- Los nombres de las funciones siguen la misma convención que los nombres de las variables (por ejemplo, fun, my_function)

- También es posible usar letras mixtas (por ejemplo, myVariable), pero solo en contextos donde ese ya es el estilo predominante, para mantener la compatibilidad retroactiva con la convención adoptada.

# Palabras Clave.

Observa las palabras que juegan un papel muy importante en cada programa de Python.

['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']

Son llamadas **palabras clave** o (mejor dicho) **palabras clave reservadas**. Son reservadas porque **no se deben utilizar como nombres**: ni para variables, ni para funciones, ni para cualquier otra cosa que se desee crear.

El significado de la palabra reservada está **predefinido**, y no debe cambiar.

Afortunadamente, debido al hecho de que Python es sensible a mayúsculas y minúsculas, cualquiera de estas palabras se pueden modificar cambiando una o varias letras de mayúsculas a minúsculas o viceversa, creando una nueva palabra, la cual no esta reservada.

Por ejemplo - **no se puede nombrar** a la variable así:

import

No se puede tener una variable con ese nombre - esta prohibido. pero se puede hacer lo siguiente:

Import

Estas palabras podrían parecer un misterio ahorita, pero pronto se aprenderá acerca de su significado.

# 2.4.3 Cómo crear una variable.

¿Qué se puede poner dentro de una variable?

Cualquier cosa.

Se puede utilizar una variable para almacenar cualquier tipo de los valores que ya se han mencionado, y muchos mas de los cuales aun no se han explicado.

El valor de la variable en lo que se ha puesto dentro de ella. Puede variar tanto como se necesite o requiera. El valor puede ser entero, después flotante, y eventualmente ser una cadena.

Hablemos de dos cosas importantes - **como son creadas las variables**, y **como poner valores dentro de ellas** (o mejor dicho, como dar o **pasarles valores**).

RECUERDA  
**Una variable se crea cuando se le asigna un valor**. A diferencia de otros lenguajes de programación, no es necesario declararla.

Si se le asigna cualquier valor a una variable no existente, la variable será **automáticamente creada**. No se necesita hacer algo más.

La creación (o su sintaxis) es muy simple: **solo utiliza el nombre de la variable deseada, después el signo de igual (=) y el valor que se desea colocar dentro de la variable**.

Observa el fragmento en el editor:
var = 1
print(var)

Consiste de dos simples instrucciones:

- La primera crea una variable llamada var, y le asigna un literal con un valor entero de 1.
- La segunda imprime el valor de la variable recientemente creada en la consola.

Como puedes ver, print() tiene otro lado: también puede manejar variables. ¿Sabes cuál será el resultado del fragmento? Ejecuta el código para verificar.

# 2.4.4 Cómo emplear una variable.

Se tiene permitido utilizar cuantas declaraciones de variables sean necesarias para lograr el objetivo del programa, por ejemplo:

    var = 1
    account_balance = 1000.0
    client_name = 'John Doe'
    print(var, account_balance, client_name)
    print(var)

Sin embargo, **no se permite utilizar una variable que no exista**, (en otras palabras, una variable a la cual no se le ha dado un valor).

Este ejemplo **ocasionará un error**:

    var = 1
    print(Var)

Se ha tratado de utilizar la variable llamada Var, la cual no tiene ningún valor (nota: var y Var son entidades diferentes, y no tienen nada en común dentro de Python).

RECUERDA  
Se puede utilizar print() para combinar texto con variables utilizando el operador + para mostrar cadenas con variables, por ejemplo:

    var = "3.8.5"
    print("Python version: " + var)

# 2.4.5 Cómo asignar un nuevo valor a una variable ya existente.

¿Cómo se le asigna un valor nuevo a una variable que ya ha sido creada? De la misma manera. Solo se necesita el signo de igual.

El signo de igual es de hecho un operador de asignación. Aunque esto suene un poco extraño, el operador tiene una sintaxis simple y una interpretación clara y precisa.

Asigna el valor del argumento de la derecha al de la izquierda, aún cuando el argumento de la derecha sea una expresión arbitraria compleja que involucre literales, operadores y variables definidas anteriormente.

Observa el siguiente código:

    var = 1
    print(var)
    var = var + 1
    print(var)

La primer línea del código **crea una nueva variable** llamada var y le asigna el valor de 1.

La sentencia se lee de la siguiente manera: asigna el valor de 1 a una variable llamada var.

De manera más corta: asigna 1 a var.

Algunos prefieren leer el código así: var se convierte en 1.

La tercera línea **le asigna a la misma variable un nuevo valor** tomado de la variable misma, sumándole 1.Al ver algo así, un matemático probablemente protestaría - ningún valor puede ser igualado a si mismo más uno. Esto es una contradicción. Pero Python trata el signo = no como igual a, sino como asigna un valor.

Entonces, ¿Cómo se lee esto en un programa?

Toma el valor actual de la variable var, sumale 1 y guárdalo en la variable var.

En efecto, el valor de la variable var ha sido incrementado por uno, lo cual no está relacionado con comparar la variable con otro valor.

¿Puedes predecir cuál será el resultado del siguiente fragmento de código?

    var = 100
    var = 200 + 300
    print(var)

# 2.4.6 Resolviendo problemas matemáticos simples.

Ahora deberías poder construir un programa corto que resuelva problemas matemáticos simples como el teorema de Pitágoras:

_El cuadrado de la hipotenusa es igual a la suma de los cuadrados de los catetos._

El siguiente código evalúa la longitud de la hipotenusa (es decir, el lado más largo de un triángulo rectángulo, el opuesto al ángulo recto) usando el teorema de Pitágoras:

    a = 3.0
    b = 4.0
    c = (a ** 2 + b ** 2) ** 0.5
    print("c =", c)

# 2.4.7 LAB Variables.

# Escenario.

A continuación una historia:

Érase una vez en la Tierra de las Manzanas, Juan tenía tres manzanas, María tenía cinco manzanas, y Adán tenía seis manzanas. Todos eran muy felices y vivieron por muchísimo tiempo. Fin de la Historia.

Tu tarea es:

- Crear las variables: john, mary, y adam.
- Asignar valores a las variables. El valor debe de ser igual al número de manzanas que cada quien tenía.
- Una vez almacenados los números en las variables, imprimir las variables en una línea, y separar cada una de ellas con una coma.
- Después se debe crear una nueva variable llamada total_apples y se debe igualar a la suma de las tres variables anteriores.
- Imprime el valor almacenado en total_apples en la consola;
- **Experimenta con tu código**: crea nuevas variables, asigna diferentes valores a ellas, y realiza varias operaciones aritméticas con ellas (por ejemplo, +, -, \*, /, //, etc.). Intenta poner una cadena con un entero juntos en la misma línea, por ejemplo, "Número total de manzanas:" y total_apples.

  john = 3
  mary = 5
  adam = 6

  print(john, mary, adam, sep=',')

  total_apples = john + mary + adam
  print(total_apples)

  # peter = 12.5

  # suzy = 2

  # print(peter / suzy)

  # print("Total number of apples:", total_apples)

# 2.4.8 Operadores Abreviados.

Es tiempo de explicar el siguiente conjunto de operadores que harán la vida del programador/desarrollador más fácil. Muy seguido, se desea utilizar la misma variable al lado derecho y al lado izquierdo del operador = operator.

Por ejemplo, si se necesita calcular una serie de valores sucesivos de la potencia de 2, se puede usar el siguiente código:

    x = x * 2

También, puedes utilizar una expresión como la siguiente si no puedes dormir y estas tratando de resolverlo con alguno de los métodos tradicionales:

    sheep = sheep + 1

Python ofrece una manera más corta de escribir operaciones como estas, lo cual se puede codificar de la siguiente manera:

    x *= 2 sheep += 1

# 2.4.9 LAB Variables: un convertidor simple.

Millas y kilómetros son unidades de longitud o distancia.

Teniendo en mente que 1 milla equivale aproximadamente a 1.61 kilómetros, complementa el programa en el editor para que convierta de:

- Millas a kilómetros;
- Kilómetros a millas.

No se debe cambiar el código existente. Escribe tu código en los lugares indicados con ###. Prueba tu programa con los datos que han sido provistos en el código fuente.

Pon mucha atención a lo que esta ocurriendo dentro de la función print(). Analiza como es que se proveen múltiples argumentos para la función, y como es que se muestra el resultado.

Nota que algunos de los argumentos dentro de la función print() son cadenas (por ejemplo, "millas son", y otros son variables (por ejemplo, miles).

Consejo  
Hay una cosa interesante más que esta ocurriendo. ¿Puedes ver otra función dentro de la función print()? Es la función round(). Su trabajo es redondear la salida del resultado al número de decimales especificados en el paréntesis, y regresar un valor flotante (dentro de la función round() se puede encontrar el nombre de la variable, el nombre, una coma, y el número de decimales que se desean mostrar). Se hablará más de esta función muy pronto, no te preocupes si no todo queda muy claro. Solo se quiere impulsar tu curiosidad.

Después de completar el laboratorio, abre Sandbox, y experimenta más. Intenta escribir diferentes convertidores, por ejemplo, un convertidor de USD a EUR, un convertidor de temperatura, etc. - ¡Deja que tu imaginación vuele! Intenta mostrar los resultados combinando cadenas y variables. Intenta utilizar y experimentar con la función round() para redondear tus resultados a uno, dos o tres decimales. Revisa que es lo que sucede si no se provee un dígito al redondear. Recuerda probar tus programas.

Experimenta, saca tus propias conclusiones, y aprende. Sé curioso.

    kilometers = 12.25
    miles = 7.38

    miles_to_kilometers = miles * 1.61
    kilometers_to_miles = kilometers / 1.61

    print(miles, "millas son", round(miles_to_kilometers, 2), "kilómetros")
    print(kilometers, "kilómetros son", round(kilometers_to_miles, 2), "millas")

# Escenario.

Observa el código en el editor: lee un valor float, lo coloca en una variable llamada x, e imprime el valor de la variable llamada y. Tu tarea es completar el código para evaluar la siguiente expresión:

3x3 - 2x2 + 3x - 1

El resultado debe ser asignado a y.

Recuerda que la notación algebraica clásica muy seguido omite el operador de multiplicación, aquí se debe de incluir de manera explicita. Nota como se cambia el tipo de dato para asegurarnos de que x es del tipo float.

Mantén tu código limpio y legible, y pruébalo utilizando los datos que han sido proporcionados. No te desanimes por no lograrlo en el primer intento. Se persistente y curioso.

Salida de muestra
x = 0
x = 1
x = -1
Salida de muestra
y = -1.0
y = 3.0
y = -9.0

    x = 0
    x = float(x)
    y = 3 * x**3 - 2 * x**2 + 3 * x - 1
    print("y =", y)

    x = 1
    x = float(x)
    y = 3 * x**3 - 2 * x**2 + 3 * x - 1
    print("y =", y)

    x = -1
    x = float(x)
    y = 3 * x**3 - 2 * x**2 + 3 * x - 1
    print("y =", y)

# 2.4.11 RESUMEN DE SECCIÓN.

1. Una **variable** es una ubicación nombrada reservada para almacenar valores en la memoria. Una variable es creada o inicializada automáticamente cuando se le asigna un valor por primera vez. (2.1.4.1)

2. Cada variable debe de tener un nombre único - un **identificador**. Un nombre válido debe ser aquel que no contiene espacios, debe comenzar con un guion bajo(\_), o una letra, y no puede ser una palabra reservada de Python. El primer carácter puede estar seguido de guiones bajos, letras, y dígitos. Las variables en Python son sensibles a mayúsculas y minúsculas.

3. Python es un lenguaje **de tipo dinámico**, lo que significa que no se necesita declarar variables en él. Para asignar valores a las variables, se utiliza simplemente el operador de asignación, es decir el signo de igual (=), por ejemplo, var = 1.

4. También es posible utilizar **operadores de asignación compuesta** (operadores abreviados) para modificar los valores asignados a las variables, por ejemplo: var += 1, o var /= 5 \* 2.

5. Se les puede asignar valores nuevos a variables ya existentes utilizando el operador de asignación o un operador abreviado, por ejemplo:

   var = 2
   print(var)

   var = 3
   print(var)

   var += 1
   print(var)

Puedes combinar texto y variables usando el operador + y emplear la función print() para generar cadenas y variables, por ejemplo:

    var = "007"
    print("Agent " + var)
