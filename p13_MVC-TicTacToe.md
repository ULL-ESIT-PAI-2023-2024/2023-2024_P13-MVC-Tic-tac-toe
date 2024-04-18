# Práctica 13. Modelo Vista Controlador. Tres en Raya
### Esta práctica junto con la anterior constituyen el examen final de la asignatura

### Objetivos
Los objetivos de esta tarea son poner en práctica:
* El diseño de una aplicación conforme al patrón MVC.

* La arquitectura Modelo Vista Controlador
* Conceptos de Programación orientada a eventos en TypeScript.
* Conceptos de Programación Gráfica en TypeScript usando la API Canvas.
* Metodologías y conceptos de Programación Orientada a Objetos en TypeScript.
* Principios y Buenas prácticas de programación Orientada a Objetos.
* El uso de elementos HTML básicos.
* El uso de propiedades de CSS para dotar de estilo a una página web simple.

### Rúbrica de evaluacion del ejercicio
Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva)
que se tendrán en cuenta a la hora de evaluar esta práctica:
* Se valorará la realización de las diferentes tareas que se proponen
* El comportamiento del programa debe ajustarse a lo descrito en este documento
* Capacidad de la programadora de introducir cambios en el programa desarrollado
* Se valorará una correcta implementación del patrón MVC y la conformidad a los principios de la OOP.
* Se acredita conocimiento y puesta en práctica de principios y buenas prácticas de programación orientada a objetos
* Saber corregir bugs en sus programas utilizando el depurador de Visual Studio Code
* Deben usarse estructuras de datos adecuadas para representar los diferentes elementos que intervienen en el problema
* Ser capaz de generar documentación para sus programas TS utilizando
  [TypeDoc](https://typedoc.org/)
  y de visualizar dicha documentación en un servidor web
* Acreditar que conoce las etiquetas de 
  [JSDoc](https://jsdoc.app/)
* Acreditar su capacidad para configurar y utilizar 
  [ESLint](https://eslint.org/)
y que es capaz de trabajar con la misma en Visual Studio Code
* Se comprobará que el código que el alumnado escribe se adhiere a las reglas de las Guías de Estilo de Google para 
[TypeScript](https://google.github.io/styleguide/tsguide.html)
y/o
[JavaScript](https://google.github.io/styleguide/jsguide.html)
* Todas las prácticas realizadas hasta la fecha, incluída la que se presenta para su evaluación, se encuentran alojadas en repositorios privados de GitHub.
* Acreditar que es capaz de editar ficheros de forma remota en su VM usando Visual Studio Code

### Indicaciones de caracter general
* La aplicación que desarrolle ha de ser orientada a objetos.
Ponga en práctica en su desarrollo los fundamentos, principios y buenas prácticas de la OOP así como los
conocimientos que haya adquirido en el uso de patrones de diseño.

* Antes de proceder al desarrollo, tómese el tiempo necesario para identificar objetos, clases, métodos y relaciones entre estas entidades.
A partir de ese primer análisis, diseñe la estructura de clases que utilizará en su programa, 
así como las relaciones existentes entre las mismas.
Desarrolle un diagrama UML para esas clases, que ha de añadir a la página índice de esta práctica.
Asegúrese de la corrección de su diagrama.
Una aplicación para la realización de diagramas UML como
[Mermaid](https://mermaid.live/edit#pako:eNptkU1PwzAMhv9KlBOI9Q9UuyC2SRx22m2KhNzEdFbzAfnQBKP_nbSlYXT4ZD-OX72xL1w6hbzmUkMIG4LWgxGW5Xi0ZECz9VdVsU2S3S3dUTjd0iM2Hv7gmj2QjQxaXOJD9GRb1qJV6K-bw0jYg8np3f2iYSDiDEfbo73LBFgRbRC6J6edL41wJjMP5vI9gezmur_WGz5W9KrBe6BPfLY7xFiwBLuF-O_8uIJfQ41zmlF4OZNWBfpkF7Nz8BU36A2QyncZVQSPJzQoeJ1Tha-QdBRc2D4_TW8q72OrKDrP6-gTrjik6A4fVs719ObnuhPsvwES3pny)
puede resultarle útil para esta finalidad, aunque puede usar cualquier otro programa que conozca, o simplemente papel y bolígrafo.

* Encapsule las clases en módulos que exporten la correspondiete clase hacia otros programas clientes que pudieran utilizarla.

* Utilice un fichero distinto para el código de cada una de las clases que intervienen en su programa.

* Realice, como siempre, un diseño incremental del programa comprobando cada una de las funcionalidades que añade, siguiendo un desarrollo TDD.

* Previo a la implementación de cada clase, diseñe y desarrolle un conjunto de tests para probar el correcto
funcionamiento de todos los métodos públicos.

* Configure adecuadamente ficheros `package.json` y `tsconfig.json` en el directorio raíz de su proyecto que
permitan gestionar las dependencias del mismo.

* Todo el código estará ubicado en el directorio `src` del proyecto. Use subdirectorios de éste si le resulta conveniente.

* Cuando finalice su desarrollo **modifique el fichero `README.md`** de su proyecto incluyendo la información
habitual en cualquier proyecto público en GitHub.
Puede usar este
[README.md](https://github.com/taniarascia/mvc?tab=readme-ov-file)
como referencia pero incluya además de la información que allí se indica, dos apartados,
`### Building and Running the code` y `Live Demo`.
En el primero de ellos ha de explicar en detalle cómo a partir de clonar su repo público ha de compilarse y
ejecutarse su aplicación, mientras que en el segundo ha de incluir un enlace (véase el apartado *Presentación
de resultados* de este documento) a la URL pública donde encontrar su aplicación.

### El juego del tres en raya
Esta es la última práctica de la asignatura en el este curso, y en ella 
se propone desarrollar en TS una aplicación web `tic-tac-toe.ts` conforme al patrón MVC.

El
[Tres en raya](https://en.wikipedia.org/wiki/Tic-tac-toe)
es un simple y conocido juego de lápiz y papel entre dos jugadores: O y X, que marcan alternativamente los espacios vacíos de un tablero de 3x3 casillas.
La aplicación que se propone crear es una versión para que un usuario juegue contra el ordenador.
En 
[esta página](https://playtictactoe.org/)
que se utilizará como referencia, puede Ud. jugar interactivamente.
Consiga que su aplicación sea todo lo similar posible a la de referencia salvo por los banner de 
publicidad de esa página y no incluya en su aplicación ninguna funcionalidad ni elementos de GUI que no estén presentes en la aplicación de referencia.

Diseñe su aplicación web como una SPA
([Single-page application](https://en.wikipedia.org/wiki/Single-page_application))
de modo que el juego se muestre en el viewport del navegador sin necesidad de usar las barras de scroll.

Las diferentes versiones del código disponible en el 
[repositorio de códigos de ejemplo](https://github.com/ULL-ESIT-PAI-2023-2024/PAI-class-code-examples/tree/master/src/T4-Events-TS/tic-tac-toe)
de la asignatura y que se explican en las
[transparencias de las sesiones de teoría](https://docs.google.com/presentation/d/1y8vpt6xbO4julrB6Tn3GeMQT_JoxBpVX24I8XH8qsEc/edit?usp=sharing)
(Case Study: Tic-tac-toe)
pueden serle útil como punto de partida, aunque la aplicación que se propone desarrollar ha de
ser orientada a objetos y conforme al patrón MVC, requisitos que no cumple el código anterior.

Aproveche el desarrollo que se propone para practicar el patrón MVC así como los mecanismos de comunicación
entre clases que se han estudiado en las sesiones de teoría de la asignatura.
Practique también a utilizar elementos básicos de código CSS para dotar de estilos adecuados a su apliación.

### Presentación de resultados
La visualización de la ejecución del programa se realizará a través de una página web alojada
en la máquina IaaS-ULL de la asignatura y cuya URL tendrá la forma:

[1] `http://10.6.129.123:8080/einstein-albert-tic-tac-toe.html`

en la que se incustará un lienzo (canvas) para dibujar las manos de la partida de poker.
Sustituya *Albert Einstein* por su nombre y apellido en la URL de su página
y la dirección IP anterior por la correspondiente a su máquina IaaS.
Coloque en esa página una cabecera con su nombre y apellido.

Utilice código HTML y CSS para lograr una página funcional y visualmente correcta.

Diseñe asimismo otra página HTML simple 

[2] `http://10.6.129.123:8080/index.html`

que sirva de "página índice" para los ejercicios de la sesión de evaluación de la práctica.
La página [1] será uno de los enlaces de [2] y a su vez [1] tendrá un enlace "Home" que apunte a [2].
Enlace también en la página índice [2] la página que contiene la documentación de su proyecto generada con
Typedoc.

Incluya una tercera página

[3] `http://10.6.129.123:8080/uml.html`

que muestre el diagrama UML de las clases que intervienen en su aplicación.

Utilice lo que haya aprendido de CSS para dotar de estilo propio a las páginas HTML que
desarrolle, aunque el CSS es el aspecto de menor importancia en este ejercicio.

**Es importante** para la evaluación de su práctica que, una vez finalizada la sesión de evaluación la página
índice ([2]) de su proyecto esté disponible para ser consultada a través de una URL pública.
Tanto la aplicación que ha desarrollado como ejercicio de la práctica como los ejercicios que haya
desarrollado en la sesión de evaluación han de estar disponibles a través de esa página.

Si esa página no está disponible, la práctica no se podrá evaluar.

Esta referencia
[Runing Node JS Server In Background](https://iulianpopa.ro/nodejs/2021/06/04/running-node-js-server-in-background/)
puede serle útil para hacer que su servidor se ejecute en background y la página esté disponible después de
que Ud. haya cerrado la sesión linux en la máquina IaaS.

## Referencias
* [Modelo-vista-controlador](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller)
* [Trabajo MVC](https://github.com/ULL-ESIT-PAI-2023-2024/2023-2024-pai-mvc-pablo-medina-moreno/tree/master/src/todo-example)
* [Runing Node JS Server In Background](https://iulianpopa.ro/nodejs/2021/06/04/running-node-js-server-in-background/)
* [PAI Code Examples](https://github.com/ULL-ESIT-PAI-2023-2024/PAI-class-code-examples)
* [The Modern Javascript Tutorial](https://javascript.info)
* [Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)
* [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)
* [ESLint](https://eslint.org/)
* [TypeDoc](https://typedoc.org/)
* [JSDoc](https://jsdoc.app/)
