# Etiquetas de bloque II

## address
Se utiliza para aportar información de contacto para el `article` más cercano o para todo el `body`.

Si por ejemplo, tenemos un artículo que menciona un usuario o una noticia y esa noticia a ocurrido en cierta dirección en concreto, se debería encerrar en una etiqueta `<address></address>` porque estamos guardando o imprimiendo información que es relevante para esa noticia en concreto o para ese usuario.

Si lo usamos en el `footer` esto correspondería a la información de contacto de la página, persona, empresa de la que pertenece dicha página.

~~~html
<body>

  <address>
    Tony Stark <br>
    Malibú 10880 <br>
    90265 <br>
    California
  </address>
  
</body>
~~~
Aquí tenemos una dirección hecha de forma semánticamente correcta y además lo estamos metiendo dentro de una etiqueta `address` que se utiliza para colocar una dirección.

## blockquote
Se utiliza para marcar las citas a otros autores o documentos. Se puede incluir el atributo `cite` para poner un enlace al documento original o fuente; esto no lo convierte en un enlace o ancla, es simplemente para que el navegador sepa de donde viene esa información.

Cuando nosotros hacemos referencia a un texto de otra página o una frase célebre de otro autor normalmente Esto debe ir en la etiqueta `blockquote`, esta es la etiqueta de bloque para citas.

~~~html
<body>
  <blockquote cite="https://www.entrepreneur.com/article/312598">
    <p>
      Hay cosas que nunca le pregunté a mi padre. Hay preguntas que me hubiera gustado hacerle: cómo se sentía por lo que hacía su empresa, si estaba conflictuado, si tenía dudas (...). Vi a jóvenes estadounidenses ser asesinados por las armas que creaba para defenderlos y protegerlos. Me di cuenta que era parte de un sistema que no rinde cuentas.
    </p>
  </blockquote>
</body>
~~~
Esta es la forma correcta de representar una cita.

## pre

Se utiliza para tener el código preformateado que necesita ser representado igual que se escribió.

Se usa muchísimo cuando estamos escribiendo letras de canciones, poemas, o código que queremos representar visualmente.

~~~html
  <pre>
    Qué buena suerte,
    qué buena suerte y que viví,
    volver a verles
    amigos míos,

        Que felicidad,
        creí que nunca más
        os volvería a verlos..
  </pre>
  
~~~
Normalmente la etiqueta `pre` suele venir acompañada de la etiqueta `code` que es una etiquta de línea.

## div
Es una división del documento, que semánticamente no significa nada y es un cotenedor genérico, en el 99 % de los casos son para dar estilos en CSS o para algo denominado "delegación de eventos en JavaScript"

Por ejemplo si tenemos una tarjeta de usuario.

```html
  <div>
    <h2>Nombre</h2>
    <p>email</p>
    <p>descripción</p>
  </div>
```
Entonces a través de este `div` nosotros podríamos dar estilo a cada uno de los diferentes elementos o generar clases.

Lo importante es: Que el contenido que este dentro de un div está relacionado, es decir si tuvieramos otro usuario lo correcto sería tenerlo en un ``div`` nuevo.

`div` no significa nada semántixamente pero sirve para dividir contenido.


## hr
*horizontal rule*, se utiliza para decirle al navegador que vamos a cambiar de tema.

Si terminamos un tema y en el siguiente párrafo hablaremos de un tema distinto debemos decirle al navegador que cambiamos de tema mediante la etiqueta `<hr>` visualmente se representa con una línea en el navegador.

**NOTA** `hr` no sirve para dibujar líneas, es solo para cambiar temas.

El elemento `hr` representa un quiebre en la temática del párrafo, como el cambio de una escena en una historia, o la transición hacia otro tema o la referencia a un libro.

~~~html
  </blockquote>
  <hr>
  <pre>
    Qué buena suerte,
    qué buena suerte y que viví,
    volver a verles
    amigos míos,

        Que felicidad,
        creí que nunca más
        os volvería a verlos..
  </pre>
  <hr>
  <div>
    <h2>Nombre</h2>
    <p>email</p>
    <p>descripción</p>
  </div>
~~~

De momento estas son algunas estiquetas a nivel de bloque.

[Siguiente **&#129042;**](/markdown/021_Etiquetas_Importantes_L%C3%ADnea.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")