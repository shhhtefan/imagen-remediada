Índice
======
###### 1.1 Manifiesto

###### 1.2 Introducción

###### 1.3 Sujetos de prueba

###### 2.1 Programa

###### 2.2 Deconstrucción

###### 2.3 Observaciones


1.1 Manifiesto
==============

01 // La tecnología condiciona nuestra forma de percibir el entorno.

02 // Las imágenes están mediadas directa o indirectamente por la tecnología.

03 // Todo puede ser re-mediado.


1.2 Introducción
================
El cuaderno que sostiene entre sus manos es un ejercicio de deconstrucción de las campañas presidenciales de Michelle Bachelet y Evelyn Matthei. Se descomponen imágenes al punto de hacer casi irreconocible su discurso original y, a partir de ello, se configuran nuevas interpretaciones.

Se utilizan dos herramientas para este proceso: diseño generativo y código. El diseño generativo es una metodología relativamente nueva utilizada en disciplinas diversas como arquitectura, diseño y ciencias computacionales. A diferencia de otras metodologías, el diseño generativo se enfoca principalmente en los procesos emergentes y en la exploración de posibilidades. Las definiciones de esta metodología están fuertemente relacionadas con la computación, por lo que muchas veces emplea un lenguaje de programación (o código) para crear los procesos. Para efectos de este libro se utilizó un lenguaje enfocado a disciplinas visuales, conocido como* Processing.*

No es la única manera de realizar un ejercicio de este tipo, pero es, a mi parecer, una manera interesante de hacerlo, particularmente porque la programación ya es un pilar de nuestra sociedad. Más bien, la *tecnología* es parte integral de nuestro mundo. Permea todas nuestras actividades y condiciona nuestra interacción con el entorno. Las imágenes, en todas sus formas, también están condicionadas.

Las imágenes para las campañas presidenciales están condicionadas por la perspectiva de cada candidata y el conglomerado político que representan. Ambas campañas hacen uso de un imaginario de la sociedad y por primera vez estamos frente a dos representaciones de la mujer chilena provenientes de dos bandos políticamente opuestos.

Todas estas imágenes fueron creadas con una intención, pero además, fueron creadas con software. Pareció natural, entonces, tratar de re-mediar las imágenes con la ayuda de un lenguaje de programación.

El cuaderno está dividido en 2 partes: *setup* y *draw.* En *setup* se establecen las variables que sirven de fundación para el ejercicio de deconstrucción. Por variables me refiero al origen de las imágenes, el criterio de selección, etc. *Draw*, en cambio, compone el grueso de este libro. Presenta las imágenes decompuestas según los tres aspectos principales del modelo de color HSB: matíz (*hue*), saturación y brillo.

Espero que cualquier persona con cierta afinidad por la visualidad vea algo de interés en este cuaderno. Además de ser un ejercicio de deconstrucción, este cuaderno es una invitación a detenerse y pensar cómo vemos las imágenes.


1.3 Sujetos de prueba
=====================
El conjunto de imágenes seleccionadas para la deconstrucción se basa
principalmente en la contingencia. Por una serie de hechos imprevistos, las
elecciones presidenciales de 2013 son la primera en enfrentar a dos mujeres de
conglomerados políticos opuestos como candidatas a la presidencia.

Esto deja un escenario interesante, pues permite comparar en términos visuales
dos formas de representar a la sociedad y a la mujer chilena en condiciones
prácticamente iguales. Ambas candidaturas hacen uso de los mismos medios en
formatos similares y el contenido de las imágenes tiene un alto grado de
similitud, si bien la forma de presentar los contenidos pueden ser distintos.

Para nutrir más la comparación de las representaciones visuales de ambas
candidatas, hay un tercer exponente, cuya presencia sirve como punto de control
con respecto al discurso de las candidatas. Este tercer exponente debería ser
contemporáneo a las campañas presidenciales y compartir algunos rasgos que
aparecen en las imágenes de las candidatas, pero también debería provenir de un
contexto ajeno a las elecciónes presidenciales. Uno de esos exponentes es
"Soltera Otra Vez", pues nos da una tercera perspectiva sobre cómo se representa
la sociedad y la mujer chilena desde otro contexto.

Con algunas excepciones hacia el final de este cuadernillo, se hizo el intento
de presentar el conjunto de imágenes de forma objetiva e imparcial.

### Bachelet

Candidata de la autodenominada "Nueva Mayoría". En 2006, Michelle Bachelet fue
la segunda mujer en presentarse como candidata a la presidencia y la primera en
llegar a la presidencia en la historia de Chile. Esta vez vuelve a presentarse
como candidata en representación de la concertación.

