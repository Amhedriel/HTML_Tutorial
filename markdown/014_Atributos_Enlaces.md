# Atributos de los enlaces

En este momento hablaremos de los 2 atributos más importantes que tiene la etiqueta `<a></a>`.

1. ***target***: lo que hace es definir cómo se abrirá el recurso solicitado. Por norma general siempre que se usa rutas *absolutas* usaremos el valor ``"_blank"``, pero el valor por defecto es `_self` que sería lo mismo a no poner nada; en el caso de las rutas relatizas a la raíz el atributo `target` no se lo utilizaría practicamente nunca.

  * *_blank* nos permite abrir el contenido de esa página en una nueva pestaña sin tener que salir de la actual, generalmente se la usa para guiar al usuario a un enlace externo a nuestra página, como podría ser un link de referencias o productos.

  ~~~html
<body>
  <h1>HOME</h1>
  <a href="contacto.html">Ir a contacto</a>
  
  <a href="http://google.com" target="_blank">Ir a Google</a>
</body>
  ~~~

2. ***download***: Atributo booleano, sirve para descargar el recurso solicitado.
***IMPORTANTE!*** el recurso que se desea descargar debe estar en el servidor.

  ~~~html
<body>
  <h1>HOME</h1>
  <a href="contacto.html" download>Descargar</a>
</body>
  ~~~

Recordar que el recurso no se abre, simplemente se descarga.

*``download``* indica que el hipervinculo es utilizado para descargar un recurso.

No podemos descargar un HTML de otro punto al igual que las imágenes, debido a que las rutas no corresponden a nuestro servidor ya que son rutas absolutas, para descargar un archivo debe estar en nuestro servidor.

---
## Estructura de HTML con imágenes

En primer lugar debemos crear una carpeta llamada **assets**, en esta carpeta se guardan todos los medios externos, imágenes, videos, música, iconos, etc. y dentro de esta carpeta crearemos una carpeta llamada **images**.


---
## Navegación con Anclas

Haremos navegación internas dentro de nuestro sitio web, para este ejemplo crearemos un Blog.

Tendremos 5 posts con texto de relleno (Lorem) y navegaremos entre ellos.

Utilizaremos un **tag** `<nav></nav>` para crear un menu de navegación, deberemos utilizar `id=""` para los posts que utilizaremos como ejemplo y en el **nav** llenaremos los **p** con enlaces a dichos posts `<p><a href="#post-1">Post 1</a></p>` en este caso referenciando al *post-1*.

~~~html
<body>
  <h1>Blog</h1>

  <nav>
    <p><a href="#post-1">Post 1</a></p>
    <p><a href="#post-2">Post 2</a></p>
    <p><a href="#post-3">Post 3</a></p>
    <p><a href="#post-4">Post 4</a></p>
    <p><a href="#post-5">Post 5</a></p>
  </nav>

  <article id="post-1">
    <h2>Post 1</h2>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptatibus iure ab libero eum blanditiis, beatae delectus sunt nulla quibusdam, illum voluptatum labore autem aliquid amet commodi distinctio maiores! Vero, deleniti doloremque laboriosam similique, accusamus est harum tempora cupiditate perferendis provident nemo natus officia cum odio aspernatur fugiat. Delectus voluptatibus error perspiciatis aut et, dolorem cumque nihil dignissimos labore quaerat enim deleniti. Eveniet maiores nesciunt sint corporis enim beatae fuga! Eum?</p>
  </article>

  <section id="post-2">
    <h2>Post 2</h2>
    <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ab, sint minus doloremque et non necessitatibus laborum praesentium maiores, beatae, voluptatem totam ex culpa aliquid omnis maxime sunt hic autem sequi dicta? Sed, ab modi porro tenetur quo placeat quasi sapiente quas. Dolorem commodi a dolores officia iusto placeat sed tempora hic, iste ratione debitis delectus omnis, quas, molestias est non consectetur nisi enim deleniti. Magnam consectetur aspernatur fugiat saepe delectus, quod, beatae nobis ea sit ducimus blanditiis quia vel excepturi, sunt ipsa quas. Dolores ratione nobis sint earum necessitatibus vitae blanditiis beatae corrupti reiciendis ipsa amet aliquid saepe qui, odio odit expedita? Omnis consequuntur, dolores unde non totam cupiditate placeat molestiae recusandae dolorem nam amet pariatur quam fugiat nesciunt mollitia at quos facilis aliquid? Quod ducimus velit nostrum, possimus cum impedit autem rem excepturi consectetur mollitia temporibus itaque neque nulla quasi sit corporis ab, similique provident harum! Laudantium, eos magnam.</p>
  </section>
