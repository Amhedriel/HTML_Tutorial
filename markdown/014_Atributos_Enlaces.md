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

Recordar que el recurso no se abre, simplemente se descarga
