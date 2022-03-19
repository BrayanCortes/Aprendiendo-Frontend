Paginas staticas:son aquellas en las que el usuario no hace cambios, como los vlogs

Paginas dinamicas:son aquellas con las que el usuario interactua, hace cambios, como twitter y facebook

Anatomia de una pagina web:

Container:

    Header:Donde va el logo, el nombre del a empresa o el titulo de la pagina web, tambien esta el area de navegacion como los menus.
    
    Main Content:Donde va toda la informacion que se pondra en la pagina, esta puede tener un SideBar donde se pone otra informacion como un chat o noticias.
    
    Footer:Es el final de la pagina web donde se pone el email de contacto o los creadores y el año de creacion de la misma.

Poniendo imagen:

![Anatomia-web](https://user-images.githubusercontent.com/101487602/159049844-e889270e-4638-4ed0-bf8c-2ad850082e8f.PNG)

La paginas principal del html debe llamarse index que es lo que se encontrara cuando las busquen.

identar bien el html para que se pueda leer de manera mas sencilla

con meta name description, content podemos poner la descripcion de la pagina web para cuando la busquen en el navegador sea mas sencillo de saber que hay en la pagina web

en html hay 2 tipos de etiquetas:

1.etiquetas contenedoras:Son las que llevan mas etiquetas adentro y ayudan a generar la estructura como se vio en la anatomia eje: Header,main,footer,div

2.etiquetas contenedoras:Son las que llevan lo que se renderiza en la paginas, imagenes, texto, videos. ej: h1

existen 6 tipos y tamaños de titulo del h1 al h6

la etiqueta a sirve para los links

ETIQUETAS MAS USADAS HTML:
Fuente:platzi.com

article: diferencia partes del contenido que pueden vivir por sí mismas.

nav: para hacer menús de navegación.

aside: contenido menos relevante, como publicidad, etc.
section: sirve para diferenciar las secciones principales del contenido.

header: cabecera del documento.

footer: pie de página del documento.

h1 - h6: títulos de nuestro sitio web.

table: tablas de contenidos, similar a la estructura de las hojas de calculo.

ul y ol: listas de items.

div: cualquier división para organizar el contenido.

h1 a h6: son etiquetas para indicar títulos con un estilo que destaca del resto.

article: es la parte de nuestro contenido que puede vivir por sí mismo. Pueden haber tantos artícle como proyectos o eventos tenga nuestro portafolio.

p: define el texto de un párrafo.

small: aplica una apariencia de texto reducido en tamaño.
strong: aplica al texto un formato de negritas.

a: corresponde a un ancla o enlace a una url interna o externa del documento.

img: con esta etiqueta podemos enlazar imágenes en el documento.
figure: le da un contexto semántico a las imágenes.

anatomia de etiquetas: 

![image](https://user-images.githubusercontent.com/101487602/159069392-ae4de200-d369-4126-bc03-0d3de1f75794.png)

algunas etiquetas llevan etiqueta de cierre porque llevan un contenido adentro en este caso la etiqueta de link, dice a que pagina nos llevara el link.la parte que esta entre la etiqueta de apertura y cierre se le conoce como contenido.

el atributo puede ser pasivo que solo lleva una letra o palabra y atributos compuestos que llevan el nombre y el valor del atributo.

CONTENIDO MULTIMEDIA HTML:

Tipos de imagen:

![image](https://user-images.githubusercontent.com/101487602/159071513-bd68758c-fe44-4382-b795-3368ea92252e.png)



existen 2 tipos de imagenes, lossy vs lossless

con perdida y sin perdida esto hay que tenerlo en cuenta porque si usamos imagenes sin perdida nuestra pagina web se va a abrir muy lento por lo que daremos muy mala experiencia a los usuarios

Lossless

los formatos de imagen sin perdida capturan todos los datos de su archivo original, No se pierde nada del archivo original, foto o obra de arte, de ahi el termino "Sin perdida". el archivo puede estar comprimido, pero todos los formatos sin perdida podran recontruir su imagen a su estado original.No se pierde calidad

Lossy

Los formatos de imagen con perdida se aproximan a su imagen original por ejemplo, una imagen con perdida podria reducir la cantidad de colores en su imagen o analizar la imagen en busca de datos innecesarios,Esto reducira el tamano del archivo auqnue pierda calidad de la imagen.


Optimizando imagenes

Tamaño optimo de peso de una imagen en un proyecto web:

Tamaño promedio: de entre 70KB y 100KB

Para optimizar imagenes utilizar:

    Tiny png que mejora el tamaño de las imagenes

    Verexif que retira metadatos de las imagenes

PONER IMAGENES EN HTML

Etiqueta img:

cuando usamos la etiqueta img en html esta nos pide un src que significa una fuente de imagen, osea de donde va a traer esa imagen y un alt que sirve para cuendo la imagen no cargue dar una descripcion de lo que se veria, sirve para el tema de accesibilidad.


Etiqueta figure:

el figure sirve para acomodar bien la imgaen y el figcaption sirve para poner una descripcion de la imagen justo debajo para que las personas sepan que es eso, incluso se puede podern el autor de la imagen o de la pagina web.

VIDEOS

con la etiqueta video, donde dice src se pone el video el cual debe estar dentro del proyecto para que se reproduzca, no sirve un link, tambien tiene atributos como controls los cuales dan los controles para ver un video como lo son, play,adelantar,la barra de duracion y el tiempo de duracion, tambien hay otro que se llama preload, este preload ayuda a que el video se renderize cuando se empieza a cargar la pagina esto ayuda a que no existan tiempos de espera muy altos.

dentro del src podemos poner lo siguiente como ejemplo #t=10,60 esto lo que significa es que el video empezara a reproducirse en el segun 10 y se pausara automatico en el segundo 60.

la etiqueta de source se usa para poner los diferentes formatos, lo que se hace es que se quita el src de video y se pega en source con los diferentes formatos de video, en la etiqueta de video solo dejamos los atributos como controls o preload, pero el src se pone en source.

![image](https://user-images.githubusercontent.com/101487602/159078171-d09ea88b-1683-4550-9e7f-18d980a21aa6.png)


Chrome respeta la jerarquia por lo que siempre escoge el de mas arriba siempre y cuando entienda ese tipo de formato

------FORMULARIOS E INPUT--------

con el input primero se crea un label, en el for del label ponemos el nombre del atributo y en el id del input debemos poner el mismo nombre que pusimos en el label.mirar claseForms index.html para entender mejor, se hizo con nombre.

con el atributo name mandamos la informacion,debe tener el mismo nombre que el for del label y el id del input




