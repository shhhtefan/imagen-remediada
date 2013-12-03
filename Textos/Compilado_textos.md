Índice
-------------------------
    1.1 Manifiesto (βeta)
    1.2 Introducción
    1.3 Sujetos de prueba
        1.3.1 Bachelet
        1.3.2 Matthei
        1.3.3 Soltera Otra Vez
    2.1 Software
        2.1.1 Español
    2.2 Re-mediación
        2.2.1 Deconstrucción
        2.2.2 Observaciones
    3.1 Manifiesto (v.1.0)

1.1 Manifiesto (βeta)
==================
01. __La tecnología condiciona nuestra forma de percibir el entorno__.  
La actividad humana está subordinada a la tecnología y no al revés. De forma voluntaria o involuntaria, dejamos que influya en nuestra percepción de la realidad. Existen otras maneras de entender el mundo, pero para bien o para mal, esta es la dominante.

02. __Las imágenes están mediadas directa o indirectamente por la tecnología__.  
Donde pongamos nuestra vista, las imágenes están condicionadas; la pantalla es nuestra ventana al mundo, los paisajes son artificiales, los números son nuestras guías.


1.2 Introducción
================
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


1.3 Sujetos de prueba
=====================
El conjunto de imágenes seleccionadas para la deconstrucción se basa principalmente en la contingencia política. Por una serie de hechos imprevistos, las elecciones presidenciales de 2013 son las primeras en enfrentar a dos mujeres de conglomerados políticos opuestos, como candidatas a la presidencia.

Esto presenta un escenario interesante, pues permite comparar en términos visuales dos formas de representar a la sociedad y a la mujer chilena, en condiciones prácticamente iguales. Ambas candidaturas hacen uso de los mismos medios en formatos similares y el contenido de las imágenes tiene un alto grado de similitud, si bien la forma de presentar los contenidos puede ser distinta.

Para nutrir más la comparación de las representaciones visuales de ambas candidatas, es conveniente introducir un tercer exponente, cuya presencia sirva como punto de control con respecto al discurso de las candidatas. Este exponente debe ser contemporáneo a las campañas presidenciales y compartir algunos rasgos que aparecen en las imágenes de las candidatas, pero también debe provenir de un contexto ajeno a las elecciones presidenciales. Un modelo posible es "Soltera Otra Vez", pues ofrece una tercera perspectiva sobre cómo se representa en los medios la sociedad y la mujer chilena desde un contexto de entretenimiento masivo, además de utilizar los mismos medios que las campañas.

Definidos los tres exponentes, es hora de marcar las condiciones para selección del conjunto de imágenes. Para este ejercicio, la selección se llevó a cabo bajo los siguientes criterios:
1. Las imágenes de cada exponente deben provenir de uno de estos cuatro medios utilizados por las candidatas/teleserie: La galería de fotos oficial, la galería de fotos de la página de su _facebook_ oficial, un banner web oficial, y capturas de imagen de un video publicado por las candidatas/Canal13.
2. Se elegirán dos imágenes por cada origen, con la excepción de las capturas de video. Para las capturas se deben elegir dos videos de cada exponente y tomar cuatro capturas por cada video, en un intervalo de 30 segundos. En síntesis, por cada exponente se deben elegir 14 imágenes.
2. En lo posible, las imágenes de las tres muestras deben compartir la proporción, el contenido visual (retrato, paisaje, etc.) y la técnica utilizada (fotografía, ilustración, etc.), y sólo deben hacerlo si provienen del mismo medio. Por ejemplo, todas las capturas de video deben compartir estas propiedades entre ellas, pero no necesariamente deben hacerlo con las fotos provenientes de la galería de _facebook_.
3. En el caso de los videos, estos deben ser publicados en fechas similares (en lo posible el mismo día) y, en el caso de las candidatas, compartir la temática. Los videos de "Soltera Otra Vez" sólo necesitan cumplir la condición temporal. 
> Nota: Los videos seleccionados por cada candidata corresponden a los primeros capítulos de la franja electoral emitidos para la primera vuelta de las elecciones presidenciales.

Las imágenes seleccionadas tuvieron modificaciones mínimas, pues se hizo lo posible para intervenirlas lo menos en esta etapa. Con la excepción de algunos cambios de tamaño para igualar las muestras, se mantuvieron las proporciones, resoluciones y modos de color tal cual se presentan en sus medios de origen.


### Bachelet

Candidata de la autodenominada "Nueva Mayoría". En 2006, Michelle Bachelet fue la segunda mujer en presentarse como candidata a la presidencia y la primera en ganar dichas elecciones en la historia de Chile.

