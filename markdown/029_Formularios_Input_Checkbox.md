# input checkbox

Ahora veremos como funcionan los `input`  tipo `checkbox`, prácticamente es lo mismo que los tipo `radio` con la diferencia que los `checkbox` nos permiten seleccionar varias opciones de una lista de opciones relacionadas.

Al igual que los `input` del tipo `radio` necesitan el `name=""` para saber a que categoria pertenecen y un `value=""`


~~~html
<body>
  <form action="">
    <h2>Lenguajes que conoces</h2>
    <label for="">
      HTML
      <input type="checkbox" name="languages" value="html" checked>
    </label>
    <label for="">
      CSS
      <input type="checkbox" name="languages" value="CSS">
    </label>
    <label for="">
      JavaScript
      <input type="checkbox" name="languages" value="javascript">
    </label>
  </form>
</body>
~~~

Podemos usar el atributo booleano `checked` incluso en las 3 opciones y esto sería válido, a diferencia de un `radio` que no lo sería.

<body>
  <form action="">
    <h2>Lenguajes que conoces</h2>
    <label for="">
      HTML
      <input type="checkbox" name="languages" value="html" checked>
    </label>
    <label for="">
      CSS
      <input type="checkbox" name="languages" value="CSS">
    </label>
    <label for="">
      JavaScript
      <input type="checkbox" name="languages" value="javascript">
    </label>
  </form>
</body>
