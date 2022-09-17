# Formularios

## Asociar input y label
Sirve para escribir el nombre del campo rellenar debe tener el atributo `for` al cual se le indica un `id` que lo hará será emparejar el ``label`` con su ``input`` correspondiente.

Veremos cómo unir un `label` a un `input`, sabemos que existe el atributo `for` que se le pone al `label` y hay que indicar el `id` que tiene el `input`, es decir:

~~~html
<body>
  <form>
    <label for="name">Nombre</label>
    <input id="name">
    <button>Enviar formulario</button>
  </form>
</body>
~~~

Para asociar `input` y `label` en `label` tendremos un `for` con el mismo `name` del `id="name"` del `input`, de esta forma si hacemos click en el input podemos escribir, pero si hago click en el Nombre también se activa para que podamos escribir

![Formulario_asociado](/media/Formulario_basico.png "Formulario asociado entre label e input")

Esta es una forma de asociar un `label` con un `input`, pero aunque hay otra manera es posible que se la vea muy poquito o quizás nunca:

~~~html
<body>
  <form>
    <label>
      Nombre
      <input>    
    </label>
    <button>Enviar formulario</button>
  </form>
</body>
~~~

Con esto se obtiene el mismo resultado que en el anterior código, pero esta forma no es muy común porque al momento de dar estilos por tener el `label` y el `input` en un bloque, da pocas opciones de jugar con los elementos, sin embargo recordemos que es válido.
