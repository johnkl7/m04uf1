# Código y documentación M04-UF1 
Ciberseguridad: Lenguaje de marcas m04uf1

## XML

### _Aqui iran los apuntes de **XML**_


La cabezera en cada archivo tiene que ser contener lo siguiente: 
```XML
<?xml versión=”1.0” enconding=”UTF-8?>
```

Existen dos tipos de etiquetas:
* ```<class></class>```: Etiquetas par. Se cierra con otra etiqueta.
*  ```<age value = "197" />```: Etiquetas impar. Cierra la misma etiqueta.

Una vez se ha creado un tipo de etiqueta u otro para un personaje, todos deben tener la misma.

### __VALIDACIÓN__

Hay dos formatos de archivo que nos permiten validar XML:
* XSD
* DTD

DTD es el mas utilizado hoy en dia. Ocupa menos y no hace falta introducir tantas etiquetas.

## DTD
Los _apuntes_ de DTD




## MARKDOWN

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





