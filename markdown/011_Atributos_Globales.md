# Atributos Globales

Revisaremos algunos de los atributos más comunes que están disponibles para la mayoría de **etiquetas** en HTML.

---

* **class** -> Este atributo se usa en la mayoría de etiquetas HTML para dar estilos a través de CSS.

Si nosotros a este `p` le ponemos una ``clase`` y le decimos por ejemplo:
~~~html
 <p class="parrafo-1">Clases</p>
~~~

A efectos visuales no cambia nada, pero podemos identificar a este párrafo a traves de CSS para darle algún tipo de estilo.

~~~CSS
  <style>
    .parrafo-1 {
        color:red;
    }
  </style>
~~~

Sin embargo de momento no veremos CSS asi que terminamos con class por el momento.

---

* **id** -> Es un identificador único que se utiliza para seleccionar el elemento desde JS y para hacer navegación a través de anclas.

Para la parte de JavaScript:
Una de las formas de incrustar JavaScript dentro HTML.

~~~html
<p id="parrafo">Identificador a través de un ID</p>
~~~

Guardaremos el párrafo

~~~JavaScript
  <script>
    const p = document.getElementById('parrafo')

    console.log(p.textContent)
  </script>
~~~
Básicamente lo que estamos haciendo es esta `p` estamos guardando la referencia al elemento `parrafo` entonces dentro de eso, al tener acceso a esta etiqueta podemos hacer cosas, como por ejemplo haremos un `console.log` para mostrar información.

De momento no se ondará en el `id` debido a lo avanzado del tema relacionado a JavaScrip, pero lo más importante por ahora es que un identificador no se puede repetir, debe ser único.

---

* **title** -> Es un atributo que ayuda a la accesibilidad mostrando una descripción del elemento al que pertenece.

Sirve para mostrar informaciónde lo que estamos representando.

~~~html
<p title="Este es un ejemplo del atributo title">Título con tooltip</p>
~~~
Con este atributo lo que hacemos es mostrar un mensaje emergente en el texto del navegador que se denomina **tooltip**.

![title](/media/Atributos_globales.png "Ejemplo de atributos globales, ahora mostrando mensaje emergente de title")

---

* **data-*** -> Es un atributo que nos permite guardar algún valor en la etiqueta HTML.

Lo escribimos como `data-*` porque es un atributo que nos permite guardar algún valor en la etiqueta HTML. Esto al nivel de HTML no se encontrará nunguna utilidad, pero será muy importante más adelante en la parte de JavaScript, este atributo salvará al solucionar problemas.

`data-` y lo que pongamos después del guión es lo que nosotros queramos para identificar

~~~html
<p id="parrafo-2" data-ejemplo="Datos de ejemplo">Datos pasados en la etiqueta</p>
~~~
~~~JS
<script>
    const parrafo2= document.getElementById('parrafo-2')
    console.log(parrafo2.dataset.ejemplo)
</script>
~~~
Al tener este atributo `data-ejemplo` le damos un valor `="Datos de ejemplo"` y como ya tenemos el atributo guardado podemos decirle `console.log(parrafo2.dataset.` y el nombre que le hayamos puesto nosostros`ejemplo)`

y en consola veremos el resultado gracias a `console.log`.

![Consola](/media/Consola1.png "Resultado de la consola")
