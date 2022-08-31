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
3. Elementos de Linea
  - Enfasis
  - Links/enlaces
  - Código
  - Imágenes
5. Elementos varios
  - Links automáticos
  - Omicion de markdown
___
## Elementos de bloque
### Párrafos y saltos de línea
En Markdown para generar un salto de línea hay que dejar simplemente un renglon vacio, lo que pasa es que como Markdown no soporta *dobles lineas*, si nosotros dejamos mas de un renglon vacio, estos se mostraran como uno solo.  
Si dejamos al final de cada renglon dos (2) espacios en blancos con la barra espaciadora, Markdown nos mantendran las lineas tal como pusimos en el codigo (si no dejamos estos espacios en blanco, se nos formateara todas las lineas en una sola).  

### Encabezados
Para disnguir el texto con los 6 tipos de encabezados que posee Markdown, solo hace falta poner la almohadilla/hashtag "#" antes de cada texto. Tambien se puede usar la misma cantidad de almohadillas que ponemos al principio para "cerrar" el encabezado, pero esto es opcional, ya que Markdown las cierra solas.  Otra manera de generar encabezados es utilizando el simbolo igual "=" para encabezados de "tipo 1 (#)" y guiones "-" para el "tipo 2 (##)"; estos irian en la de abajo de nuestro "encabezado", y la cantidad es arbitraria, ya que puede ser desde 1 hasta lo que nosotros queramos.  

### Citas
Estas se generan con el operador _mayor que_ ">" e irian al comienzo de nuestro bloque de texto a citar; en el caso de que una cita se componga de varios parrafos, tendriamos que poner en cada comienzo el simbolo correspondiente.  
Si se llegase a necesitar, se puede anidar citas (tener una dentro de otra), para esto tendriamos que agregar un operador más (la cantidad de operadores > es proporcional a la cantidad de "anidacion" que va a tener una cita).  
Para que en la cita podamos poner una linea en blanco, tendriamos que en esa "linea en blanco" poner la cantidad de operadores que estemos usando en esa jerarquia/anidacion.  

### Listas
Dentro de las listas tenemos:  
> Listas desordenadas  
> > Estas las podemos crear con el operador asterisco "*", guion "-" o suma "+".  
>  
> Listas ordenadas  
> > Estas las podemos crear utilizando un numero seguido de un punto "1.".  

Cualquiera de los dos tipos de listas las podemos anidar, esto se lograria agregando una tabulacion y/o cuatro (4) espacios en blancos adelante del elemento que queramos anidar.  

### Codigos de bloques
Para poder generar un codigo de bloque al cual Markdown no formatearia y queramos que se distinga, lo que tenemos que hace es entre nuestro codigo colocar en la linea de arriba y en la de abajo el tres operadores virguilla "~~~".  

### Reglas horizontales
Estas se utilizan para separar secciones de una manera visual, la creacion de las mismas es utilizando los siguientes operadores:
- asteriscos "*".
- guiones medios "-".
- guiones bajos "_".

Para generar estas reglas tenemos que poner 3 operadores de los que mencionamos previamente.  


---

## Elementos de linea
