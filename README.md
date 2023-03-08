# Código y documentación M04-UF1 
Ciberseguridad: Lenguaje de marcas m04uf1

## XML - _Aqui iran los apuntes de **XML**_

n entre sistemas de computación, como sitios web, bases de datos y aplicaciones de terceros. Las reglas predefinidas facilitan la transmisión de datos como archivos XML a través de cualquier red, ya que el destinatario puede usar esas reglas para leer los datos de forma precisa y eficiente.

### EJEMPLO DE CODIGO XML

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

### CABEZERA

La cabezera de cada archivo tiene que ser la siguiente: 
```XML
<?xml versión=”1.0” encoding=”UTF-8?>
```

Existen dos tipos de etiquetas:
* ```<class></class>```: Etiquetas par. Se cierra con otra etiqueta.
*  ```<age value = "197" />```: Etiquetas impar. Cierra la misma etiqueta.

Una vez se ha creado un tipo de etiqueta u otro para un personaje, todos deben tener la misma.

### __VALIDACIÓN__

Hay dos formatos de archivo que nos permiten validar XML:
* XSD
* DTD

>DTD es el mas utilizado hoy en dia. Ocupa menos y no hace falta introducir tantas etiquetas.

## DTD
Los _apuntes_ de DTD





## MARKDOWN
Markdown es un lenguaje de documentacion

### LISTAS

* uno
* dos 
	* sub apartado de 2
	* otro más
* tres

> Un gran poder conlleva
>
> una gran responsabilidad.
>
> - Confucio 2024

>**Esto es una cita**
>>Esto es una cita dentro de una cita
>
>Seguimos

---

Un enlace a la mejor web del mundo:

