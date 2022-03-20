Archivo Notas para CSS

es como la skin y html es las articulaciones o huesos del skin

la mejor forma de incluir css en el proyecto es en carpetas diferentes y arhcivos refenciados en el head con el link. se puede poner debajo del titulo, el java script si es bueno ponerlo despues del body pero el css arriba del body


se pueden agregar estilos por etiqueta,clase o id

para que los cambios del css se vean reflejados en el html primero tengo que guardar el html

![image](https://user-images.githubusercontent.com/101487602/159144976-aa0440ed-582e-45c9-bd7b-d394576ebe65.png)



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

HERENCIA EN CSS

html tiene un tamaño de fuente predefinida de 16 px y eso se puede cambiar en css mirar el styles de la claseHerencia.

La herencia se puede romper, 

Orden de declaracion

1.Importancia
    
    Primero se cargan los estilos del navegador,luego nuestros estilos.
    
    El important si bien sirve es una mala practica no se deberia de usar a menos que se extrictamente necesario

2.Especificidad

    En el cuadro se tienen numeros de izquierda a derecha donde izquierda es mas importante y derecha menos importante.
    
  ![image](https://user-images.githubusercontent.com/101487602/159144440-9e7471a7-4ac3-4a20-92b4-ff692d740d49.png)


REGLAS DE CASCADA DEL NAVEGADOR

![image](https://user-images.githubusercontent.com/101487602/159144475-88b59ef1-8baa-4025-b520-dea911738dfc.png)


3.Orden en las fuentes

    es como mandamos a llamar los estilos, se mira de arriba a abajo, se aplican los estilos que esten hasta abajo osea los ultimos y por tanto reescribir los estilos que pusimos arriba.Tambien afecta en donde llamamos nuestra hoja de estilos en el html con el link.

Los id son unicos  solo los puede tener un elemento las clases son genericas y las pueden tener varios elementos

en el editor de texto solo con pararse encima de una regla de css vemos Specificity, entre mas puntaje tenga tenga mas arriba en el orden esta.

No es bueno tener tanto id en el css es mejor que eso se deje para js, mejor trabajar en clases


COMBINADORES

Ayudan a tener una especificidad mucho mas alta para evitar el uso de ids


h2 + p{
    color: red;
} combinador hermano cercano o Adjacent Siblings--> Esto significa aplicale el color rojo a todas las etiquetas parrafo que esten cerca de un h2

h2 ~ p{
    color:blue
}Combinador hermano general o General Siblings-->esto quiere decir todos los hermanos que esten juntos identados osea que existan en la misma altura, mirar el ejemplo de claseCombinadores.

div > p{
    color: blueviolet;
}Combinador Hijo directo: se lee a la etiqueta parrafo que sea hija directa de un div ponerle color morado.osea que si la etiqueta parrafo esta dentro de un div osea justo debajo del div sin nada que lo tape como una etiqueta secion o otro tipo de etiqueta contenedora aplicara la regla de css, si esto no es asi entonces no la aplicara, debe ser decendiente directo.

.nav a{
    color: blue;
}Combinador descendiente: es la que hemos estado usando siempre las mas basica de todas.