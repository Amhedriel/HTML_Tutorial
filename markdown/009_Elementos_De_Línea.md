# Elementos de Línea I

Hablaremos de algunos elemntos de línea en esta sección:

## \<em>
Etiqueta que se utiliza para representar énfasiscon esto aparecerán las palabras en cursiva pero esto no significa que con la etiqueta `<em></em>` pongamos el texto en cursiva, para estilos se utiliza CSS.

Lo que hacemos con `<em></em>` es indicarle al navegador que lo que está encerrado en esta etiqueta es más importante que el resto del texto

El elemento ``<em>`` puede ser anidado, con cada nivel de anidamiento indicando un mayor grado de énfasis.

~~~html
    <p><em>El dinero</em> es importánte pero la salud es lo más importante</p>
~~~


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

## \<br>

El elemento HTML line break \<br> produce un salto de línea en el texto (retorno de carro). Es útil para escribir un poema o una dirección, donde la división de las líneas es significante.

Si nosotros tenemos un texto que se rompe en función del espacio que tiene disponible, sin embargo, es posible que se necesite que el texto se rompa en un punto concreto y para eso tenemos la etiqueta `<br>`

~~~html
<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br> 

Qobcaecati alias explicabo tenetur corrupti ipsam a necessitatibus sapiente incidunt? Quos voluptates porro maiores, <br>

nesciunt quisquam alias, ipsum rem vitae sed consequatur architecto perferendis amet aliquid ea sequi cupiditate obcaecati corporis quod? Ducimus sapiente ipsa error?.</p>

~~~

Ahora dá igual que haya espacio disponible, porque el navegador va a forzar un salto de línea en este punto

No utilices \<br> para incrementar el espacio entre líneas de texto; para ello utiliza la propiedad margin de CSS o el elemento \<p>.

Indica donde empieza la siguiente línea después del salto.

**Nota de uso:** Este atributo está obsoleto en HTML5 y no debe utilizarse por los autores. En su lugar utiliza la propiedad clear de CSS.

## \<wbr>


## \<time>


## hora/fecha


## \<i> \<b> \<u>