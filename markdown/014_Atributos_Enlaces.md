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

## Estructura de HTML con imágenes

En primer lugar debemos crear una carpeta llamada **assets**, en esta carpeta se guardan todos los medios externos, imágenes, videos, música, iconos, etc. y dentro de esta carpeta crearemos una carpeta llamada **images**.

## Navegación con Anclas

Haremos navegación internas dentro de nuestro sitio web, para este ejemplo crearemos un Blog.

Tendremos 5 posts con texto de relleno (Lorem) y navegaremos entre ellos.


