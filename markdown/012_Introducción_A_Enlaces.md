# Introducción a enlaces (anclas)

Los enlaces son los que le dan el funcionamiento a la web tal como nosotros la conocemos.

## Enlaces:
También conocidos por links popularmente. Su objetivo es conectar una página web con otra página web, con un recurso que puede ser tanto interno como externo, o con otro sitio web.

Tienen el atributo obligatorio ``href``, donde le especificamos la ruta del recurso o sitio que queremos obtener.

Tienen el atributo obligatorio ``target``, que configura cómo queremos visualizar el recurso o sitio que solicitamos.

Crearemos 2 archivos HTML `index` y `contacto`, veremos como comunicar ambas páginas a travéz de un link.

Veremos la forma de ponerlos.

## **\<a>**

Los enlaces se establecen con la etiqueta ``<a>`` que viene de (ancla).

Por defecto no aparece el atributo `href=""` es lo opuesto que tiene el atributo obligatorio `href` y es donde le especificamos la ruta del recurso o sitio que queremos obtener.

También tiene el atributo `target`.

En nuestro caso *index.html* y *contacto.html* están en el mismo nivel lo que significa que los 2 están dentro de la misma carpeta.

~~~html
<body>
  <h1>HOME</h1>
  <a href="contacto.html">Ir a contacto</a>
</body>
~~~
Con esto podremos ver en la página nuestro link.

Su aspecto por defecto es de color azul subrayado y se puede cambiar con CSS.

Si hacemos clik en ir a contacto entonces podemos ver que la ruta a cambiado y estamos en *contacto.html*.

Para volver a la página principal *index.html* editaremos *contacto.html* con un link a *index.html*.

~~~html
<body>
  <h1>Contacto</h1>

  <a href="index.html">Ir al inicio</a>
</body>
~~~
Con esto podremos tener un link a *index.html* o **home**

---
## **target**

 [Siguiente **&#129042;**](/markdown/013_Rutas_Absolutas_Relativas.md "Resumen")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")