<hr>
  <article id="post-3">
    <h2>Post 3</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum necessitatibus dolorum quod sed corrupti ad labore repellat? Illum soluta rem saepe quaerat, dignissimos aliquid, voluptatem harum dolorem iste eius, eum labore deleniti recusandae esse corrupti ea reprehenderit ut dolore. Laborum, cumque nesciunt aut deleniti in tenetur? Rerum cum eligendi distinctio praesentium voluptates? Expedita, perspiciatis corrupti sapiente quidem laboriosam odio ex cumque aperiam recusandae, hic, aut nihil qui. Voluptatibus adipisci hic repudiandae voluptatem quaerat odio totam numquam, sed, atque non cumque velit, ab exercitationem dolorum deleniti modi quae facere. Deserunt, consequuntur ad. Harum quam nostrum, omnis quasi ex molestias ad aut!</p>
  </article>
<hr>
  <article id="post-4">
    <h2>Post 4</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum necessitatibus dolorum quod sed corrupti ad labore repellat? Illum soluta rem saepe quaerat, dignissimos aliquid, voluptatem harum dolorem iste eius, eum labore deleniti recusandae esse corrupti ea reprehenderit ut dolore. Laborum, cumque nesciunt aut deleniti in tenetur? Rerum cum eligendi distinctio praesentium voluptates? Expedita, perspiciatis corrupti sapiente quidem laboriosam odio ex cumque aperiam recusandae, hic, aut nihil qui. Voluptatibus adipisci hic repudiandae voluptatem quaerat odio totam numquam, sed, atque non cumque velit, ab exercitationem dolorum deleniti modi quae facere. Deserunt, consequuntur ad. Harum quam nostrum, omnis quasi ex molestias ad aut!</p>
  </article>
<hr>
  <article id="post-5">
    <h2>Post 5</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum necessitatibus dolorum quod sed corrupti ad labore repellat? Illum soluta rem saepe quaerat, dignissimos aliquid, voluptatem harum dolorem iste eius, eum labore deleniti recusandae esse corrupti ea reprehenderit ut dolore. Laborum, cumque nesciunt aut deleniti in tenetur? Rerum cum eligendi distinctio praesentium voluptates? Expedita, perspiciatis corrupti sapiente quidem laboriosam odio ex cumque aperiam recusandae, hic, aut nihil qui. Voluptatibus adipisci hic repudiandae voluptatem quaerat odio totam numquam, sed, atque non cumque velit, ab exercitationem dolorum deleniti modi quae facere. Deserunt, consequuntur ad. Harum quam nostrum, omnis quasi ex molestias ad aut!</p>
  </article>
<hr>

  <footer> <small>Davikin Amhedriel </small></footer>
</body>
~~~

Aqui vemos el ejemplo completo y nos permmite navegar entre los posts de la misma página sin problemas.

Esto no solo es útil para movernos dentro de la misma página, podríamos desde otra página ir a este punto:

~~~html
<body>
  <h1>HOME</h1>
  <nav>
    <p><a href="/html/Web-demo/paginas/blog.html#post-1">Post 1</a></p>
    <p><a href="/html/Web-demo/paginas/blog.html#post-2">Post 2</a></p>
    <p><a href="/html/Web-demo/paginas/blog.html#post-3">Post 3</a></p>
    <p><a href="/html/Web-demo/paginas/blog.html#post-4">Post 4</a></p>
    <p><a href="/html/Web-demo/paginas/blog.html#post-5">Post 5</a></p>

  </nav>
  <a href="contacto.html">Ir a contacto</a>

  <a href="http://google.com" target="_blank">Ir a Google</a>
</body>
~~~
Con esta adición de **``<nav></nav>``** en nuestro **index.html** nos habilita un menú a los posts de nuestra página de **blog.html**
