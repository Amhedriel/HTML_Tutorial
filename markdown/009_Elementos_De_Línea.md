# Elementos de Línea I

Hablaremos de algunos elementos de línea en esta sección:

## \<em>
Etiqueta que se utiliza para representar énfasiscon esto aparecerán las palabras en cursiva pero esto no significa que con la etiqueta `<em></em>` pongamos el texto en cursiva, para estilos se utiliza CSS.

Lo que hacemos con `<em></em>` es indicarle al navegador que lo que está encerrado en esta etiqueta es más importante que el resto del texto

El elemento ``<em>`` puede ser anidado, con cada nivel de anidamiento indicando un mayor grado de énfasis.

~~~html
    <p><em>El dinero</em> es importánte pero la salud es lo más importante</p>
~~~

---
## \<strong>

El elemento strong es el apropiado para marcar con especial énfasis las partes más importantes de un texto.

~~~html
    <p><em>El dinero</em> es importánte pero <strong>la salud</strong> es lo más importante</p>
~~~

Como podremos observar en la página web con `<strong></strong>` el contenido se podrá ver cómo negrita sin embargo esto no es para darle negrita al texto, sirve para que el navegador entienda que de toda la frase lo que esta encerrado en `<strong></strong>` es lo más importante de la frase, después vendría lo que esta entre la etiqueta `<em></em>` y por último lo que no está encerrado.

## \<small>
El elemento HTML \<small> hace el tamaño del texto una talla más pequeña (por ejemplo, de largo a mediano, o de pequeño a extra pequeño) que el tamaño mínimo de fuente del navegador. En HTML5, este elemento es reutilizado para representar comentarios laterales y letra pequeña, incluyendo derechos de autor y texto legal, independientemente de su estilo de presentación.

Menos énfasis que el texto normal.

~~~html
  <p><em>El dinero</em> es importánte pero <strong>la salud</strong> es lo más importante. <small>Saludos!</small></p>
~~~

Con esto decimos que tiene mucha menos relevancia para que el texto que el resto del texto.

---
## \<br>

El elemento HTML line break \<br> produce un salto de línea en el texto (retorno de carro). Es útil para escribir un poema o una dirección, donde la división de las líneas es significante.

Si nosotros tenemos un texto que se rompe en función del espacio que tiene disponible, sin embargo, es posible que se necesite que el texto se rompa en un punto concreto y para eso tenemos la etiqueta `<br>`

~~~html
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> 

Qobcaecati alias explicabo tenetur corrupti ipsam a necessitatibus sapiente incidunt? Quos voluptates porro maiores, <br>

nesciunt quisquam alias, ipsum rem vitae sed consequatur architecto perferendis amet aliquid ea sequi cupiditate obcaecati corporis quod? Ducimus sapiente ipsa error?.</p>

~~~

Ahora dá igual que haya espacio disponible, porque el navegador va a forzar un salto de línea en este punto

No utilices \<br> para incrementar el espacio entre líneas de texto; para ello utiliza la propiedad ``margin`` de CSS o el elemento \<p>.

Indica donde empieza la siguiente línea después del salto. Se usaba para establecer una dirección por ejemplo, que los saltos de lineas si són relevantes, un poema o cualquier tipo de texto que el salto de línea si que tenga relevancia y sea importante.

Jamás utilizar `br` para dar separación entre 2 elementos.

**Nota de uso:** Este atributo está obsoleto en HTML5 y no debe utilizarse por los autores. En su lugar utiliza la propiedad `clear` de CSS.

---
## \<wbr>

"Word Breaking Oportunity", esto es un salto de línea si al navegador le hiciera falta hacerlo, es decir, si nosotros tenemos una palabra larga y necesitemos cortarla en caso de que no quepa para eso se usa `<wbr>`, sin embargo una palabra lo suficientemente larga como para que no quepa en el navegador sería muy complicado pensar en una, pero si es una **url**:

Digamos que tenemos una así:

~~~html
    <p>https://github.com/Amhedriel/<wbr>cursos/html/elementos/<wbr>elementos_de_linea?tab=overview&from=2022-09-01&to=2022-09-01</p>
~~~

Donde lo tengamos guardado o estructurado de otra forma, y queramos que se corte en puntos concretos como por ejemplo después de algubas barras, tendríamos que usar esta etiqueta.

---
## \<time>

Esta etiqueta se utiliza para representar un contenido de **fecha** y **hora**, en que casos puede ser relevante tener fecha y hora, como por ejemplo en un Blog o un Post en el que sea publicado a cierto día y cierta hora y sea relevante que sea ese día y esa hora.

El elemento HTML \<time> representa un periodo específico en el tiempo. Puede incluir el atributo ``datetime`` para convertir las fechas en un formato interno legible por un ordenador, permitiendo mejores resultados en los motores de búsqueda o características personalizadas como recordatorios.

Puede representar uno de los contenidos siguientes:

* Una hora en formato de 24 horas
* Una fecha precisa en el Calendario Gregoriano (con hora y zona horaria opcionales)
* Un periodo de tiempo válido

Lo muestra como si lo tuviéramos dentro de cualquier otra etiqueta pero el navegador está entendiendo que está representando una fecha y por lo tanto le dará la importancia semántica que debería tener fecha/hora.

El orden de fecha/hora no es necesario, es válido hora/fecha o si sólo tuvieramos hora.

~~~html
<time>01/09/2022 10:35</time>
~~~

---
## \<i> \<b> \<u>

Por último tenemos estas 3 etiquetas que se utilizan para dar estilo, sin embargo no se utilizan porque para eso está CSS.

~~~html
    <p>
      <i>Italic</i>
      <b>Bold</b>
      <u>Underline</u>
    </p>
~~~

Sin embargo el único que sería utilizado para tener iconos es la etiqueta `<i></i>`.

---

## \<sup>

Es la etiqueta de super índice generlmente utilizada en matemátias o ciencias.

~~~html
<p>4 elevado al cuadrado se representa así 4 <sup>2</sup></p>
~~~

## \<sub>

Cuando estamos escribiendo algo referido con la química los subíndices si son importantes.

