# Veremos los atributos para las talas

## Agrupar celdas en columnas y filas

Al ver que *recreo* está ocupando una sola celda, pero necesitamos que ocupe 5, y en el caso de *Total de asignaturas* ocupara todas las celdas hasta el **J** *Jueves*, y el *12* lo dejara en el **V** para que quede más estético.

Para hacer que las celdas ocupen más de una fila o más de una columna tenemos 2 atributos:

* **rowspan**: sirve para que una celda ocupe más de una fila, el valor por defecto es 1.

* **colspan**: sirve para que una celda ocupe más de una columna, el valor por defecto es 1.

***NOTA*** El valor por defecto es 1 por eso todo el contenido hasta ahora está ocupando su espacio en su respectiva **celda**.

~~~html
  <tr>
      <td>11:20 - 11:45</td>
      <td colspan="5">Recreo</td>
  </tr>
~~~

Con esto nuestro contenido "Recreo" ya está ocupando las 5 colunmas, pero no es apreciable visiblemente, asi que manipularemos un poco html para tener estilos y hacer apreciable los cambios.

~~~html
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tablas</title>
  <style>
    td {
      background-color: steelblue;
    }
  </style>

</head>
~~~

![Tabla1](/media/Tabla_Coloreada1.png "Tabla coloreada para ver el espacio que ocupa Recreo de una manera más visual")

Con esto ahora podemos arreglar el "Total de asignaturas y 12".

~~~html
    <tfoot>
      <tr>
        <td colspan="5">Total de asignaturas</td>
        <td>12</td>
      </tr>
    </tfoot>
~~~

Con esto colocamos 5 espacios de "Total de asignaturas" y en la sexta celda "12"

Ahora veremos un ejemplo de `rowspan`, digamos que no se dictara "música" por un tiempo pero lo reemplazaremos com "Tecnología".

~~~html
    <tr>
      <td>12:40 - 13:35</td>
      <td rowspan="2">Tecnología</td>
      <td>Educación Física</td>
      <td>Plástica</td>
      <td>Religión</td>
      <td rowspan="2">Tecnología</td>
    </tr>
    <tr>
      <td>13:35 - 14:30</td>
      <td>Francés</td>
      <td>Tecnología</td>
      <td>Francés</td>
    </tr>
    </tbody>
~~~

Comprendamos que al hacer este tipo de manipulaciones en html con las tablas llegan momento en que las rompemos, debemos tener en cuenta que cada ``<td>`` ocupa un espacio aún estando vacio y suele causar problemas de espacio, en este caso ampliamos "Tecnoligía" reemplazando "Música" por ese motivo borramos este último de la tabla para evitar errores.

---

## Seleccionar columnas

Hasta ahora vimos que dentro de un `tr` podemos seleccionar toda la primera fila, pero de momento no sabemos cómo seleccionar una sola columna, eso veremos ahora.

Cuando necesitamos seleccionar una columna, tenemos la etiqueta `<colgroup></colgroup>` que nos permite seleccionar una columna en concreto. Dentro pondremos tantas etiquetas `<col>` como columnas tengamos, cada etiqueta `col` equivaldrá a una columna siguiendo el mismo orden que tienen en la tabla.

~~~html
  <style>
    col {
      background-color: tomato;
    }
  </style>
...
<table>
    <caption>HORARIO DE CLASES </caption>
    <colgroup>
      <col>
    </colgroup>
    <thead>
      <tr>
        <th></th>
        <th>L</th>
        <th>M</th>
    ...
</table>
~~~

Visualmente no cambia nada pero lo que estamos haciendo es seleccionar la primera columna como solo hay un `col`.

![Tabla_ejemplo_col](/media/Tabla_Coloreada2.png "Vemos la primera columna coloreada pòr utilizar col")

~~~html
<table>
    <caption>HORARIO DE CLASES </caption>
    <colgroup>
      <col>
      <col>
    </colgroup>
    <thead>
      <tr>
        <th></th>
        <th>L</th>
        <th>M</th>
    ...
</table>
~~~

Ahora al tener 2 `col` estamos seleccionando la primera y la segunda columna.

~~~html
<table>
    <caption>HORARIO DE CLASES </caption>
    <colgroup>
      <col>
      <col>
      <col>
      <col>
      <col>
      <col>
    </colgroup>
    <thead>
      <tr>
        <th></th>
        <th>L</th>
        <th>M</th>
    ...
</table>
~~~

Aqui estamos seleccionando las 6 columnas que tenemos en el ejemplo.

Si necesitamos que una etiqueta `col` agrupe más de una columna, tenemos el atributo `span`, que funciona exactamente igual que `rowspan` y `colspan`.

Para ayuda visual colorearemos un poco el ejemplo

~~~html

  <style>
    col:nth-child(2){
      background-color: aqua;
    }

  </style>
  ...
<table>
    <caption>HORARIO DE CLASES </caption>
    <colgroup>
      <col>
      <col>
      <col>
      <col>
      <col>
      <col>
    </colgroup>
    <thead>
      <tr>
        <th></th>
        <th>L</th>
        <th>M</th>
    ...
</table>
~~~

Con este `style` le estamos diciendo que nos seleccione el **segundo** `colspan` que existe.

![Tabla_seleccionada](/media/Tabla_Coloreada3.png "Selección de col 2")

~~~html

<table>
    <caption>HORARIO DE CLASES </caption>
    <colgroup>
      <col span="5">
      <col>
    </colgroup>
    <thead>
      <tr>
        <th></th>
        <th>L</th>
        <th>M</th>
    ...
</table>
~~~

Con este `col span="5"` esta ocupando desde la primera columna hasta la quinta.

La opción `colgroup` es muy buena opción para dar a estilos como dar color a cada uno de las columnas, pero no es la forma correcta de dar estilo, asi que la mejor opción es CSS y no manchar nuestro html.