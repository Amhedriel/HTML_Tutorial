# Atributos Globales

Revisaremos algunos de los atributos más comunes que están disponibles para la mayoría de **etiquetas** en HTML.

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


* **title** -> Es un atributo que ayuda a la accesibilidad mostrando una descripción del elemento al que pertenece.



* **data** -> Es un atributo que nos permite guardar algún valor en la etiqueta HTML.