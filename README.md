# Markdown
Markdown es un lenguaje de marcado ligero creado en 2004 por John Gruber, trata de conseguir la máxima legibilidad y facilidad de publicación tanto en su forma de entrada como de salida, inspirándose en muchas convenciones existentes para marcar mensajes de correo electrónico usando texto plano.

Facilita la aplicación de formato y estilo a texto plano empleando una serie de caracteres de forma especial.

El objetivo de su creador fue hacer que la gente pudiera escribir usando un formato de texto plano fácil de leer, fácil de escribir y con la posibilidad de convertir su documento en HTML válido.

La gran simpleza de su sintaxis hizo que tuviera una rápida adopción y popularidad en la comunidad de desarrolladores.

Actualmente aparte de permitir generar contenido HTML de forma dinámica, también se emplea (casí de forma estándar) para la creación de documentación técnica y con la proliferación de la arquitectura JAM Stack para la creación de sitios estáticos a través de herramientas de tipo SSG (Static Site Generator) y SSR (Server Side Rendering) como Hugo, Gatsby, Eleventy, Next.js, Sergey, Astro, entre otros, Markdown se ocupa para la generación de contenido editorial (artículos de blog) de forma dinámica.

## Aprendiendo _Markdown_
El símbolo "#" al comienzo de una línea, indica que se trata de un encabezado de nivel 1 en HTML.

Cuando se encierra una palabra entre guiones bajos (_) estamos indicando que se trata de una palabra escrita en cursiva. Esto se puede utilizar, por ejemplo, cuando utilizamos palabras ajenas al idioma.

Ambos casos se ven ejemplificados en el título de esta sección.

## Párrafos
Esto es un párrafo. A la hora de dar _Enter_, se divide el texto en párrafos.

Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quo, doloremque voluptate. Possimus nisi nostrum quidem ducimus nesciunt. Hic aliquid ipsa earum odio deserunt magni sint neque, repellat minus fugiat provident?

Este es otro párrafo.

## Cursivas y Negrita
Como se vió antes, _para aplicar cursiva se usan guiones bajos_ (\_de esta manera\_); y **para aplicar negrita, se usan ateriscos dobles** (\*\*de esta manera\*\*). **_Aplicando ambos_**, esto se consigue aplicando negrita a la cursiva (\*\*\_de esta manera\_\*\*).

# Encabezado nivel 1
## Encabezado nivel 2
### Encabezado nivel 3
#### Encabezado nivel 4
##### Encabezado nivel 5
###### Encabezado nivel 6

**NOTA:** Para que los encabezados apliquen, se debe dejar un espacio en blanco ' ' entre el último # y el texto.

## Enlaces
Se utilizan dos juegos de caracteres: corchetes [ ] y paréntesis ( ). Los corchetes son utilizados cuando se requiere que se visualice un texto para el link, y entre paréntesis el link en sí. Por ejemplo: [YouTube](https://www.youtube.com/).

Para enlaces internos al documento _Markdown_, por defecto, los encabezados mediante el símbolo # ya generan un enlace a dicho bloque de texto. Entonces, si quiero utilizar un enlace hacia otro bloque de texto del documento, se utilizan los dos juegos de caracteres (corchetes y paréntesis), pero dentro de los paréntesis se pone el encabezado al que se hace referencia. Por ejemplo: [Aprendiendo _Markdown_](#aprendiendo-markdown).

**NOTA:** Para los enlaces internos, cuando el enlace lleva está conformado por más de una palabra, se utilizan guiones medios (-) como separador.

[Este enlace lleva a la sección párrafos](#párrafos).

## Imágenes
Para utilizar imágenes que se encuentran dentro del mismo proyecto, se _linkean_ como se acostumbra en lenguajes como HTML, CSS o JS, por ejemplo. Para diferenciar la imágen de un enlace normal, se utiliza el símbolo de exclamación (!) antes de los corchetes [ ].

También se pueden llamar imágenes desde internet, como la siguiente, que es una imagen de la categoría Animals del sitio [PlaceIMG](https://placeimg.com/).

![Animals](https://placeimg.com/200/200/animals).

## Divisiones
Para realizar una división se utilizan tres guiones medios seguidos (---).

---

Este es otro texto.

---

Estas divisiones son equivalentes a la etiqueta hr de HTML. 

**NOTA:** Si no se deja una línea en blanco entre las divisiones, el texto adyacente se convierte en un encabezado.

## Listas
### Listas ordenadas
Consisten en ingresar un número seguido de un punto. Por ejemplo:

1. Primer elemento de la lista
2. Segundo elemento de la lista.
3. Tercer elemento de la lista.

## Listas desordenadas
Se utiliza el asterisco o un guión medio sin el punto. Debe haber un espacio en blanco entre el caracter y el texto. Por ejemplo:

* Elemento
* Elemento
* Elemento

- Elemento
- Elemento
- Elemento

## Sublistas
- Otoño
    * Marzo
    * Abril
    * Mayo
- Invierno
    * Junio
    * Julio
    * Agosto
- Primavera
    * Septiembre
    * Octubre
    * Noviembre
- Verano
    * Diciembre
    * Enero
    * Febrero

## Citas
Para incluir citas se utiliza el símbolo de "mayor que" >.

Esto es una cita de línea:
> Siempre tienes opción de no tener opinión. - Marco Aurelio

Esto es una cita de bloque:

> Todo lo que escuchamos es una opinión, no es un hecho.
>
> Todo lo que vemos es una perspectiva, no la verdad.
>
> Marco Aurelio

## Tablas
Se utiliza un _pipe_ ( | ) para delimitar el borde de la tabla. Se debe tener una fila principal, como un encabezado. Luego, se debe utilizar divisiones para, justamente, dividir la fila encabezado del resto de filas.

|   Nombre  |   Edad    |       Correo      |
|   ---     |   ---     |       ---         |
|   Gordon  |   37      |    gman@gmail.com |
|   Fulano  |   145     | fulano@hotmail.com|
|   De Tal  |   19      | detal@outlook.com |

## Códigos
Si para un artículo técnico, por ejemplo, se necesita introducir piezas de código, se puede introducir en línea o en bloque, al igual que las citas.

Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quo, doloremque voluptate. Possimus nisi nostrum, `let ` quidem ducimus nesciunt. Hic aliquid ipsa earum odio deserunt magni sint neque, repellat minus fugiat provident?

Se puede apreciar el uso de los tildes graves para encerrar la palabra reservada _let_ dentro de un fragmento de código en línea.

Si se necesita encerrar un bloque de código, se delimita el código con tres tildes graves al inicio y tres al final.

Adicionalmente, si se conoce el lenguaje de programación con el que se está trabajando, se puede indicar después de los tres primeros tildes, la extensión del tipo de documento correspondiente al lenguaje.

```js   
function sumar (a,b) {
    return a + b;
}
```

Si en un documento md queremos escribir código HTML, automáticamente va a funcionar, pues soporta sus etiquetas. Por ejemplo, un formulario a modo de barra de búsqueda:

<form>
    <label for="q">Buscar:</label>
    <input type="search" name="q" id="q">
</form>

## Comentarios
Los comentarios se definen de igual manera que en HTML.
<!-- Esto es un comentario en _Markdown_ -->

## Escape de caracteres
Cuando se requiere representar en algún artículo los símbolos que se utilizan para delimitar la negrita o la cursiva, para escapar los caracteres se utiliza la barra invertida " \ ".

Por ejemplo, para escribir en cursiva debemos delimitarla con dos guiones medios, de esta manera: \_cursiva\_. Lo mismo sucede para la negrita, esto es: \*\*negrita\*\*.