Esta vez vuelve a presentarse como candidata en representación de un conglomerado político que reúne a la izquierda chilena con la Concertación. Ganó las elecciones primarias y obtuvo el mayor porcentaje de votaciones con 46,68%[ref] en primera vuelta de las elecciónes presidenciales, en noviembre del 2013.

### Matthei

Es la cuarta mujer en presentarse como candidata a la presidencia y la primera en hacerlo en representación de la derecha.

Se presentó como reemplazo luego de que Pablo Longueira, quien había ganado las elecciones primarias, bajara su candidatura a mitad de año. En primera vuelta fue la segunda candidata más votada con 25,01%[ref].

### Soltera otra vez

Teleserie nocturna de Canal 13, cuya primera temporada fue estrenada en mayo de 2012. Ha gozado de la suficiente popularidad como para tener una segunda temporada, la cual comenzó a emitirse en julio de 2013. La segunda temporada sigue los sucesos ocurridos en la primera temporada, en la que Cristina, la protagonista, comienza una búsqueda por perder su estado de soltería.


2.1 Software
============
La deconstrucción de la selección de imágenes se hizo a través de un _software_ especializado creado en _Processing_. Como lenguaje de programación, _Processing_ se creó con el fin de ser un puente entre las disciplinas visuales y las disciplinas ligadas a la computación. Es una versión adaptada de _Java_, un lenguaje multipropósito, y como tal contiene código predefinido para facilitar el trabajo a personas ajenas a este mundo. Sin embargo, usuarios avanzados son capaces de escribir un _software_ desde cero para una gran cantidad de situaciones. Con un poco de dominio sobre este lenguaje, de pronto se está ante una caja de herramientas útil para el fin de este cuaderno; la construcción y deconstrucción de imágenes. Mientras algunos deciden usar métodos tradicionales para crear imágenes, otros se han aventurado desde hace años a producirlas directamente a través de la programación.
> Nota: _Processing_ (a veces escrito _p5_) no sólo es un lenguaje de programación. Se le llama así al conjunto de lenguaje, entorno de desarrollo que ejecuta el lenguaje y comunidad que le da vida al proyecto. La comunidad ha producido una serie de tutoriales y guías introductorias para ayudar a diseñadores, artistas y aficionados a aprender la sintaxis detrás de _p5_. Un buen punto de partida es http://hello.processing.org/ y http://processing.org/tutorials/gettingstarted/.

El concepto de _código_ no está ligado a un sólo lenguaje de programación, ni siquiera es exclusivo de los lenguajes computacionales. Como lenguaje, _Processing_ es sólo una de diversas formas de crear las condiciones para generar imágenes, y al igual que cualquier lengua, puede ser traducida. Si se traduce el código de la página siguiente a español, se obtendrá una serie de condiciones que definen cómo y cuándo se crea una imagen.


Un software, en español
-----------------------
> Nota: Estas son las instrucciones que definen las condiciones fundacionales para el _software_ necesario para la deconstrucción de las imágenes. Es el código original, escrito en nuestro idioma y de forma concisa, y sirve de punto de partida para la traducción a cualquier otro lenguaje de programación, no solo _Processing_.

1.  Un grupo de imágenes es seleccionado y ordenado como una secuencia.

2.  Se carga la primera imagen de esa secuencia. Se dibuja una grilla de un tamaño definido previamente sobre la imagen cargada. La grilla subdivide la imagen cargada, creando una nueva imagen.

3.  Ahora cada cuadrado de la grilla es de un sólo color. El color de un cuadrado es definido a partir de su posición en la imagen cargada original. La nueva imagen se guarda.

4.  Los cuadrados de la grilla se reagrupan en función de sus matices. La nueva imagen se guarda.

5.  Los cuadrados de la grilla se reagrupan en función de su saturación, desde arriba hacia abajo y de mayor saturación a menor saturación. La nueva imagen se guarda.

6.  Los cuadrados de la grilla se reagrupan en función de su luminosidad, desde arriba hacia abajo y de mayor luminosidad a menor luminosidad. La nueva imagen se guarda.

7.  Se comprueba si existen más imágenes en la secuencia. Si existen, se carga la siguiente imagen original y se repite el proceso. Si no quedan más imágenes en la secuencia, el proceso se da por completado.


El mismo software, en código: Processing
----------------------------------------
(ver maqueta)


2.2 Re-mediación
==================
De todos los métodos para descomponer una imagen, este cuaderno sólo se preocupa de estudiar las imágenes en términos de color. Como estudio de color, las siguientes páginas dividen las imágenes seleccionadas anteriormente en 4 categorías: la imagen original, matiz, saturación y brillo. Esto nace a partir de las propiedades del color definidos en el modelo HSB.

