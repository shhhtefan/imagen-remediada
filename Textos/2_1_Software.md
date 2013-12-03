Software
========
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
