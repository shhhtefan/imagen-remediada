Índice y contenidos clave
=========================

###### 1.1 Manifiesto

1.  La tecnología condiciona la forma en que percibimos nuestro mundo

2.  Todas las imágenes están mediadas por la tecnología.

3.  Re-mediación

###### 1.2 Introducción

1.  De qué trata el libro

2.  Por qué es importante publicar un libro sobre aquello

3.  Estructura del libro

4.  A quien/es va dirigido

###### 1.3 Sujetos de prueba

Criterios de selección:

1.  Contingencia

2.  Presentar campañas políticas y razón de la elección de las candidatas

3.  Razon de la presencia de "Soltera Otra Vez"

###### 1.3.1 Bachelet

1.  Reseña de su campaña

###### 1.3.2 Matthei

1.  Reseña de su campaña

###### 1.3.3 Soltera Otra Vez

1.  Reseña de la teleserie

###### 2.1 Programa

1.  Presentar processing

2.  El código como herramienta de condicionamiento

	###### 2.1.1 Español

	1.  Programa traducido al español

###### 2.2 Deconstrucción

1.  Explicar qué se hizo con el programa

2.  Modelo de Color

3.  Modo de estudio

###### 2.3 Observaciones

1.  Objetivas: Comparativa de color en términos de matiz, saturación y brillo

2.  Subjetivas: Interpretaciones personales en términos de matiz, saturación y
    brillo, pero en su dimensión retórica.


1.1 Manifiesto
==============

01 // La tecnología condiciona nuestra forma de percibir el entorno.

02 // Las imágenes están mediadas directa o indirectamente por la tecnología.

03 // Todo puede ser re-mediado.



1.2 Introducción
================

El cuaderno que sostiene entre sus manos es un ejercicio de deconstrucción de
las campañas presidenciales de Michelle Bachelet y Evelyn Matthei. Se
descomponen imágenes al punto de hacer casi irreconocible su discurso original
y, a partir de ello, se configuran nuevas interpretaciones.

Se utilizan dos herramientas para este proceso: diseño generativo y código. El
diseño generativo es una metodología relativamente nueva utilizada en
disciplinas diversas como arquitectura, diseño y ciencias computacionales. A
diferencia de otras metodologías, el diseño generativo se enfoca principalmente
en los procesos emergentes y en la exploración de posibilidades. Las
definiciones de esta metodología están fuertemente relacionadas con la
computación, por lo que muchas veces se emplea un lenguaje de programación (o
código) para crear los procesos. Para efectos de este libro se utilizó un
lenguaje enfocado en disciplinas visuales, conocido como* Processing*.

No es la única manera de realizar un ejercicio de este tipo, pero es, a mi
parecer, una manera interesante de hacerlo, particularmente porque la
programación ya es un pilar de nuestra sociedad. En realidad, la *tecnología* es
parte integral de nuestro mundo, permea todas nuestras actividades y condiciona
nuestra interacción con el entorno. Las imágenes, en todas sus formas, también
están condicionadas.

Las imágenes para las campañas presidenciales están condicionadas por la
perspectiva de cada candidata y el conglomerado político que representan. Ambas
campañas hacen uso de un imaginario de la sociedad y por primera vez estamos
frente a dos representaciones de la mujer chilena, provenientes de dos bandos
políticamente opuestos.

Todas estas imágenes fueron creadas con una intención, pero además fueron
creadas con software. Pareció natural, entonces, tratar de re-mediar las
imágenes con la ayuda de un lenguaje de programación.

El cuaderno está dividido en 2 partes: *setup* y *draw.* En *setup* se
establecen las variables que sirven de fundación para el ejercicio de
deconstrucción; por variables me refiero al origen de las imágenes, el criterio
de selección, etc. *Draw*, en cambio, compone el grueso de este libro, y
presenta las imágenes descompuestas según los tres aspectos principales del
modelo de color HSB: matíz (*hue*), saturación y brillo.

Espero que cualquier persona con cierta afinidad por la visualidad vea algo de
interés en este cuaderno. Además de ser un ejercicio de deconstrucción, este
cuaderno es una invitación a detenerse y pensar cómo vemos las imágenes.



1.3 Sujetos de prueba
=====================

El conjunto de imágenes seleccionadas para la deconstrucción se basa
principalmente en la contingencia. Por una serie de hechos imprevistos, las
elecciones presidenciales de 2013 son las primeras en enfrentar a dos mujeres de
conglomerados políticos opuestos, como candidatas a la presidencia.

Esto presenta un escenario interesante, pues permite comparar en términos
visuales dos formas de representar a la sociedad y a la mujer chilena, en
condiciones prácticamente iguales. Ambas candidaturas hacen uso de los mismos
medios en formatos similares y el contenido de las imágenes tiene un alto grado
de similitud, si bien la forma de presentar los contenidos puede ser distinta.

