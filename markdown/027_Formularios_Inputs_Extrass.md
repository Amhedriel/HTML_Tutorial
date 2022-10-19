# inputs extras

Ahora veremos algunos tipos de input que existen:

* color -> Se utiliza para especificar un color.
* number -> Se utiliza para valores numéricos.
* range -> Se utiliza para establecer un rango.
* reset -> Se utiliza para resetear el formulario.
* text -> Valor por defecto.
* hidden -> Campo oculto, puede contener valor pero no se mostrará.

Estos últimos `input` no pertenecen a ninguna categoría en concreto, asi que son miscelaneos.

## color
Este `input` lo que nos permite es mostrar una plantilla para elegir colores, se puede hacer una página en la que queramos que el usuario elija un color, donde el ususario tenga cierto poder del control del color.

~~~html
<body>
  <form action="">
    <input type="color">
  </form>
</body>
~~~
<body>
  <form action="">
    <input type="color">
  </form>
</body>

## number
El `input` de tipo `number` es para valores numéricos que no sean fechas, que viene acompañado de *widgets* de arriba y abajo para cmabiar valores, la forma depende del navegador, pero con CSS o JS se puede cambiar visualmente.

~~~html
<body>
  <form action="">
    <input type="color">
    <input type="number">
  </form>
</body>
~~~
<body>
  <form action="">
    <input type="number">
  </form>
</body>

## range

Esto crea una barra para poder seleccionar un rango, además los `input` de tipo `range` aceptan el atributo `step=""` que determina de cuanto en cuanto se mueve la barra, si cilicamos un valor de 10 por ejemplo, hará que la barra se mueva de 10% en 10% de un lado a otro; también tiene los atributos `min="" max=""`

~~~html
<body>
  <form action="">
    <input type="range" step="5" min="0" max="20">
  </form>
</body>
~~~
<body>
  <form action="">
    <input type="range" step="5" min="0" max="20">
  </form>
</body>

Con este ejemplo podemos ver que el `input type="range"` crea una barra de rango que con `step="5"` le estamos indicando que corra 5 espacios por tick en una barra con un `min="0"`(mínimo de 0, o sea que no cambie) recorra 5 espacios por tick hasta llegar al número máximo `max="20"` que sería 20, siendo 20 el máximo valor posible para alcanzar lo que hace que dicha barra solo pueda moverse 4 espacios por múltiplo de 5 en total.

## reset

Los `input` del tipo `reset` se utiliza sobre todo al lado del botón `submit` y sirve para resetear el formulario, si tenemos algo escrito y pulsamos el botón, todos los datos del formulario se quedarán con el comportamiento por defecto.

~~~html
<body>
  <form action="">
    <input type="reset">
  </form>
</body>
~~~

<body>
  <form action="">
    <input type="reset">
  </form>
</body>

## text hidden

El ``input`` que se denomina del tipo texto, es el valor por defecto, que equivale a no poner nada, pero es importante saber que es `type="text"` porque si por defevto tenemos un `input="hidden"` que en funcion de lo que haya seleccionado el usuario se muestre o no con JS podemos cambiar este input en concreto e indicar que si seleccionaste la opción "A" que este input cambie de `hidden` a `text` entonces este campo se mostraría.

~~~html
<body>
  <form action="">
    <input type="text">
    <input type="hidden">
  </form>
</body>
~~~

<body>
  <form action="">
    <input type="text">
    <input type="hidden">
  </form>
</body>

[Siguiente **&#129042;**](/markdown/028_Formularios_Inputs_Radio.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")