[CondorChem](https://conderchem.com)
Y [ESTO](https://enti.cat) es otro enlace.
### Imagen incrustada
![Imagen incrustada](https://pm1.narvii.com/6826/133204a8158cd924c60e39e50abd5dc0b0b24173v2_hq.jpg)

```kotlin
fun main (args: Array<String>) {

print("Enter a number: ")
// reads line from standard input keyboard
// and !! operator ensures the input is not null
val stringInput = readLine()!!

//converts the string input to integer
var integer:Int = stringInput.toInt()

println("You entered = $integer)}
```

### Listas de tareas
- [ ] Primera tarea
- [x] Segunda tarea
- [ ] Tercera tarea

### Carácteres extendido

:yum: :flushed:

## Estilo de carácteres

*cursiva* _cursiva_

**negrita** __negrita__

~~TACHADO~~

~~***tachado negrita y cursiva***~~


### Tablas

| id_character | name | age | level |
| ---: | ---: | ---: | ---: |
| 1 | Eustaquio | 197 | 99 |
| 2 | Mariana | 20 | 100 |
| 3 | Mortadelo | 100 | 1 |
| 4 | Messi | 44 | 32 |

### Escapar caracteres

\# ejemplo de escapado

\*que en otras cosas*


## HTML (Hypertext Markup Language)

Se creo para usarse con HTTP. 
* HTTP salio en 1991.
* HTML en el 1993.
>En 1991 Tim Berners-Lee creo HTTP y con ello las bases de HTML. Hasta ese entonces (1991) no habia herramientas para comunicarse o transferir información por Internet.


### WWW

Antes de saber acerca de WWW (www.google.es), tenemos que saber que es el **.es**. A esto se le llama TLD (Top level domain). Cuando introducimos una pagina web como la anterior en el navegador, lo primero que se lee es el **.es** .
>El DNS se guarda el TLD, de esta manera es mas rapido y mas fácil de clasificar. Todos los servidores de DNS empiezan a leer por el TLD.
Al principio solo habia 3 TLDs : 
* .com 
* .edu 
* .net

**Todos ellos pertenecian a Estados Unidos, que se los quisieron quedar para ellos aunque al final no pudieron**

Ponemos **WWW** para diferenciarlos del resto de servicios. Antes se podia acceder por el navegador a una web y utilizar FTP para transferir archivos (*ftp.ubuntu.com*). WWW remarca que cuando nos conectamos a esa direccion, con ese prefijo, nos vamos a conectar al puerto **80** .
Actualmente si por ejemplo entramos a enti.cat, el navegador utiliza HTTPS (no HTTP) y utiliza el puerto correspondiente. Hoy en dia no se le da importancia a veces a WWW. Lo mas habitual es:

* Mantenerlo y que se vea.
* Hacer una redireccion de salto.


### Empezando HTML (HTML 5 o LIFE SCHEME)

> Life scheme hace referencia a que esta continuamente evolucionando.
---
Internet explorer estuvo en guerra con Netscape, y se lo cargo.
Cuando murio Netscape, fue liberado por la fundacion Mozilla. Su objetivo es hacer un navegador que respete los estandares web. Despues salion Opera, Chrome y todos sus derivados.

>Firefox no depende de ninguna compañia (es open-source).
>Opera no es muy fiable por temas de seguridad.

Hoy en dia todos respetan bastante el Life scheme.

Durante el HMTL4 y el LIFE SCHEME (5) hubo otro. XHTML, que consistia en:

* Una mezla de XML y DTD.
* Algunas mejoras de HTML4.

>Netscape habia hecho tan bien el motor, que hacer que interpretara las malas practicas del Microsoft fue imposible, y murio.
![IE vs NS](https://www.mindfiresolutions.com/blog/wp-content/uploads/netsVsIE11.png)

### ETIQUETAS

**Todos los documentos HTML empiezan con un *index.html***.
Todo texto , todo elemento tiene que ir dentro de una etiqueta de bloque. Esta seria la etiqueta de párrafo:
* ```<p>ola k ase</p>```
Para poner un texto en cursiva utilizamos ```</em>```, la semantica es lo que aporto HTML 5.
* ```<h1></h1>``` : Cabeza numero 1.
* ```<h2></h2>``` : Cabezera numero 2.

Todo documento HTML tiene una etiqueta raiz. La etiqueta raiz de HTML es ```**<html></html>**``` . Pero a la vez dentro de todo documento HTML, tiene que haber dos etiquetas mas obligatorias:

* ```<head></head>``` : Va la información de como se tiene que interpretar cosas dentro del body o de la página misma.
* ```<body></body>``` : Abre y cierra los contenidos.

>Head y body son etiquetas hermanas o siblings en inglés ,ya que estan en la misma parte del arbol. Las etiquetas que estan en el mismo nivel son etiquetas hermanas.

* ```<title></title>``` : Se utiliza para el titulo de la pestaña.

La primera linea de todas es el DTD. Esta linea la tiene que tener todo documento HTML. Si no introducimos esta linea habra problemas de **compatibilidad y lo interpretara mal**.
> ```<!DOCTYPE html>```

* ```<marquee></marquee>``` : Con esta etiqueta se mueve el texto por la pantalla. 
* ```<blink></blink>``` : Con esta etiqueta el texto parpadea.

### TIPOS DE ELEMENTOS
* Elementos en bloque: h1,h2,p ... Los elementos en bloque fuerzan el salto de linea.
* Elementos en linea : strong,em ...


### LISTAS
Las etiquetas **ul** se utilizan para hacer listas. 
* ```<ul></ul>``` : lista
* ```<li></li>``` : li se utiliza para los elementos de la lista. (list elements)

Ejemplo:
```HTML 
<ul>
	<li>Manzanas</li>
	<li>Peras</li>
	<li>Limones</li>
</ul>
```

### ENLACES
* ```<a></a>``` : La etiqueta "a" se utiliza para realizar enlaces, para el **hipertexto**.
* Se utiliza **href** para hacer referencia al enlace.

El texto alternativo sirve para que el enlace siga funcionando aunque la imagen no carge.

