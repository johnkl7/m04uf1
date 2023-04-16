# Código y documentación M04-UF1 John Largao
Ciberseguridad: Lenguaje de marcas m04uf1

## APUNTES LENGUAJES DE MARCAS UF1

## SMGL

SGML fue el primer lenguaje de marcado estandarizado a nivel internacional. Fue creado en los años 80. SGML fue creado para la creación de documentos electrónicos estructurados y complejos. Este lenguaje sentó las bases para la
creación de otros lenguajes de marcado, como HTML, XML y otros. 

Después de SGML vino HMTL con los enlaces en los años 90 y fue muy popular. Pero hubo un problema. Mosaic (1993) fue publicado por el creador de HTML. Netscape salió después.
Microsoft compro una empresa y le cambio el nombre al navegador que tenía esa empresa y nombraron al navegador Internet Explorer. Microsoft se cargó a Netscape imponiendo internet Explorer en todos sus ordenadores,
además venía en el núcleo o kernel del sistema por lo que no se podía desinstalar. Internet Explorer interpretaba HTML muy mal. Netscape lo hacia respetando los estándares. Los desarrolladores se adaptaron a como hacia las cosas Explorer y Netscape murió.
Netscape libero su código fuente que se llamaba Mozilla y salieron proyectos como Firefox.
>Netscape había hecho tan bien el motor, que hacer que interpretara las malas prácticas de Microsoft fue imposible, y murió.</br>
![IE vs NS](https://www.mindfiresolutions.com/blog/wp-content/uploads/netsVsIE11.png)

## XML 

Después de HTML 4 se creó XML, se creó para dictaminar unas reglas muy rígidas que se tienen que cumplir, pero a la vez flexibles para ofrecer al usuario hacer más cosas y libertad. XML se creó más bien para establecer las normas y después tu "puedes crear tu propio
lenguaje de marcas". **No impone visualización, impone estructura**. XML es un formato de transporte.
La cabecera de cada archivo tiene que ser la siguiente: 
```XML
<?xml versión=”1.0” encoding=”UTF-8?>
```

Ejemplo de código XML: 

```XML <?xml version="1.0" encoding="UTF-8" ?>
<character>
	<name>Messi</name>
	<surname>Mendoza</surname>
	<!-- COMENTARIO -->
	<age years="50" />
	<race>Gigante</race>
	<class>Healer</class>
	<gender abbrev="N">Non-binary</gender>
	<height cm="1.6" />
	<weight kg="1000" />
	<language abbrev="EUK">Portugués</language>
	<tienelaeso />
</character>
```

### __VALIDACIÓN__

Hay dos formatos de archivo que nos permiten validar XML:
* XSD
* DTD

**DTD** (Document Type Definition) y **XSD** (**XML** Schema Definition) son dos formatos que se utilizan para validar documentos XML. Ambos formatos describen la estructura y contenido de un documento XML y especifican las reglas que deben cumplir los elementos
y atributos del documento.
DTD es un formato más antiguo que XSD y es más simple de utilizar. Una DTD se define como un archivo de texto que contiene una serie de reglas para la validación del documento XML.
La DTD define los elementos que pueden aparecer en el documento XML y cómo estos elementos se relacionan entre sí. La validación de un documento XML con una DTD se realiza mediante la verificación de que el documento cumple con las reglas especificadas en la DTD.
A pesar de que es más simple, las DTD presentan algunas limitaciones, como la imposibilidad de validar los tipos de datos o de definir restricciones más complejas.</br>
Por otro lado, XSD es un formato más reciente y complejo que DTD.
XSD define un esquema XML que describe la estructura y contenido del documento XML. Los esquemas XSD son más flexibles que las DTD y permiten la definición de tipos de datos personalizados y restricciones más complejas. Además,
los esquemas XSD pueden ser utilizados para validar los datos introducidos en los formularios web, lo que los hace especialmente útiles en aplicaciones de comercio electrónico y otras aplicaciones web.
Aunque las DTD han sido más utilizadas históricamente debido a su simplicidad, los esquemas XSD se están convirtiendo en la opción preferida para la validación de documentos XML debido a su mayor flexibilidad y capacidad para manejar casos más complejos
de validación. DTD es el más utilizado hoy en día. Ocupa menos y no hace falta introducir tantas etiquetas.

### WWW

Antes de saber acerca de WWW (www.google.es), tenemos que saber que es el **.es**. A esto se le llama TLD (Top level domain). Cuando introducimos una página web como la anterior en el navegador, lo primero que se lee es el **.es** .
El DNS se guarda el TLD, de esta manera es más rápido y fácil de clasificar. Todos los servidores de DNS empiezan a leer por el TLD.
Al principio solo había 3 TLDs : 
* .com 
* .edu 
* .net

**Todos ellos pertenecían a Estados Unidos, que se los quisieron quedar para ellos aunque al final no pudieron**

Ponemos **WWW** para diferenciarlos del resto de servicios. Antes se podía acceder por el navegador a una web y utilizar FTP para transferir archivos (*ftp.ubuntu.com*). WWW remarca que cuando nos conectamos a esa dirección, con ese prefijo, nos vamos a conectar al puerto **80** .
Actualmente si por ejemplo entramos a enti.cat, el navegador utiliza HTTPS (no HTTP) y utiliza el puerto correspondiente. Hoy en día no se le da importancia a veces a WWW. Lo más habitual es:

* Mantenerlo y que se vea.
* Hacer una redirección de salto.

## HTML 5 o LifeScheme
> Life scheme hace referencia a que está continuamente evolucionando

HTML es el lenguaje de marcas más popular hoy en día. Se creó para usarse con HTTP. 
* HTTP salió en 1991.
* HTML en el 1993.

En 1991 Tim Berners-Lee creo HTTP y con ello las bases de HTML. Hasta ese entonces (1991) no había herramientas para comunicarse o transferir información por Internet.
Finales de los años 90 mediados de los 2000 se impuso flash, que era un software privativo que ofrecía animaciones, multimedia etc. Flash controlaba todo el sector, no tenía competencia por lo que había muchos agujeros de seguridad.
HTML 5 (2008) vino como un borrador, trajo etiquetas importantes como la etiqueta video, ya no hacía falta flash para poner video web, pero cada uno utilizaba el formato que quería. Las etiquetas de audio permitían audio.
Internet Explorer se dejó de utilizar porque los dispositivos móviles utilizaban navegadores con HMTL 5. HTML 5 mato a internet Explorer.  En el año 2012 Microsoft decidió crear otro navegador: Edge. La primera versión era exactamente igual de mal que Explorer,
mejoraron el rendimiento, pero seguía siendo igual de malo al interpretar los estándares. Edge se empezó a usar un poco pero luego cayo.  Microsoft utilizo Chromium para crear un nuevo navegador.

Internet explorer estuvo en guerra con Netscape, otro navegador, y se lo cargo.
Cuando murió Netscape, fue liberado por la fundación Mozilla. Su objetivo es hacer un navegador que respete los estándares web. Después salieron Opera, Chrome y todos sus derivados.

>Firefox no depende de ninguna compañia (es open-source).
>Opera no es muy fiable por temas de seguridad.

Hoy en día todos respetan bastante el Life scheme.

Durante el HMTL4 y el LIFE SCHEME (5) hubo otro. XHTML, que consistía en:

* Una mezcla de XML y DTD.
* Algunas mejoras de HTML4.


### ETIQUETAS

Existen dos tipos de etiquetas:
* ```<class></class>```: Etiquetas par. Se cierra con otra etiqueta.
*  ```<age value = "197" />```: Etiquetas impar. Cierra la misma etiqueta.
Una vez se ha creado un tipo de etiqueta u otro para un personaje, **todos** deben tener la misma.

**Todos los documentos HTML empiezan con un *index.html***.
Todo texto, todo elemento tiene que ir dentro de una **etiqueta o elemento de bloque**. Esta sería la etiqueta de párrafo:
* ```<p>ola k ase</p>``` 
Para poner un texto en cursiva utilizamos ```</em>```, **la semántica es lo que aporto HTML 5**.
* ```<h1></h1>``` : Cabeza número 1. Es el titulo de la pagina.
* ```<h2></h2>``` : Cabecera número 2. Dentro de esta puede haber h3,h4...
* ```<img />```: Para las imágenes, esta etiqueta se cierra solo con la contra barra. Se utiliza **src** para indicar el link de la imagen.
Todo documento HTML tiene una etiqueta raíz. La etiqueta raíz de HTML es ```**<html></html>**``` . Pero a la vez dentro de todo documento HTML, tiene que haber dos etiquetas más obligatorias:

* ```<head></head>``` : Va la información de como se tiene que interpretar cosas dentro del body o de la página misma. Aquí dentro van etiquetas como ```<title></title>``` , ```<style></style>``` (*estas dos etiquetas son siblings, ya que están al mismo nivel*)
* ```<body></body>``` : Abre y cierra los contenidos.

>Head y body son etiquetas hermanas o siblings en inglés, ya que están en la misma parte del árbol. Las etiquetas que están en el mismo nivel son etiquetas hermanas.

* ```<title></title>``` : Se utiliza para el título de la pestaña.

La primera línea de todas es el DTD. Esta línea la tiene que tener todo documento HTML. Si no introducimos esta línea habrá problemas de **compatibilidad y lo interpretara mal**.
> ```<!DOCTYPE html>```

* ```<marquee></marquee>``` : Con esta etiqueta se mueve el texto por la pantalla. 
* ```<blink></blink>``` : Con esta etiqueta el texto parpadea.
* ```<blockquote></blockquote>``` : Es para hacer texto mas especial, como citas.
* ```<form></form>```
* ```<input></input>``` : Permite introducir valores.

### TIPOS DE ELEMENTOS
* Elementos en bloque: h1,h2,p ... Los elementos en bloque fuerzan el salto de linea. Son como cajas.
* Elementos en línea : **strong**(hace el texto en negrita, refuerza el texto), _em_ ... **Los elementos en línea van dentro de los elementos en bloque.**
>Los elementos en línea(```<a>```) no tienen margin, padding, width, height ...

### LISTAS
Las etiquetas **ul** se utilizan para hacer listas. 
* ```<ul></ul>``` : lista sin ordenar (**unordered list**)
* ```<ol></ol>``` : lista ordenada (**ordered list**)
* ```<li></li>``` : li se utiliza para los elementos de la lista. (**list item**). Siempre va dentro de o **ul** u **ol**.

Ejemplo:

```HTML 
<ul>
	<li>Manzanas</li>
	<li>Peras</li>
	<li>Limones</li>
</ul>

<ol>
	<li>Limones</li>
	<li>Arbol</li>
	<li>Naranja</li>
</ol>
```

### ENLACES
* ```<a></a>``` : La etiqueta "a" se utiliza para realizar enlaces, para el **hipertexto**. Es una etiqueta en línea. Se pueden incrustar imágenes, videos, audios etc.
* Se utiliza **href** para hacer referencia al enlace.
* Se utiliza **alt** para insertar un texto alternativo.
* Con el **title** es el texto que sale cuando pasamos el ratón por encima.

El texto alternativo sirve para que el enlace siga funcionando aunque la imagen no cargue.


### BLOQUES LOGICOS

* ```<header></header>``` : Es una etiqueta semántica, no aporta nada visual inicialmente. Header no es como ```<head>```, header esté ya dentro del body, es la "cabeza" del body.
>**La semántica significa lo que es y lo que significa. Es el significado de lo que escribimos más allá del propio texto.**
---
* ```<main></main>``` : Aquí van los contenidos del cuerpo.
* ```<footer></footer>``` : Es el pie de página.
* ```<nav></nav>``` : Proporciona enlaces de navegación. Esta etiqueta puede estar en cualquier elemento. Dentro del de header, main, del footer.
>Todas estas etiquetas son siblings.


### ID

ID identifica un elemento de una página de manera única. Cada vez que queramos acceder a un elemento y sus propiedades utilizaremos su ID.
```<p id="numerito">ESTO ES EL HTML INTERNO DE P</p>```: INNERHTML es el texto interior que contiene y que después puede ser utilizado para cambiar su contenido con JavaScript.


## CSS (CASCADE)
Se decide "en cascada", porque todo va afectando a lo siguiente, no hace falta volver a definir las propiedades de una etiqueta de nuevo.

* ```<style></style>``` : Esta etiqueta nos permite cambiar el estilo. Se utiliza con **CSS**
Todo elemento de bloque tiene:
* MARGIN: Margen exterior. 16px(arriba) 0(derecha) 128px(abajo) 20px(izquierda). Funciona como las agujas del reloj. El **px** se tiene que especificar a no ser que el valor sea 0, ya que se puede trabajar con varias unidades a parte de px.
* PADDING: Margen interior.
>Las etiquetas que editamos dentro de la etiqueta style las llamamos **selectores**.
>El body a su vez tiene su propio MARGIN. Está empujando hacia fuera.


>HTML es la estructura, CSS la forma, JavaScript la acción. 

* ```<link />```: Esta etiqueta permite referenciar ciertas configuraciones como por ejemplo la configuración de la etiqueta ```<style></style>``` o las hojas de estilo. Se utiliza **rel** para referenciar el nombre y **href** para introducir el nombre del archivo.
Displays: Es como se muestran los elementos en bloque.
* BLOCK 
* INLINE
* NONE
* FLEX : Cuando un elemento en bloque pasa a ser flexible los elementos en bloque que hay dentro se vuelven flexibles también.


## JAVASCRIPT

JavaScript es un lenguaje de programación que se utiliza principalmente para crear aplicaciones web interactivas y dinámicas. Habitualmente se utiliza con HTML y CSS para crear dichas aplicaciones web. HTML se utiliza para estructurar y dar formato</br>
al contenido de la página, CSS se utiliza para dar estilo y diseño, y con JavaScript añadimos acción, interactividad, dinamismo.

### VARIABLES

Para definir variables en JavaScript se utiliza la palabra reservada "let". No se indica el tipo de dato con el que tratamos, por lo tanto, utiliza un **tipado débil**. Esto quiere decir que es posible cambiar el tipo de dato de una variable de manera directa.
También se puede concatenar varios tipos de datos distintos.
Todas las variables por defecto ya existen, lo que pasa que están en estado "undefined" si no les asignas ningún valor.

### BUCLES

```js
for (let i=0; i < 10; i++){
	console.log(i)
	}
```

```js
let valor1 = 10;
let valor2 = 6;
	
	if (valor1 == valor2){
		console.log("Son iguales");
	}
	else if (valor1 > valor2){
		console.log("El valor1 es mayor");
	}
	else {
		console.log("El valor2 es mayor")
	}
```


```js
let contador = 0;
	while (contador < 10 ){
	console.log(contador)
	contador++;
	}
```


### FUNCIONES

```js
function saluds (){
	console.log("ola k ase");
}
saluda();	
```

En java script los parámetros son opcionales, por general no usarlos dará error, pero muchas veces imprimirá el resto del contenido. 

setInterval: Es una función que ejecutara algo especifico (una función, por ejemplo) que le pasamos por un parámetro, en el segundo parámetro indicaremos los milisegundos que se utilizaran de intervalo. 
```setInterval(cuenta,1000);```

clearInterval: Con esta función se para el intervalo.

>No se puede poner el mismo nombre a un id y una función.

### EVENTOS

JavaScript es un lenguaje orientado a objetos y eventos. Programamos cosas que esperan a que sucedan cosas o eventos.

```<input type="button" value="¡¡¡Clic!!!" onClick="alerta_maxima();"/>``` : En este caso el evento seria CLICK, que lanza la función alerta_maxima.
La etiqueta button tal cual actua como un submit. Para que el texto no desaparezca hay que poner **type="button"**.

### VARIABLE DOCUMENT

Contiene todos los elementos de la página. 

### PROPIEDADES

Cuando hacemos referencia a varias propiedades (color,background por ejemplo), a diferencia de CSS donde se separan con un guion, en JavaScript se escriben las dos palabras juntas con la primera letra de la segunda en mayúscula. ```.backgroundColor```

style: Sirve para acceder a los estilos. Contiene todos los estilos de un elemento incluso los que no están seteados.
* .color = color de la fuente.
* .backgroundColor: para cambiar el color de fondo. 

### FUNCION FETCH

JavaScript permite descargar archivos de nuestro servidor o otros de manera asíncrona para obtener datos. Significa que puede ocurrir independientemente del momento de la carga, cuando se llega al fetch dentro del código, se ejecuta
otro hilo de ejecución y fetch se ejecuta aparte y va haciendo sus cosas. De esta manera, el codigo no espera a que acabe el fetch, los dos hilos funcionan independientemente, fetch funcionando en segundo plano.
Cuando una función asíncrona termina no nos devuelve los datos directamente, lo hace de otra manera, devolviéndonos una promesa que después convertimos en un objeto.

## JSON 

JSON (JavaScript Object Notation) es un lenguaje orientado al intercambio de datos. Es muy popular debido a su simplicidad y capacidad para ser interpretado por varios lenguajes de programación.
Con JSON abrimos y cerramos con llaves, no utilizamos etiquetas como en HTML.

| Lenguaje | name | 
| ---: | ---: |
| HTML | ```<name></name>```| 
| JSON | "name" |

JSON es más ágil (es puro JavaScript), no se utilizan validadores, es por eso que en entornos de trabajo como bancos se utiliza HTML en vez de JSON. Muchos bancos y amazon tienen los datos
almacenados en ambos (xml y json). Nos envían los archivos a nosotros en JSON para que sea más rápido, pero cuando pasa algo tienen los datos guardados en HTML.



