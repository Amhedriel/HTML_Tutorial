# Button vs type button

## input type:

Ahora veremos algunos tipos de input que existen:
* button -> Se comporta igual que un botón \<button><button>.
* color -> Se utiliza para especificar un color.
* date -> Se utilizapara introducir una fecha.
* datetime -> Obsoleto.
* datetime-local -> Fecha y hora, no funciona en firefox.
* email -> Se utiliza para introducir un email.
* hidden -> Campo oculto, puede contener valor pero no se mostrará.
* month -> Se utiliza para introducir un mes.
* number -> Se utiliza para valores numéricos.
* password -> Se utiliza para contraseñas
* range -> Se utiliza para establecer un rango.
* reset -> Se utiliza para resetear el formulario.
* search -> Se utiliza para las barras de búsqueda.
* submit -> Se utiliza para enviar el formulario.
* tel -> Se utiliza para introducir números telefónicos.
* text -> Valor por defecto.
* time -> Se utiliza para introducir una hora.
* url -> Se utiliza para introducir URLs.
* week -> Se utiliza para introducir el número de semana del año.

Estos `input` no són todos los que existen pero son los que generalmente más se utilizan.

## button

Con este `input`, veremos que aparece un botón pero sin texto.

~~~html
<body>
  <form>
    <input type="button">
  </form>
</body>
~~~

<input type="button">

Esto es una diferencia cuando agregábamos la etiqueta `button` con el texto de enviar por ejemplo:

~~~html
<body>
  <form>
    <input type="button">
    <button>Enviar</button>
  </form>
</body>
~~~
Aquí si aparece el texto "Enviar", pero en un `input` del tipo `button` el valor que queremos que se escriba en el botón se tiene que establecer con el atributo `value=""`, ahi podremos agregar el texto que mos interesa mostrar en el botón.

~~~html
<body>
  <form>
    <input>
    <input type="button" value="Enviar">
    <button>Enviar</button>
  </form>
</body>
~~~
<body>
  <form>
    <input>
    <input type="button" value="Enviar">
    <button>Enviar</button>
  </form>
</body>

A efectos prácticos se diría que visualemente son iguales, pero hay una gran diferencia entre un `input` del tipo `button` y una etiqueta `<button></button>`, un `<input type="button">` NO SIRVE para enviar un formulario, sin embargo el `<button>Enviar</button>` SI ENVÍA el formulario.

***NOTA*** Es muy importante que si colocamos un `<input type="button">` es para poner un botón en el formulario y que haga algún tipo de operación a travéz de JS pero que no sirve para enviar ningún formulario.

Ahora bien, si queremos enviar el formulario con un `<input type="">` tendríamos que usar un tipo `submit` que claramente dice que se utiliza para enviar un formulario.

~~~html
<body>
  <form>
    <input type="submit" value="Enviar input">
  </form>
</body>
~~~

<body>
  <form>
    <input>
    <input type="submit" value="Enviar input">
  </form>
</body>

Y si llenamos el cvampo de `input` y enviamos el formulario con enviar entonces si se enviaría.