Para nutrir más la comparación de las representaciones visuales de ambas
candidatas, es conveniente introducir un tercer exponente, cuya presencia sirva
como punto de control con respecto al discurso de las candidatas. Este tercer
exponente debería ser contemporáneo a las campañas presidenciales y compartir
algunos rasgos que aparecen en las imágenes de las candidatas, pero también
debería provenir de un contexto ajeno a las elecciones presidenciales. Uno de
esos exponentes es "Soltera Otra Vez", pues ofrece una tercera perspectiva sobre
cómo se representa la sociedad y la mujer chilena desde un contexto de
entretenimiento masivo.

Con algunas excepciones hacia el final de este cuaderno, se hizo el intento de
presentar el conjunto de imágenes de forma objetiva e imparcial.



### Bachelet

Candidata de la autodenominada "Nueva Mayoría". En 2006, Michelle Bachelet fue
la segunda mujer en presentarse como candidata a la presidencia y la primera en
ganar dichas elecciones en la historia de Chile.

Esta vez vuelve a presentarse como candidata en representación de la
concertación. Ganó las elecciones primarias y obtuvo el mayor porcentaje de
votaciones con 46,68% en primera vuelta del 2013.



### Matthei

Es la cuarta mujer en presentarse como candidata a la presidencia y la primera
en hacerlo en representación de la derecha.

Se presentó como reemplazo, luego de que Pablo Longueira, quien había ganado las
elecciones primarias, bajara su candidatura a mitad de año. En primera vuelta
fue la segunda candidata más votada con 25,01%.



### Soltera otra vez

Teleserie nocturna de Canal 13, cuya primera temporada fue estrenada en mayo de
2012. Ha gozado de la suficiente popularidad para tener una segunda temporada,
la cual comenzó a emitirse en julio de 2013. La segunda temporada sigue los
sucesos ocurridos en la primera temporada, en la que Cristina, la protagonista,
comienza una búsqueda por perder su estado de soltería.



2.1 Programa
============

La deconstrucción de la selección de imágenes se hizo a través de un programa
especializado creado en *Processing.* Como lenguaje de programación,
*Processing* se creó con el fin de ser un puente entre las disciplinas visuales
y las disciplinas ligadas a la tecnología computacional. Es una versión
simplificada de otro lenguaje de programación, pues contiene código predefinido
para facilitar el trabajo a personas ajenas a la programación. Sin embargo,
usuarios avanzados son capaces escribir un programa desde cero para una gran
cantidad de situaciones. Con un poco de dominio sobre este lenguaje, de pronto
se está ante una caja de herramientas útil para la construcción y deconstrucción
de imágenes. Mientras algunos deciden usar métodos tradicionales para crear
imágenes, otros se han aventurado desde hace años a producirlas directamente a
través de la programación.

El código no está ligado a un solo lenguaje de programación. Como lenguaje,
*Processing* es solo una forma de crear las condiciones para generar imágenes, y
al igual que cualquier lengua, puede ser traducido a otras lenguas y viceversa.
Si se traduce el código de la página siguiente a español, se obtendrá una serie
de condiciones que definen cómo y cuándo se crea una imagen.



Un programa, en español
-----------------------

1.  Un grupo de imágenes es seleccionado y ordenado como una secuencia.

2.  Se carga la primera imagen de esa secuencia. Se dibuja una grilla de un
    tamaño definido de antemano sobre la imagen cargada. La grilla subdivide la
    imagen cargada, creando una nueva imagen.

3.  Ahora cada cuadrado de la grilla es de un solo color. El color de un
    cuadrado es definido a partir de su posición en la imagen cargada original.
    La nueva imagen se guarda.

4.  Los cuadrados de la grilla se reagrupan en función de sus matices. La nueva
    imagen se guarda.

5.  Los cuadrados de la grilla se reagrupan en función de su saturación, de
    arriba hacia abajo y de mayor saturación  mayor saturación. La nueva imagen
    se guarda.

6.  Los cuadrados de la grilla se reagrupan en función de su luminosidad, de
    arriba hacia abajo y de mayor luminosidad a menor luminosidad. La nueva
    imagen se guarda.

7.  Se comprueba si existen más imágenes en la secuencia. Si existe, se carga la
    siguiente imagen original y se repite el proceso. Si no quedan más imágenes
    en la secuencia, el proceso se da por completado.





2.2 Deconstrucción
==================

De todos los métodos para descomponer una imagen, este cuaderno solo se preocupa
de estudiar las imágenes en términos de color. Como estudio de color, las
siguientes páginas dividen las imágenes seleccionadas anteriormente en 4 tipos:
la imagen original, matiz, saturación y brillo. Esto nace a partir de un modelo
específico para clasificar el color, denominado HSB.

