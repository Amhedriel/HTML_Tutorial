# Introducción a las tablas

Las tablas en HTML sirven para representar el contenido tabulado que sería el contenido que queremos mostrar dentro de una tabla, cuya finalidad es que el contenido en concreto este estructurado y que no haya una forma mejor que estructurarlo en una tabla.

Una referencia de un buen uso de una tabla sería para estructurar el contenido de un horario de clases.

## Estrucutra básica de una tabla

Vamos a construir una estructura básica de una tabla, para ello utilizaremos las tres etiquetas principales que tiene una tabla.

* **table** -> Etiqueta que encierra una tabla.
* **tr** -> table row, etiqueta que construye una fila.
* **td** -> table data, etiqueta que construye una celda.

**NOTA** El número de **celdas** dentro de un `tr` establecerá el número de **columnas** de la tabla.

### **table**

Cuando empieza un table empieza una tabla y al cerrarlo termina

### **table row \<tr>\</tr>**

Es la etiqueta que construye un **fila** de cada tabla.

### **table data \<td>\</td>**

Es la etiqueta que construye una **celda**.

Para crear una tabla, primero debemos colocar la etiqueta `<table></table>` para establecer nuestra tabla y crearemos nuestro primer `<tr></tr>` esto sería un **table row**, aqui estableremos el número de **celdas** que va a tener dentro nuestra **fila**, entonces ponemos un `<td></td>` y ponemos el primer contenido de la celda.

~~~html
<body>

  <h1>Tablas</h1>
  
  <table>
    <tr>
      <td>8:30 - 9:30</td>
    </tr>
  </table>
</body>
~~~

Con esto podríamos ver una tabla con una **fila**,**columna** que forma una **celda**.

~~~html
<body>

  <h1>Tablas</h1>
  
  <table>
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
    <tr>
      <td>10:25 - 11:20</td>
      <td>Educación Física</td>
      <td>Ciencias</td>
      <td>Lenguaje</td>
      <td>Lenguaje</td>
      <td>Educación Física</td>
    </tr>
    <tr>
      <td>11:20 - 11:45</td>
      <td>Recreo</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>11:45 - 12:40</td>
      <td>Inglés</td>
      <td>Sociales</td>
      <td>Inglés</td>
      <td>Tutoría</td>
      <td>Inglés</td>
    </tr>
    <tr>
      <td>12:40 - 13:35</td>
      <td>Música</td>
      <td>Educación Física</td>
      <td>Plástica</td>
      <td>Religión</td>
      <td>Música</td>
    </tr>
    <tr>
      <td>13:35 - 14:30</td>
      <td>Tecnología</td>
      <td>Francés</td>
      <td>Tecnología</td>
      <td>Francés</td>
      <td>Tecnología</td>
    </tr>
  </table>
</body>
~~~

Este sería un ejemplo de maquetación de tablas.

![Tabla1](/media/Tablas1.png "Tabla_básica")


|8:30 - 9:30      |Matemáticas      |Matemáticas      |Sociales         |Matemáticas      |Matemáticas      |
| ----------------| ----------------| ----------------| ----------------| ----------------| ----------------|
|9:30 - 10:25     |Lenguaje         |Lenguaje         |Matemáticas      |Ciencias         |Lenguaje         |
|                 |                 |                 |                 |                 |                 |
|10:25 - 11:20    |Educación Física |Ciencias         |Lenguaje         |Lenguaje         |Educación Física |
|                 |                 |                 |                 |                 |                 |
|11:20 - 11:45    |Recreo           |                 |                 |                 |                 |
|                 |                 |                 |                 |                 |                 |
|11:45 - 12:40    |Inglés           |Sociales         |Inglés           |Tutoría          |Inglés           |
|                 |                 |                 |                 |                 |                 |
|12:40 - 13:35    |Música           |Educación Física |Plástica         |Religión         |Música           |
|                 |                 |                 |                 |                 |                 |
|131:35 - 14:30   |Tecnología       |Francés          |Tecnología       |Francés          |Tecnología       |
|                 |                 |                 |                 |                 |                 |


