# 2.5.1 Comentarios – ¿por qué, cuándo, y dónde?

Un texto insertado en el programa el cual es, **omitido en la ejecución**, es denominado un **comentario**.

¿Cómo se colocan este tipo de comentarios en el código fuente? Tiene que ser hecho de cierta manera para que Python no intente interpretarlo como parte del código.

Cuando Python se encuentra con un comentario en el programa, el comentario es completamente transparente - desde el punto de vista de Python, el comentario es solo un espacio vacío, sin importar que tan largo sea.

En Python, un comentario es un texto que comienza con el símbolo # y se extiende hasta el final de la línea.

Si se desea colocar un comentario que abarca varias líneas, se debe colocar este símbolo en cada línea. Justo como en el siguiente código:

    # Este programa evalúa la hipotenusa c.
    # a y b son las longitudes de los cátetos.
    a = 3.0
    b = 4.0
    c = (a ** 2 + b ** 2) ** 0.5  # Se emplea ** en lugar de una raíz cuadrada.
    print("c =", c)

Los desarrolladores buenos y responsables **describen cada pieza importante de código**, por ejemplo, el explicar el rol de una variables. Aunque la mejor manera de comentar una variable es dándole un nombre que no sea ambiguo.

Por ejemplo, si una variable determinada esta diseñada para almacenar el área de un cuadrado, el nombre square_area será muchísimo mejor que aunt_jane.

El nombre dado a la variable se puede definir como **auto-comentable**.

# 2.5.2 Marcar fragmentos de código.

Los comentarios pueden ser útiles en otro aspecto - se pueden utilizar para **marcar un fragmento de código que actualmente no se necesita**, cual sea la razón. Observa el siguiente ejemplo, sí se **descomenta** la línea resaltada, esto afectara la salida o resultado del código:

    # Este es un programa de prueba.
    x = 1
    y = 2
    # y = y + x
    print(x + y)

Esto es frecuentemente realizado cuando se esta probando un programa, con el fin de aislar un fragmento de código donde posiblemente se encuentra un error.

https://codersfree.com/posts/comentar-descomentar-varias-lineas-visual-studio-code

Si deseas comentar o descomentar rápidamente varias línea(s) de código, selecciona las líneas que deseas modificar y utiliza el siguiente método abreviado de teclado: CTRL + / (Windows) or CMD + / (Mac OS). Es un truco muy útil, ¿no? Ahora experimenta con el código en el editor.

    # uncomment_me = 1
    # uncomment_me_too = 3
    # uncomment_me_also = 5

    print(uncomment_me, uncomment_me_too, uncomment_me_also, sep="\n")

# 2.5.3 LAB Comentarios.

# Escenario

El código en el editor contiene comentarios. Intenta mejorarlo: agrega o quita comentarios donde consideres que sea apropiado (en ocasiones el remover un comentario lo hace mas legible), y cambia el nombre de las variables donde consideres que esto mejorará la comprensión del código.

Nota  
Los comentarios son muy importantes. No solo hacen que el programa sea **más fácil de entender**, pero también sirven para **deshabilitar aquellas partes de código que no son necesarias** (por ejemplo, cuando se necesita probar cierta parte del código, e ignorar el resto). Los buenos programadores **describen** cada parte importante del código, y dan **nombres significativos** a variables, debido a que en ocasiones es mucho más sencillo dejar el comentario dentro del código mismo.

Es bueno utilizar nombres de variables **legibles**, y en ocasiones es mejor **dividir el código** en partes con nombres (por ejemplo en funciones). En algunas situaciones, es una buena idea escribir los pasos de como se realizaron los cálculos de una forma sencilla y clara.

Una cosa mas: puede ocurrir que un comentario contenga una pieza de información incorrecta o errónea - ¡nunca se debe de hacer eso a propósito!

    # este programa calcula los segundos en cierto número de horas determinadas

    hours = 2  # número de horas
    seconds = 3600  # número de segundos en una hora

    print("Horas: ", hours)
    print("Horas en segundos: ", hours * seconds)

    print("adios")

# 2.5.4 RESUMEN DE SECCIÓN.

1.  Los comentarios pueden ser utilizados para colocar información adicional en el código. Son omitidos al momento de la ejecución. Dicha información es para los lectores que están manipulando el código. En Python, un comentario es un fragmento de texto que comienza con un #. El comentario se extiende hasta el final de la línea.

2.  Si deseas colocar un comentario que abarque varias líneas, es necesario colocar un # al inicio de cada línea. Además, se puede utilizar un comentario para marcar un fragmento de código que no es necesario en el momento y no se desea ejecutar. (observa la última línea de código del siguiente fragmento), por ejemplo:

        # Este programa imprime
        # una introducción en la pantalla.
        print("¡Hola!")  #Invocando a la función print()
        # print("Soy Python.")

3.  Cuando sea posible, se deben **auto comentar los nombres** de las variables, por ejemplo, si se están utilizando dos variables para almacenar la altura y longitud de algo, los nombres length y width son una mejor elección que myvar1 y myvar2.

4.  Es importante utilizar los comentarios para que los programas sean más fáciles de entender, además de emplear variables legibles y significativas en el código. Sin embargo, es igualmente importante **no utilizar** nombres de variables que sean confusos, o dejar comentarios que contengan información incorrecta.

5.  Los comentarios pueden ser muy útiles cuando tú estás leyendo tu propio código después de un tiempo (es común que los desarrolladores olviden lo que su propio código hace), y cuando otros están leyendo tu código (les puede ayudar a comprender que es lo que hacen tus programas y como es que lo hacen).
