Archivo Notas para CSS

es como la skin y html es las articulaciones o huesos del skin

la mejor forma de incluir css en el proyecto es en carpetas diferentes y arhcivos refenciados en el head con el link. se puede poner debajo del titulo, el java script si es bueno ponerlo despues del body pero el css arriba del body


se pueden agregar estilos por etiqueta,clase o id

para que los cambios del css se vean reflejados en el html primero tengo que guardar el html

//////////////////////////////
/           Reto            /
/                           /
/ Crear una lista de super  /
/ Usando html y css se pide /  
/ el uso de imgagenes       /
/////////////////////////////

Pseudo clases y pseudo elementos

BEM

Aprender bem que es el que ayuda a nombrar clases de manera sencilla siguiendo unas reglas globales.

![image](https://user-images.githubusercontent.com/101487602/159143700-c77873c2-bec7-4bb8-aca3-a700d8930438.png)

-------------------------------------------------------------------------------------------------------------
con list-style=none podemos quitar los numeros o guiones de las listas.

padding es un espacio interno en un contenedor.

border-radius redondea las esquinas del elemento al que se la aplicamos.

text-decoration quita las lineas que hacen ver los textos como si fuera vinculos.

Pseudo clases

Hover es que el mouse este arriba del elemento es decir cuando yo pase el mouse encima de un elemento que tenga hover hara un efecto.

active cambia cuando se le da click al objeto en cuestion

Pseudo elemento

Se llaman con :: no como las pseudo clases que se llaman solo con :

el pseudo elemento after siver para poner algo despues del elemento, se usa con content

![image](https://user-images.githubusercontent.com/101487602/159143725-6d212c32-550f-4586-bc4d-7844529fdb10.png)


ANATOMIA DE UNA REGLA EN CSS

![image](https://user-images.githubusercontent.com/101487602/159143769-c99e1f44-920d-4c97-be58-62144ede5143.png)

![image](https://user-images.githubusercontent.com/101487602/159143782-0964b483-6697-4476-9112-043878408dbb.png)


MODELO DE CAJA

Tiene varios estilos que son

Margin:espacio de la caja hacia afuera.

Border:

Padding:Espacio de la caja hacia adentro.

Content:Texto,img,video.

se puede jugar con el width,height, y dependiendo la posicion con el left,bottom,top o right. mirar la imagen acontinuacion para entender mejor

![image](https://user-images.githubusercontent.com/101487602/159143841-12e11bd4-e042-40bd-8323-c44958ecf3f6.png)

![image](https://user-images.githubusercontent.com/101487602/159143847-bba1721e-62ef-43fd-8f2f-0c8e2dca0b15.png)

COMO RESETEAR LOS ESTILOS QUE SETEA EL NAVEGADOR?:

Selector universal *

El scroll se puede quitar con el boxsizing:suma el padding con el width del elemento por lo que quita el espacio del elemento para no hacer crecer el borde y generar el scroll.

lo que se puso en selectro universal debe ponerse siempre en todas las hojas de estilo para quitar los valores por defecto del navegador.

