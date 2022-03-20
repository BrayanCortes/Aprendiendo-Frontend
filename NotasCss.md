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

![image](https://user-images.githubusercontent.com/101487602/159145493-68473428-2683-40c2-9f03-583f24e829e9.png)


Ayudan a tener una especificidad mucho mas alta para evitar el uso de ids


h2 + p{
    color: red;
} 

combinador hermano cercano o Adjacent Siblings--> Esto significa aplicale el color rojo a todas las etiquetas parrafo que esten cerca de un h2


h2 ~ p{
    color:blue
}

Combinador hermano general o General Siblings-->esto quiere decir todos los hermanos que esten juntos identados osea que existan en la misma altura, mirar el ejemplo de claseCombinadores.


div > p{
    color: blueviolet;
}

Combinador Hijo directo: se lee a la etiqueta parrafo que sea hija directa de un div ponerle color morado.osea que si la etiqueta parrafo esta dentro de un div osea justo debajo del div sin nada que lo tape como una etiqueta secion o otro tipo de etiqueta contenedora aplicara la regla de css, si esto no es asi entonces no la aplicara, debe ser decendiente directo.


.nav a{
    color: blue;
}

Combinador descendiente: es la que hemos estado usando siempre las mas basica de todas.


MEDIDAS ABSOLUTAS VS MEDIDAS RELATIVAS

![image](https://user-images.githubusercontent.com/101487602/159146191-13110974-7d18-4fc2-8cb1-26c7770bc98e.png)


Cuando se hable de medidas absolutas se habla en pixeles o px estas no cambian

medidas relativas son con porcentaje o las demas que veremos en la tabla estas cambian dependiendo del dispostivo donde se vean.

el responsive se hace con medida reltaivas

medida relativa em:es un acronimo de elemento y lo que hace es que tomara el tamaño de fuente que tiene el padre por defecto se debe usar con cuidado ya que puede ocasionar problemas uy grandes si no se llaman las medidas con cuidado.

Medida relativa rem:siempre va a tener referencia al estilo que tenga el root o la etiqueta root del proyecto, osea el html y el navegador por defecto a la etiqueta html le agrega un font de 16px, rem es mejor y menos confuso que el em.

---------------------------------------------------------------

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    font-size: 62.5%;
}

tanto el selector universal como el html siempre deben ir en todas las hojas de estilos de un proyecto de la forma en la que esta ahi para poder manejar el rem de una manera sencilla.

----------------------------------------------------------------

vh y vw, esto lo que hace es que se ocupe un porcenaje de la pantalla dependiendo que valor le demos, si ponemos width 50vw ocupara el 50% de la pantalla.

margin 0 auto:agrega un margin automatico de izquierda a derecha pero no de top y bottom, este margin centra de manera automatica el container donde lo pongamos

max y min sirven para el responsvie tambien sirve para solucionar problemas de overflow: esto quiere decir que tenemos mas texto de lo que puede tener el container.


POSITION


![image](https://user-images.githubusercontent.com/101487602/159171055-2b1add17-2254-4bb0-ba30-98a903bed475.png)

RETO DUPLICAR LO DE LA IMAGEN.

![image](https://user-images.githubusercontent.com/101487602/159171071-6ecee5d7-9942-418d-95a2-8c37abe111fa.png)


Todas las etiquetas html vienen por defecto con la posicion static osea se quedan donde tu las pones.

absolute:

Display-----------

display inblock lo que hace es que la etiqueta ocupa todo el espacio frente a ella

display in line lo que hace es que la etiqueta ocupa solo lo que necesita y deja el resto libre para otras etiquetas, a los elementos in line no se les puede agregar ni margin padding top o botom

pero en los elementos de inlineblock si pueden, combina los mejor de los 2.

RETO HACER UN LAYOUT COMO EL DE LA IMAGEN con css vanila y despues hacerlo con flexbox:

![image](https://user-images.githubusercontent.com/101487602/159171767-07cfe3de-261f-4d8e-b73e-c0a0c9052c26.png)


display flex: es flexible y deja hacer lo de inline block mirar clase flex,clase display.

con flex-direction podemos cambiar la posicion de columasn y filas.

flex-wrap:wrap sirve para que se autoacomode el contenido sin importar que tan grande sea el contenedor.

justify content:center: ayuda a alinear el contenido de forma horizontal.tambien exitste el space evenly que deja un espacio entre cada uno de los objetos, incluyendo la margenes.


flexbox layouts:

Todos los contenedores a los cual no se les ponga un order se van a pasar automaticamente a ala izquierda y los que tenga un order empiezan del primero hacia la derecha.

flexgrow: hace crecer el item que tenga la regla y es responsive

-----------------------------------------------

Variables o custom properties:mirar la claseVariables alla hay comentarios de como hacerlo.


FONTS Y WEB FONTS

Fuente genericas ya instaladas y seteadas en tu pc y navegador:

Se pueden buscar fuentes en google fonts

![image](https://user-images.githubusercontent.com/101487602/159173659-a39d960a-2ad3-497a-a617-c398d5dd5817.png)

las fuentes de google fonts es mejor ponerlas con link en el header como si se tratara de una hoja de estilos.

![image](https://user-images.githubusercontent.com/101487602/159173824-b84d86f3-fd8c-4833-9362-27a4b02180e9.png)


