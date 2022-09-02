# Introduccion Markdown
El siguiente repositorio tiene como finalidad mostrar y explicar el uso del lenguaje MARKDOWN para la realizacion de archivos con extension .md.

___

Dentro de __MarkDown__ podemos encontrar tres tipos de *elementos basicos*, los cuales cada uno tiene su subclasificacion interna:
1. Elementos de bloque
  - Párrafos y saltos de linea
  - Encabezados
  - Citas
  - Listas
  - Bloques de código
  - Reglas horizontales
2. Elementos de Linea
  - Enfasis
  - Links/enlaces
  - Código
  - Imágenes
3. Multimarkdown
  - Abreviaciones 
  - Definiciones
  - Notas al pie de pagina
  - Tablas

___

## Elementos de bloque
### Párrafos y saltos de línea
En Markdown para generar un salto de línea hay que dejar simplemente un renglon vacio, lo que pasa es que como Markdown no soporta *dobles lineas*, si nosotros dejamos mas de un renglon vacio, estos se mostraran como uno solo.  
Si dejamos al final de cada renglon dos (2) espacios en blancos con la barra espaciadora, Markdown nos mantendran las lineas tal como pusimos en el codigo (si no dejamos estos espacios en blanco, se nos formateara todas las lineas en una sola).  

### Encabezados
Para disnguir el texto con los 6 tipos de encabezados que posee Markdown, solo hace falta poner la almohadilla/hashtag `#` antes de cada texto. Tambien se puede usar la misma cantidad de almohadillas que ponemos al principio para "cerrar" el encabezado, pero esto es opcional, ya que Markdown las cierra solas.  Otra manera de generar encabezados es utilizando el simbolo igual `=` para encabezados de "tipo 1 (#)" y guiones `-` para el "tipo 2 (##)"; estos irian en la de abajo de nuestro "encabezado", y la cantidad es arbitraria, ya que puede ser desde 1 hasta lo que nosotros queramos.  

### Citas
Estas se generan con el operador _mayor que_ `>` e irian al comienzo de nuestro bloque de texto a citar; en el caso de que una cita se componga de varios parrafos, tendriamos que poner en cada comienzo el simbolo correspondiente.  
Si se llegase a necesitar, se puede anidar citas (tener una dentro de otra), para esto tendriamos que agregar un operador más (la cantidad de operadores > es proporcional a la cantidad de "anidacion" que va a tener una cita).  
Para que en la cita podamos poner una linea en blanco, tendriamos que en esa "linea en blanco" poner la cantidad de operadores que estemos usando en esa jerarquia/anidacion. Ejemplo de uso:
~~~
> Aca tendriamos una cita.
>
> > Esta estaria anidada dentro de la 1er cita.
> 
> Hasta aca seria la 1er cita.
~~~

### Listas
Dentro de las listas tenemos:  
> Listas desordenadas  
> > Estas las podemos crear con el operador asterisco `*`, guion `-` o suma `+`.  
>  
> Listas ordenadas  
> > Estas las podemos crear utilizando un numero seguido de un punto `1.`.  

Cualquiera de los dos tipos de listas las podemos anidar, esto se lograria agregando una tabulacion y/o cuatro (4) espacios en blancos adelante del elemento que queramos anidar.  

### Codigos de bloques
Para poder generar un codigo de bloque al cual Markdown no formatearia y queramos que se distinga, lo que tenemos que hace es entre nuestro codigo colocar en la linea de arriba y en la de abajo el tres operadores virguilla `~~~`.

### Reglas horizontales
Estas se utilizan para separar secciones de una manera visual, la creacion de las mismas es utilizando los siguientes operadores:
- asteriscos `*`.
- guiones medios `-`.
- guiones bajos `_`.

Para generar estas reglas tenemos que poner 3 operadores de los que mencionamos previamente.  

---

