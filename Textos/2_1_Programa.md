Programa
========

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