El modelo HSB divide el color en tres categorías: matiz, saturación y
luminosidad. Visualmente corresponde a un cono invertido, donde el matiz se mide
por el perímetro de la base del cono y cada matiz tiene una posición específica
de los 360° de la base. La saturación de un color corresponde al área que abarca
desde el centro de la base hasta la punta del cono, y se mide en niveles de 0% -
100%. El brillo se mide en el eje que atraviesa el cono por el centro y también
se mide en niveles de 0% - 100%.

El estudio presenta dos dimensiones, individuales pero complementarias. Un
aspecto del estudio se preocupa únicamente por observar las imágenes a través de
las tres propiedades del color, y presenta observaciones concisas y objetivas.
Su contraparte consiste en una interpretación subjetiva de las imágenes, que
toma prestados los conceptos de la teoría de color en su dimensión retórica.
Matiz, saturación y brillo toman un doble sentido en cuanto son una propiedad
del color, así como un adjetivo usado para referirse a otros elementos de
nuestro entorno.



2.3 Observaciones
=================

Observaciones (cuantitativas)
---

Nota: Vale la pena recordar que estas observaciones aplican únicamente a:

1.  El uso de color en cuánto matiz, saturación y brillo según sus definiciones
    en el modelo de color HSB.

2.  Esta selección de imágenes. Tanto las candidatas como la teleserie siguió
    publicando imágenes y videos durante la producción de este cuaderno, y
    podrían haber sido creadas en condiciones distintas a las de esta selección.
    Además se mantiene la nomenclatura de (B), (M) y (S) para hacer evidente que
    no se esta analizando a las candidatas y la protagonista de la teleserie,
    sino la selección de imágenes.



Como recordatorio, se vuelven a definir las propiedades de color del modelo
HSB[ADOBE]:

**Matiz**: Color reflejado o transmitido a través de un objeto. Se mide como una
posición en la rueda de colores estándar y se expresa en grados entre 0° y 360°.
Normalmente, el tono se identifica por el nombre del color, como rojo, naranja o
verde.

**Saturación:** Es la fuerza o pureza del color. La saturación representa la
cantidad de gris que existe en proporción al tono y se expresa como un
porcentaje comprendido entre el 0% (gris) y el 100% (saturación completa). En la
rueda de colores estándar, la saturación aumenta a medida que nos aproximamos al
borde de la misma.

**Brillo:** Luminosidad u oscuridad relativa del color y normalmente se expresa
como un porcentaje comprendido entre 0% (negro) y 100% (blanco).



### Matiz:

| Matíz			| (B) 	   | (M)	  | (S)      |
|---------------|----------|----------|----------|
| Azul          | 13       | 06       | 09       |
| Rojo          | 03       | 04       | 05       |
| Naranja       | 01       | 05       | 05       |
| Amarillo      | 02       | 06       | 07       |
| Verde         | 0        | 02       | 02       |
| Violeta       | 0        | 0        | 02       |
| Indeterminado | 08       | 0        | 01       |

(B) se diferencia notoriamente de las otras muestras al utilizar
mayoritariamente matices de azul, complementado con otro matiz de igual o menor
jerarquía. (M) y (S), en cambio, hacen uso de una paleta de colores variada y
comparten los mismos matices con leves diferencias. Resulta interesante el
parecido de (M) y (S) en su uso del color, considerando sus contextos y
discursos disímiles, aunque no queda claro si la similitud en el tratamiento de
las imágenes se debe a que estas estaban subordinadas al medio para el cual
fueron producidas, si se debe al contenido visual, o ambas. Con la excepción de
las imágenes producidas para *Facebook*, casi todas las imágenes de (M)
comparten al menos una de las tres propiedades del color con (S).



### Saturación:

| Fuente | Veces con la im agen más saturada |
|--------|-----------------------------------|
| (B)    | 03                                |
| (M)    | 03                                |
| (S)    | 08                                |

### Brillo:

| Fuente | Veces con la imagen más luminosa |
|--------|----------------------------------|
| (B)    | 04                               |
| (M)    | 05                               |
| (S)    | 05                               |





Observaciones (cualitativas)
---

### Definiciones (R.A.E.)

**Matiz:**

(De *matizar*).

**1.** m. Rasgo poco perceptible que da a algo un carácter determinado.

**2.** m. Unión de diversos colores mezclados con proporción.

**3.** m. Cada una de las gradaciones que puede recibir un color sin perder el
nombre que lo distingue de los demás.

**4.** m. Rasgo y tono de especial colorido y expresión en las obras literarias.

**5.** m. En lo inmaterial, grado o variedad que no altera la sustancia o
esencia de algo.

**Saturación:**

(Del lat. *saturatĭo, -ōnis*).

**1.** f. Acción y efecto de saturar.

**Brillo:**

(De *brillar*).

**1.** m. Luz que refleja o emite un cuerpo.

**2.** m. Lucimiento, gloria.

**Brillar:**

(Del it. *brillare*).

**1.** intr. Dicho de un cuerpo: Emitir o reflejar luz.

**2.** intr. Dicho de una persona: Sobresalir en talento, hermosura, etc.





