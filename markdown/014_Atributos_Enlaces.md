# Atributos de los enlaces

La etiqueta ``<a></a>`` tiene algunos atributos específicos que debe conocer. Aquí hay un resumen rápido de lo que son:

## Atributo ``href``

El atributo base de los hipervínculos ``href`` define la dirección URL de destino, haciendo que se pueda hacer clic en la palabra o frase marcada. Como crea el hipervínculo a otra página web, el enlace HTML ``href`` no funcionaría según lo previsto sin él:

    <a href="https://www.bitdegree.org">This is a link to coding lessons.</a>

## Atributo ``title``

El atributo ``title`` describe información adicional sobre el propósito del vínculo. Si un usuario pasa el ratón sobre el enlace HTML, aparecerá una información sobre herramientas que describe el objetivo, el título o cualquier otra información que especifique:

    <a href="https://www.bitdegree.org/" title="Link to learn">Learn to code</a>

---

## Atributo ``target``

El atributo define dónde se abrirá el vínculo HTML. Aquí están todas las opciones posibles:

1. ***target***: lo que hace es definir cómo se abrirá el recurso solicitado. Por norma general siempre que se usa rutas *absolutas* usaremos el valor ``"_blank"``, pero el valor por defecto es `_self` que sería lo mismo a no poner nada; en el caso de las rutas relativas a la raíz el atributo `target` no se lo utilizaría prácticamente nunca.


|Option||Description|
|---|---|---|
|**`_blank`**||Redirecciona al usuario a una ventana nueva|
|**`_self`** (default feature)||Carga el URL en la misma ventana|
|**`_parent`**||Carga la dirección URL en el marco principal. Solo se usa con marcos.|
|**`_top`**||Carga el documento vinculado en todo el cuerpo de la ventana|
|**`frame name`** (obsoleto)||Se cargó el documento vinculado en un marco con nombre|
||||

~~~html
<a href="https://www.bitdegree.org" target="_blank">Loads in New tab</a>
<a href="https://www.bitdegree.org" target="_self">Loads in Self</a>
<a href="https://www.bitdegree.org" target="_parent">Loads in Parent</a>
<a href="https://www.bitdegree.org" target="_top">Loads in Body</a>
~~~

## *``_blank``* 
Nos permite abrir el contenido de esa página en una nueva pestaña sin tener que salir de la actual, generalmente se la usa para guiar al usuario a un enlace externo a nuestra página, como podría ser un link de referencias o productos.

~~~html
<body>
  <h1>HOME</h1>
  <a href="contacto.html">Ir a contacto</a>
  
  <a href="http://google.com" target="_blank">Ir a Google</a>
</body>
~~~

---

## **``download``** indica que el hipervínculo es utilizado para descargar un recurso.

***download***: Atributo booleano, sirve para descargar el recurso solicitado.

***IMPORTANTE!*** el recurso que se desea descargar debe estar en el servidor.

  ~~~html
<body>
  <h1>HOME</h1>
  <a href="contacto.html" download>Descargar</a>
</body>
  ~~~

No podemos descargar un HTML de otro punto al igual que las imágenes, debido a que las rutas no corresponden a nuestro servidor ya que son rutas absolutas, para descargar un archivo debe estar en nuestro servidor.

Recordar que el recurso no se abre, simplemente se descarga.

## `Bookmarks`

Si tiene una página web con mucho contenido, el uso de marcadores con enlaces HTML permitirá a los usuarios saltar a partes específicas de inmediato, en lugar de desplazarse por la página completa. Por ejemplo, puede usar marcadores alfabéticos y relevantes para el tema para un glosario de términos.

Si desea marcar secciones de su contenido, deberá usar el atributo `id`. Úsalo para marcar la sección de la página en la que pretendes que terminen los usuarios:

    <h2 id="about-corgi">Pembroke Welsh Corgi</h2>

Luego, una vez que esté creando el hipervínculo, simplemente agregue un símbolo hash antes del nombre de identificación. El fragmento de código debería tener un aspecto similar al siguiente:

    <a href="#about-corgi">Jump to read about adorable Pembroke Welsh Corgi!</a>

Si desea ser aún más avanzado, también puede incluir un enlace `id` a un marcador desde una página diferente. Suponiendo que se especifica un valor en la otra página, simplemente incluya su URL de destino antes del símbolo hash. Aquí hay un ejemplo:

    <a href="https://www.bitdegree.org/tutorials/difference-between-html-and-html5/#What_is_HTML5">Jump to read about HTML5</a>

## `Email Tag`

Si desea que los visitantes de su sitio se comuniquen fácilmente con usted para obtener comentarios o consultas, una forma de hacerlo es creando un enlace `mailto`. Esta llamada etiqueta de correo electrónico parece un hipervínculo pero, una vez que se hace clic, utiliza el cliente de correo predeterminado del visitante para crear un borrador de correo electrónico.

>*Note: Adding a mailto link can lead to unnecessary spamming of your email account. Another option for increasing client engagement is adding HTML forms, which you’ll learn a bit later.

Puede crear un enlace de este tipo con el mismo atributo `href`. Sin embargo, en lugar de una URL normal, debe escribir `mailto:`, junto con su dirección de correo electrónico:

    <a href="mailto:name@email.com">Have any questions?</a>

Si desea agregar un asunto predeterminado, puede expandir la línea con el parámetro `subject`:

    <a href="mailto:name@email.com?subject=Feedback">Have any questions?</a>

También puede agregar un mensaje de cuerpo predeterminado a través del parámetro ``body``:

    <a href="mailto:name@email.com?subject=Feedback&body=Feedback and Questions Go Here">Have any questions?</a>

---

## Estructura de HTML con imágenes

En primer lugar debemos crear una carpeta llamada **assets**, en esta carpeta se guardan todos los medios externos, imágenes, videos, música, iconos, etc. y dentro de esta carpeta crearemos una carpeta llamada **images**.

---


[Siguiente **&#129042;**](/markdown/015_Introducci%C3%B3n_Listas.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")