El modelo HSB divide el color en tres categorías: matiz, saturación y luminosidad. Visualmente corresponde a un cono invertido, donde el matiz se mide por el perímetro de la base del cono y cada matiz tiene una posición específica en los 360° de la base. La saturación de un color está representado por el área que abarca desde la base hasta la punta del cono, y se expresa en niveles de 0% - 100%. El brillo se mide en el eje que atraviesa el cono por el centro, en niveles de 0% - 100%.
> Falta: Acompañar con diagrama.

El estudio presenta dos dimensiones individuales pero complementarias. Un aspecto del estudio se preocupa únicamente por observar las imágenes a través de las tres propiedades mencionadas en el párrafo anterior, y se manifiesta a través de observaciones concisas y objetivas. Su contraparte consiste en una interpretación subjetiva de las imágenes, que toma prestados los conceptos de la teoría de color en su _dimensión retórica_. Matiz, saturación y brillo toman un doble sentido en cuanto son una propiedad del color, así como adjetivos en nuestro lenguaje común para referirse a elementos distintos al color. 

Todo esto se despliega a lo largo de dos secciones. En el primer apartado, ambas perspectivas dialogan entre ellas y junto a las imágenes en forma de afirmaciones cortas, mientras el segundo y último apartado contiene un breve análisis desde ambas perspectivas que complementa las anotaciones de la primera sección.

##2.2.1 Deconstrucción

(ver maqueta)

##2.2.2 Observaciones

###Observaciones cuantitativas

>Nota: Vale la pena recordar que estas observaciones aplican únicamente a:
1.  El uso de color en cuanto matiz, saturación y brillo según sus definiciones en el modelo de color HSB.
2.  Esta selección de imágenes. Tanto las candidatas como la teleserie siguió publicando imágenes y videos durante la producción de este cuaderno, y podrían haber sido creadas en condiciones distintas a las de esta selección. Además se mantiene la nomenclatura de (B), (M) y (S) para hacer evidente que no se esta analizando a las candidatas y la protagonista de la teleserie, sino la selección de imágenes.

#### Matiz:
>Nota: __Matiz__: Color reflejado o transmitido a través de un objeto. Se mide como una posición en la rueda de colores estándar y se expresa en grados entre 0° y 360°. Normalmente, el tono se identifica por el nombre del color, como rojo, naranja o verde.

| Matiz         | (B)      | (M)      | (S)      |
|---------------|----------|----------|----------|
| Azul          | _13_     | _06_     | _09_     |
| Rojo          | 03       | 04       | 05       |
| Naranja       | 01       | 05       | 05       |
| Amarillo      | 02       | _06_     | _07_     |
| Verde         | 0        | 02       | 02       |
| Violeta       | 0        | 0        | 02       |
| Indeterminado | _08_     | 0        | 01       |

(B) se diferencia notoriamente de las otras muestras al utilizar  mayoritariamente matices de azul, complementado con otro matiz de igual o menor jerarquía. (M) y (S), en cambio, hacen uso de una paleta de colores variada y comparten los mismos matices con leves diferencias. Con la excepción de las imágenes producidas para _facebook_, casi todas las imágenes de (M) comparten al menos una de las tres propiedades del color con (S). Resulta interesante el parecido entre ambas muestras en su uso del color, considerando sus contextos y discursos disímiles, aunque no queda claro si la similitud en el tratamiento de las imágenes se debe a que estas estaban subordinadas al medio para el cual fueron producidas, al contenido de ellas, o ambas.


#### Saturación:
>Nota: __Saturación:__ Es la fuerza o pureza del color. La saturación representa la cantidad de gris que existe en proporción al tono y se expresa como un porcentaje comprendido entre el 0% (gris) y el 100% (saturación completa). En la rueda de colores estándar, la saturación aumenta a medida que nos aproximamos al borde de la misma.

| Fuente | más saturada    | medianamente sat.   | menos sat.  |
|--------|-----------------|---------------------|-------------|
| (B)    | 03              | 04                  | _09_        |
| (M)    | 03              | _08_                | 03          |
| (S)    | _08_            | 02                  | 02          |
> Nota: Si bien le reconfiguración de los colores se hizo con la ayuda de los _software_, las observaciones se realizaron de forma visual. Por esto, las anotaciones sobre la saturación no son 100% confiables, ya que esta puede provocar distintos resultados finales dependiendo de la luminosidad del color. Esto es especialmente cierto en las imágenes de (B).

(B) pareciera utilizar colores desaturados, mientras (S) prefiere colores fuertes y saturados. (M) se encuentra en un punto medio en relación a las demás muestras, pues dependiendo del medio donde aparecieron las imágenes originalmente, varía en sus niveles de saturación. Las otras dos muestras, en cambio, son consistentes en sus niveles.

