# input radio
Veremos los `input` que nos permiten seleccionar elementos dentro de una lista de opciones.

* radio -> Permite seleccionar una única opción de una lista de opciones relacionadas.

* checkbox -> Permite seleccionar varias opciones de una lista de opciones relacionadas.

* select -> Crea una lista de opciones donde podemos seleccionar una o varias opciones.

Los `select` no son un `input`, son una etiqueta aparte pero también nos permiten seleccionar elementos.

Cada opción irá dentro de una etiqueta `<option></option>`.

## radio

Permite seleccionar una única opción de una lista de opciones relacionadas.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio">
    </label>
    <label for="">Femenino
      <input type="radio">
    </label>
    <label for="">Otro
      <input type="radio">
    </label>
  </form>
</body>
</html>
~~~

<body>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio">
    </label>
    <label for="">Femenino
      <input type="radio">
    </label>
    <label for="">Otro
      <input type="radio">
    </label>
  </form>
</body>
</html>

### **name**
Como podemos observar con `radio` podemos seleccionar opciones relacionadas, pero de este modo todas las opciones pueden ser seleccionadas, entonces debemos usar el atributo `name=""` y que es obligatorio, y el `name` tiene que ser el mismo para todos los casos que están relacionados.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio" name="gender">
    </label>
    <label for="">Femenino
      <input type="radio" name="gender">
    </label>
    <label for="">Otro
      <input type="radio" name="gender">
    </label>
  </form>
</body>
~~~

<body>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio" name="gender">
    </label>
    <label for="">Femenino
      <input type="radio" name="gender">
    </label>
    <label for="">Otro
      <input type="radio" name="gender">
    </label>
  </form>
</body>

Y con esto le estamos informando al navegador que los 3 `input` pertenecen a la misma categoría y que por lo tanto solo podremos seleccionar uno de los 3.

### **checked**
Ahora si tenemos un `input` del tipo `radio` y queremos que una de las opciones este seleccionada por defecto tenemos el atributo `checked` que es un atributo *booleano* y con eso ya sabemos que no necesita ni un *igual* ni un *valor*.
 
~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio" name="gender">
    </label>
    <label for="">Femenino
      <input type="radio" name="gender">
    </label>
    <label for="">Otro
      <input type="radio" name="gender" checked>
    </label>
  </form>
</body>
~~~

<body>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio" name="gender">
    </label>
    <label for="">Femenino
      <input type="radio" name="gender">
    </label>
    <label for="">Otro
      <input type="radio" name="gender" checked>
    </label>
  </form>
</body>

### **value**
Tenemos otro atributo que es obligatorio que se llama `value=""` que nos sirve para decirle al formulario cuando lo enviemos que valor es el que contiene el elemnto y no necesariamente debe corresponder el valor con el `label` pero es recomendable que sea identificaivo.

~~~html
<body>
  <form action="">
    <h2>Género</h2>
    <label for="">Masculino
      <input type="radio" name="gender" value="masculino">
    </label>
    <label for="">Femenino
      <input type="radio" name="gender" value="femenino">
    </label>
    <label for="">Otro
      <input type="radio" name="gender" value="desconocido" checked>
    </label>
  </form>
</body>
~~~

Esto cuando se envie al servidor lo que va a recibir es `name="gender"` y los `value=""` para saber a que categoría pertenece y cual es el valor que a elegido el usuario.