## Elementos de linea
### Énfasis (negritas y cursivas)
Para "envolver" una porción de texto en cursiva solo hay que poner al principio y al final del texto 1 operadores de asteriscos `*` o guion bajo `_`; y si queremos que la porción sea "envuelva" en negrita tenemos que hacer lo mismo pero con 2 operadores. Por supuesto si queremos combinar la cursiva con la negrita, tenemos que usar 3 operadores al principio y 3 al final. (Es indistinto si usamos asteriscos o guiones bajos).

### Links o enlaces
Podemos agregar dos tipos de enlaces:
1. Enlaces en linea: estos estan en linea con el texto y los creamos escribiendo entre corchetes `[]` el texto enlazado al link yentre parentesis `()` el link en cuestión. Ejemplo: `[texto a enlazar](enlace en cuestion)`.
2. Enlaces como referencia: estos son una manera ordenada para generar enlaces, lo que tenemos que hacer es simple, en una porcion alejada del texto (se recomienda al principio) tenemos que poner entre corchetes `[]`  el nombre de referencia que queramos utilizar para el enlace y dos puntos `: ` el enlace en cuestión (de esta manera cada vez que queramos utilizar el enlace, solo hace falta poner en el texto `[texto a utilizar][nombre de referencia]`).  Ejemplo:`[nombre de referencia]: enlace en cuestión`.
3. Links automaticos: otra manera de generar enlaces es de manera automatica, estos los necesitaremos si queremos enlazar directamente la dirección url completa; la manera que los creamos es poner el link entre los aperadores `<>`. Ejemplo: `<direccion_url.com>`.

### Código
Otra manera de escribir codigo pero en linea esta vez, es encerrar nuestro codigo entre comillas sencillas " ` ".

### Imágenes
Para insertar una imagen es como generar/poner un enlace, solo que debemos agregar un signo de exclamacion `!` al principio del enlace (podemos insertar una imagen realizando un enlace "en linea" o "como referencia"); ademas podemos agregar un texto alternativo para los casos en que la imagen no pueda ser cargada. Otra cosa mas que es opcional es poner un titulo alternativo a la imagen. `![Texto alternativo](/ruta/a/la/imagen.jpg "Titulo alternativo")`.

---

## Multimarkdown
### Abreviaciones
La manera de crear abreviaciones es de la misma manera que enlaces de referencia, solo que esta vez iria precedido de un asterisco. Ejemplo: `*[referencia]: explicacion de la referencia`.

### Definiciones
Si necesitamos hacer una lista de definiciones pero no queremos que tenga identificativos de listas, lo que podemos hacer es antes de cada definición colocar el operador de 2 puntos `:` seguido de 2 espacios y la definicion que queremos colocar. Ejemplo: `:  elemento de la definicon de un objeto`.

### Notas al pie de página
Para crear notas al pie de página debemos definirlas como los enlaces de referencia, solo que para hacerlo seria `[^nombreNota]: texto de la nota al pie de página`. Para usarla solo seria necesario poner tal cual '[^nombreNota]' 

### Tablas
La construcción de tablas con markdown requiere un par de pasos:
1. Especificar los elementos de la cabecera de cada columna
:  Esto se hace encerrando cada elemento entre barras verticales `|`. Ejemplo: `| Encabezado 1 | Encabezado 2 | Encabezado 3 |`.
2. Crear una linea adicional para indicar que terminaron los encabezados
:  Esto se hace igual que el paso anterior, solo que en vez del nombre iran dos guiones. Ejemplo: `| -- | -- | -- |`.
3. Añadir el contenido a la tabla
:  La creacion del contenido es igual que el 1er paso, ya que markdown identifica automaticamente que es contenido por haber realizado el paso 2. Ejemplo: `| Contenido 1-1 | Contenido 1-2 | Contenido 1-3 |`.
En resumen la construcción de una tabla quedaria de la siguiente manera:
~~~
| Encabezado 1 | Encabezado 2 | Encabezado 3 |
| -- | -- | -- |
| Elemento 1-1 | Elemento 1-2 | Elemento 1-3 |
| Elemento 2-1 | Elemento 2-2 | Elemento 2-3 |
| Elemento 3-1 | Elemento 3-2 | Elemento 3-3 |
~~~