#### Brillo:
>Nota: __Brillo:__ Luminosidad u oscuridad relativa del color y normalmente se expresa como un porcentaje comprendido entre 0% (negro) y 100% (blanco).

| Fuente | más luminosa   | medianamente lum.   | menos luminosa   |
|--------|----------------|---------------------|------------------|
| (B)    | 04             | 01                  | _09_             |
| (M)    | _05_           | _07_                | 02               |
| (S)    | _05_           | 06                  | 03               |

Parece haber una relación entre los matices dominantes y la configuración de brillo (y saturación). Aunque las tres muestras tienen un número similar de veces en las que son las más brillantes, (B) gravita mucho más hacia colores poco luminosos. (M) y (S) se mantienen en niveles medios-altos a lo largo de toda la selección.


### Observaciones cualitativas

####Matiz
> Nota: __Matiz:__  
(De _matizar_).  
__1.__ m. Rasgo poco perceptible que da a algo un carácter determinado.  
__2.__ m. Unión de diversos colores mezclados con proporción.  
__3.__ m. Cada una de las gradaciones que puede recibir un color sin perder el nombre que lo distingue de los demás.  
__4.__ m. Rasgo y tono de especial colorido y expresión en las obras literarias.  
__5.__ m. En lo inmaterial, grado o variedad que no altera la sustancia o esencia de algo.

(B) tiene un matiz sereno en su mayoría. El azul proporciona una sensación de seguridad y calma.
(M) está marcada por un matiz difuso. Es quizás la más difusa de las tres muestras. A veces hay un matiz de serenidad, otras uno de exaltación, de energía, otras de indeterminación.
(S) también tiene un matiz difuso, pero se diferencia con algunos hitos de tonos femeninos, o al menos lo que se considera femenino. Estos tonos están ausentes en Bachelet y Matthei o toman un rol secundario.

####Saturación
> Nota: __Saturación:__  
(Del lat. _saturatĭo, -ōnis_).  
__1.__ f. Acción y efecto de saturar.  

(S) es mucho más saturado en términos de contenido, aunque (M) se acerca bastante. (B) se aleja de ambas muestras con imágenes más limpias, más desaturadas.

####Brillo
> Nota:__Brillo:__  
(De _brillar_).  
__1.__ m. Luz que refleja o emite un cuerpo.  
__2.__ m. Lucimiento, gloria.  
__Brillar:__
(Del it. _brillare_).
__1.__ intr. Dicho de un cuerpo: Emitir o reflejar luz.
__2.__ intr. Dicho de una persona: Sobresalir en talento, hermosura, etc.

En ningun caso se aprecia brillantez, pero si destellos de gloria. (B) y (M) representan figuras poderosas, pero maternales a su manera, mientras (S) carece de ese brillo. Sin embargo, (S) es más luminosa y se destaca por sobre las otras dos muestras en su notoriedad.

---

Las muestras descompuestas no sostienen el discurso original por si mismas, pero este nunca desaparece. Una fracción del discurso se mantiene y se complementa con las interpretaciones nacidas de la abstracción forzada de las imágenes. A este nivel de descomposición, el contenido original pierde relevancia y toma el asiento trasero, influenciando el nuevo discurso. La posición de las imágenes en la grilla,  el conocimiento de sus orígenes, las anotaciones que las acompañan, se mezclan en una reinterpretación en conjunto con las propias experiencias de quien las observa, para formar nuevas imágenes mentales; un constructo entre lo visualizado, lo pensado y lo sentido. (B) ya no es sereno porque tuvo su origen en una fotografía de las campañas presidenciales de Michelle Bachelet, sino porque la abstracción ahora remite a un paisaje costero. 

De pronto, y sin mayor esfuerzo, hemos destripado las condiciones impuestas por el discurso original y hemos reacondicionado una imagen, es decir, la hemos _re-mediado_.


3.1 Manifiesto (v.1)
====================
01. __La tecnología condiciona nuestra forma de percibir el entorno__.  
La actividad humana está subordinada a la tecnología y no al revés. De forma voluntaria o involuntaria, dejamos que influya en nuestra percepción de la realidad. Existen otras maneras de entender el mundo, pero para bien o para mal, esta es la dominante.

02. __Las imágenes están mediadas directa o indirectamente por la tecnología__.  
Donde pongamos nuestra vista, las imágenes están condicionadas; la pantalla es nuestra ventana al mundo, los paisajes son artificiales, los números son nuestras guías.

03. __Todo puede ser re-mediado__.  
Podemos y debemos entender la influencia de la tecnología sobre nuestra percepción. Al re-mediar las cosas, realizamos un ejercicio de apropiación.