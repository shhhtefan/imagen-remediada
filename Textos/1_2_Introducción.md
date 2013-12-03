Introducción
============
El cuaderno que sostiene entre sus manos es un ejercicio de deconstrucción de las imágenes de las campañas presidenciales de Michelle Bachelet y Evelyn Matthei, donde se descomponen imágenes al punto de hacer casi irreconocible su discurso original y, a partir de ello, se configuran nuevas interpretaciones.

Se utilizan dos herramientas para este proceso: diseño generativo y código computacional. El diseño generativo es una metodología relativamente nueva utilizada en disciplinas diversas como diseño, arquitectura y ciencias de computación. A diferencia de otras metodologías, el diseño generativo se enfoca principalmente en los procesos emergentes y en la exploración de posibilidades. Las definiciones de esta metodología están fuertemente relacionadas con la computación, por lo que muchas veces se emplea un lenguaje de programación (o código) para crear los procesos. Para efectos de este libro se utilizó un lenguaje enfocado en disciplinas visuales, conocido como _Processing_.
>Nota: En este cuaderno, código computacional hace referencia a un lenguaje de programación y suele usarse como sinónimo del concepto de _software_; el _software_ es código.
>Nota: Para saber más sobre _Processing_, hay una breve introducción en la sección 2.1.

Un ejercicio de este tipo no está limitado a estas herramientas y podría prescindir de ellas sin complicaciones. Sin embargo, estas presentan un potencial para disciplinas visuales como el diseño gráfico, particularmente porque el diseño generativo propone un cambio de paradigma[citar GD]: dejar de depender exclusivamente de las _cajas negras_, es decir, herramientas gráficas pre-construidas y hacerse cargo del proceso mismo de creación de imágenes; nos invita a condicionar el proceso generativo.

> Nota: El diseño generativo no nos obliga a usar exclusivamente lenguajes de programación. Grupos como _Conditional Design_, por ejemplo, codifican sus procesos haciendo uso de elementos análogos: pintura, lápices, personas. El diseño generativo no elimina herramientas tradicionales como Adobe Photoshop, más bien presenta una guía de acciones perfectamente compatibles con este tipo de _software_ u otras formas de producción visual.

Otro factor a favor del _software_, es que esta se ha vuelto un pilar para un gran conjunto de actividades profesionales. En realidad, la tecnología es parte integral del mundo profesional, pues permea todas nuestras actividades y condiciona nuestra interacción con el entorno. 

Las imágenes, en todas sus formas, también están mediadas, pero no sólo por la tecnología. Las imágenes para las campañas aquí analizadas están condicionadas por la perspectiva de cada candidata y el conglomerado político que representan. Ambas campañas hacen uso de un imaginario de la sociedad y, por primera vez en nuestra historia, estamos frente a dos representaciones de la mujer chilena, provenientes de proyectos políticos opuestos.

Todas las imágenes de las campañas fueron creadas con una intención, pero además fueron producidas con _software_; editores de imágenes, editores audiovisuales, procesadores de video, etc. Pareció natural, entonces, tratar de _re-mediar_ las imágenes con la ayuda de un lenguaje de programación. 

El cuaderno está dividido en 2 partes: _setup_ y _draw._ En _setup_ se establecen las variables que sirven de fundación para el ejercicio de deconstrucción; por variables me refiero al contexto de las imágenes, su origen, el criterio de selección, etc. _Draw_, en cambio, compone el grueso de este cuaderno, y presenta las imágenes descompuestas según los tres aspectos principales del modelo de color HSB: matiz (_hue_), saturación y brillo. 
>Nota: _setup_ y _draw_ son conceptos utilizados en _Processing_. _Setup_ se utiliza para organizar todos los parámetros inicales, necesarios para la ejecución del _software_, y sólo se inicia una vez. _Draw_ es el segmento que ejecuta el código en tiempo real y se repite una y otra vez hasta que el _software_ es terminado. Es también el cuerpo principal de un _software_ escrito en _Processing_. 

>Nota: Todo el material utilizado para la producción de este cuaderno, incluyendo los _software_ y las maquetas iniciales, están disponibles en https://github.com/stepetri/imagen-remediada.

Este ejercicio es sólo una breve introducción a la reflexión sobre la producción de imágenes, pero espero que cualquier persona con afinidad por la visualidad vea algo de interés en estas páginas. Además de ser un ejercicio de deconstrucción, este cuaderno es una invitación a detenerse y pensar cómo vemos las imágenes, particularmente aquellas mediadas por la tecnología.