Ganó las elecciones primarias y sacó el mayor porcentaje de votaciones con
46,68% en primera vuelta del 2013.

### Matthei

Es la cuarta mujer en presentarse como candidata a la presidencia y la primera
en hacerlo en representación de la derecha.

Se presentó como reemplazo, luego de que Pablo Longueira, quien había ganado las
elecciones primarias, bajó su candidatura a mitad de año. En primera vuelta fue
la segunda candidata más votada con 25,01%.

### Soltera otra vez

Teleserie nocturna de Canal 13 cuya primera temporada fue estrenada en mayo de 2012. Ha gozado de la suficiente popularidad para tener una segunda temporada,
la cual comenzó a emitirse en julio de 2013. La segunda temporada sigue los
sucesos ocurridos en la primera temporada, donde Cristina, la protagonista,
comenzó una búsqueda por perder su estado de soltería.


2.1 Programa
============
La deconstrucción de la selección de las imágenes se hizo a través de un
programa especializado creado en Processing. Como lenguaje de programación,
Processing se creó como un puente entre las disciplinas visuales y las
disciplinas ligadas a la tecnología computacional. Es una versión simplificada
de otro lenguaje de programación, pues contiene código predefinido para
facilitar el trabajo a personas ajenas a la programación. Sin embargo, a medida
que se aprende más de Processing, se puede escribir un programa desde cero para
una gran cantidad de situaciones. Con un poco de dominio sobre el lenguaje, de
pronto se está ante una caja de herramientas útil para la construcción y
deconstrucción de imágenes. Mientras algunos deciden usar métodos tradicionales
para crear imágenes, algunos se han aventurado desde hace años a generar
imágenes directamente a través de la programación.

El código no está ligado a un solo lenguaje de programación. Como lenguaje,
Processing es solo una forma de crear las condiciones para generar imágenes.
Como cualquier lengua, puede ser traducido a otras lenguas y viceversa. Si
traducimos el código de la página siguiente a español, obtenemos una serie de
condiciones que definen cómo y cuándo se crea una imagen.


2.1.1 Español
-------------
Un grupo de imágenes es seleccionado y ordenado como una secuencia. Se carga la
primera imagen de esa secuencia. Se dibuja una grilla de un tamaño definido de
antemano sobre la imagen cargada. La grilla subdivide la imagen cargada, creando
una nueva imagen. Ahora cada cuadrado de la grilla es de un solo color. El color
de un cuadrado es definido a partir de su posición en la imagen cargada
original. La nueva imagen se guarda.

Los cuadrados de la grilla se reagrupan en función de sus matices. La nueva
imagen se guarda.

Los cuadrados de la grilla se reagrupan en función de su saturación, de arriba
hacia abajo y de mayor saturación a mayor saturación. La nueva imagen se guarda.

Los cuadrados de la grilla se reagrupan en función de su luminosidad, de arriba
hacia abajo y de mayor luminosidad a menor luminosidad. La nueva imagen se
guarda.

Se comprueba si existen más imágenes en la secuencia. Si existe, se carga la
siguiente imagen original y se repite el proceso. Si no quedan más imágenes en
la secuencia, el proceso se da por completado.


2.2 Deconstrucción
==================
De todos los métodos para descomponer una imagen, este cuaderno solo se preocupa de estudiar las imágenes en términos de color. Como estudio de color, las
siguientes páginas dividen las imágenes seleccionadas anteriormente en 4 tipos:
Una paleta de color basada en la imagen original, matiz, saturación y
luminosidad. Esto nace a partir de un modelo específico de clasificar el color,
denominado HSB.

El modelo HSB divide el color en tres categorías: matíz, saturación y
luminosidad. Visualmente corresponde a un cilindro, donde el matíz corrresponde
a una rueda de 360° en los extremos del cilindro. Cada matiz corresponde a un
grado específico. La saturación de un color se mide en el eje que va desde el
centro de la rueda hasta los límites exteriores, en niveles de 0% - 100%. La
luminosidad se mide en el eje que atraviesa el cilindro por el centro y también
se mide en niveles de 0% - 100%.

El estudio presenta dos dimensiones, individuales pero complementarias. Un
aspecto del estudio se preocupa únicamente de observar las imágenes con la
teoría de color como base y presenta observaciones concisas y objetivas. Su
contraparte es una interpretación subjetiva de las imágenes que toma prestados
los conceptos de la teoría de color en su dimensión retórica. Matiz, saturación
y luminosidad toman un doble sentido en tanto aspecto del color como adjetivo de algún elemento de las imágenes.


2.3 Observaciones
=================

(En proceso)
