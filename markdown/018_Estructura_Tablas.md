# Etiquetas que podemos añadir a una tabla

## Como poner un título a la tabla

Los títulos de las tablas se establecen con la etiqueta `caption` que es una etiqueta opcional ya que no todas las tablas necesitan un título, esta etiqueta se debe colocar justo después de la etiqueta `table`.


~~~html
<h1>Tablas</h1>
  
  <table>
    <caption>HORARIO DE CLASES </caption>
    <tr>
      <td>8:30 - 9:30</td>
      <td>Matemáticas</td>
      <td>Matemáticas</td>
      <td>Sociales</td>
      <td>Matemáticas</td>
      <td>Matemáticas</td>
    </tr>
~~~

## Cabeceras de las tablas

Estas se establecen con letiqueta `thead` y dentro tendremos una etiqueta `tr` para establecer la fila de la cabecera, pero en caso de las **celdas** en lugar de utilizar `td` para esas **celdas** vamos a utilizar un `th` que sería un table head.

~~~html
 <table>
    <caption>HORARIO DE CLASES </caption>
    <thead>
      <tr>
        <th></th>
        <th>L</th>
        <th>M</th>
        <th>X</th>
        <th>J</th>
        <th>V</th>
      </tr>
    </thead>
    <tr>
      <td>8:30 - 9:30</td>
      <td>Matemáticas</td>
      <td>Matemáticas</td>
      <td>Sociales</td>
      <td>Matemáticas</td>
      <td>Matemáticas</td>
    </tr>
~~~

Si necesitamos tener una celda vacía entonces colocaremos el `th` sin contenido.

## Cuerpo de las tablas

El hecho de tener un `th` quiere decir que estamos estableciendo grupos dentro de la **tabla**, entonces la semántica correcta para todo el contenido de la **tabla** sería un `tbody`.

~~~html
<tbody>
      <tr>
        <td>8:30 - 9:30</td>
        <td>Matemáticas</td>
        <td>Matemáticas</td>
        <td>Sociales</td>
        <td>Matemáticas</td>
        <td>Matemáticas</td>
      </tr>
    <tr>
      <td>9:30 - 10:25</td>
      <td>Lenguaje</td>
      <td>Lenguaje</td>
      <td>Matemáticas</td>
      <td>Ciencias</td>
      <td>Lenguaje</td>
    </tr>
    ...
</tbody>
~~~

Esta etiqueta es opcional siempre y cuando no estemos utilizando un `thead` en cuanto establezcamos una cabecera el resto de bloques de la tabla tienen que estar dentro de un `tbody`.

## Foot

Es completamente opcional y se utiliza para poner un pie de tabla.

~~~html
</tbody>
    <tfoot>
      <tr>
        <td>Total de asignaturas</td>
        <td>12</td>
      </tr>
    </tfoot>
  </table>
~~~

Con esto tendríamos la estructura completa de una **tabla**, `<thead></thead>` `<tbody></tbody>` `<tfoot></tfoot>` y dentro tenemos los `<tr></tr>` para las filas y los `<td></td>` para las celdas.


[Siguiente **&#129042;**](/markdown/019_Atributos_De_Tablas.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")