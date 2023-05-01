# 1.2.1 Python - una herramienta, no un reptil.s

## ¿Qué es Python?

Python es un lenguaje de programación de alto nivel, interpretado, orientado a objetos y de uso generalizado con semántica dinámica, que se utiliza para la programación de propósito general.

Python proviene de una vieja serie de comedia de la BBC llamada **Monty Python's Flying Circus**.

# 1.2.2 ¿Quién creó Python?

Python fue creado por **Guido van Rossum**, nacido en 1956 en Haarlem, Países Bajos.

# 1.2.3 Un proyecto de programación por pasatiempo.

Según Guido van Rossum:

En Diciembre de 1989, estaba buscando un proyecto de programación de "pasatiempo" que me mantendría ocupado durante la semana de Navidad. Mi oficina (...) estaría cerrada, pero tenía una computadora en casa y no mucho más en mis manos. Decidí escribir un intérprete para el nuevo lenguaje de scripting en el que había estado pensando últimamente: un descendiente de ABC que atraería a los hackers de Unix/C. Elegí Python como el título de trabajo para el proyecto, estando en un estado de ánimo ligeramente irreverente (y un gran fanático de Monty Python's Flying Circus).

## Los objetivos de Python.

En 1999, Guido van Rossum definió sus objetivos para Python:

Un lenguaje **fácil e intuitivo** tan poderoso como los de los principales competidores.
De **código abierto**, para que cualquiera pueda contribuir a su desarrollo.
El código que es tan **comprensible** como el inglés simple.
**Adecuado para tareas cotidianas**, permitiendo tiempos de desarrollo cortos.

Python no es una lengua joven. **Es maduro y digno de confianza**.
Se ubica en los primeros puestos, como uno de los lenguajes mas utilizados: https://pypl.github.io/PYPL.html

# 1.2.4 ¿Qué hace que Python sea tan especial?

## ¿Por qué Python?

- **Es fácil de aprender**: El tiempo necesario para aprender Python es más corto que en muchos otros lenguajes; esto significa que es posible comenzar la programación real más rápido.

- **Es fácil de enseñar**: La carga de trabajo de enseñanza es menor que la que necesitan otros lenguajes; esto significa que el profesor puede poner más énfasis en las técnicas de programación generales (independientes del lenguaje), no gastando energía en trucos exóticos, extrañas excepciones y reglas incomprensibles.

- **Es fácil de utilizar para escribir software nuevo**: A menudo es posible escribir código más rápido cuando se emplea Python.

- **Es fácil de entender**: A menudo, también es más fácil entender el código de otra persona más rápido si está escrito en Python.

- **Es fácil de obtener, instalar y desplegar**: Python es gratuito, abierto y multiplataforma; no todos los lenguajes pueden presumir de eso.

# 1.2.5 ¿Rivales de Python?

Python tiene dos competidores directos, con propiedades y predisposiciones comparables. Estos son:

- **Perl**: Un lenguaje de scripting originalmente escrito por Larry Wall.
- **Ruby**: Un lenguaje de scripting originalmente escrito por Yukihiro Matsumoto.

El primero es más tradicional, más conservador que Python, y se parece a algunos de los buenos lenguajes antiguos derivados del lenguaje de programación C clásico.

En contraste, este último es más innovador y está más lleno de ideas nuevas. Python se encuentra en algún lugar entre estas dos creaciones.

# 1.2.6 ¿Dónde podemos ver a Python en acción?

Se utiliza ampliamente para implementar complejos **Servicios de Internet** como motores de búsqueda, almacenamiento en la nube y herramientas, redes sociales, etc.

Muchas **herramientas de desarrollo** se implementan en Python. Cada vez se escriben más **aplicaciones de uso diario** en Python. Muchos **científicos** han abandonado las costosas herramientas patentadas y se han cambiado a Python. Muchos **testers** de proyectos de TI han comenzado a usar Python para llevar a cabo procedimientos de prueba repetibles.

# 1.2.7 ¿Por qué no Python?

A pesar de la creciente popularidad de Python, todavía existen algunos nichos en los que Python está ausente o rara vez se ve:

- **Programación de bajo nivel** (a veces llamada programación "cercana al metal"): si deseas implementar un controlador o motor gráfico extremadamente efectivo, no se usaría Python.

- **Aplicaciones para dispositivos móviles**: este territorio aún está a la espera de ser conquistado por Python, lo más probable es que suceda algún día.

# 1.2.8 Existe más de un Python.

## Python 2 vs. Python 3

Python 2 es una versión anterior del Python original. Su desarrollo se ha estancado intencionalmente, aunque eso no significa que no haya actualizaciones. Por el contrario, las actualizaciones se emiten de forma regular, pero no pretenden modificar el idioma de manera significativa. Prefieren arreglar cualquier error recién descubierto y agujeros de seguridad. La ruta de desarrollo de Python 2 ya ha llegado a un callejón sin salida, pero Python 2 en sí todavía está muy vivo.

Python 3 es la versión más nueva (para ser precisos, la actual) del lenguaje. Está atravesando su propio camino de evolución, creando sus propios estándares y hábitos.

**Todos los ejemplos de código que encontrarás durante el curso se han probado con Python 3.4, Python 3.6, Python 3.7, Python 3.8 y Python 3.9.**

# 1.2.9 Implementaciones de Python.

- **Cython**: Es una de las posibles soluciones al rasgo de Python más doloroso - la falta de eficiencia. Los cálculos matemáticos grandes y complejos pueden ser fácilmente codificados en Python (mucho más fácil que en "C" o en cualquier otro lenguaje tradicional), pero la ejecución del código resultante puede requerir mucho tiempo.

- **Jython**: Puede comunicarse con la infraestructura Java existente de manera más efectiva. Es por esto que algunos proyectos lo encuentran útil y necesario.

- **PyPy**: Tepresenta un entorno de Python escrito en un lenguaje similar a Python llamado RPython (Restricted Python). En realidad es un subconjunto de Python.

El código fuente de PyPy no se ejecuta de manera interpretativa, sino que se traduce al lenguaje de programación C y luego se ejecuta por separado.

- **MicroPython**: Es una implementación eficiente de software de código abierto de Python 3 que está optimizada para ejecutarse en **microcontroladores**.

Creado originalmente por **Damien George**, un programador australiano, que en el año 2013 realizó una exitosa campaña en Kickstarter y lanzó la primera versión de MicroPython con una placa de desarrollo con tecnología STM32F4 llamada pyboard.

En 2017, MicroPython se utilizó para crear **CircuitPython**, otro lenguaje de programación de código abierto que se ejecuta en el hardware del microcontrolador, que es un derivado del lenguaje MicroPython.
