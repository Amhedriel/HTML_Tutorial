# Elementos de bloque

Los elementos, en HTML (lenguaje de marcas de hipertexto - Hypertext Markup Language) usualmente son elementos "en bloque" o elementos "en línea". Un elemento en bloque ocupa todo el espacio de su elemento padre (contenedor), creando así un "bloque". Este artículo ayuda a explicar lo que esto significa.

Los navegadores suelen mostrar el elemento a nivel de bloque con un salto de línea antes y después del elemento.

Los elementos de bloque van a ocupar todo el ancho disponible aunque su contenido no lo ocupe.

Ej:

~~~html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bloque</title>
</head>
<body>
    <!-- Los elemntos de bloque van a ocupar todo el ancho disponible aunque su contenido no lo haga, por lo que los elementos que pongamos a continuación satarán a la siguiente línea. -->
    <h1>Soy un elemento de bloque</h1>
    <p>Soy otro elemento de bloque</p>
</body>
</html>
~~~

Como vemos tenemos un ``h1`` y también un ``p`` pero en el navegador el `p` no se colocará dentro del `h1`, esto debido a que es un **elemento de bloque**, una forma de comprobarlo es con la consola del navegador.

![Elementos de bloque](/media/Elementos_de_bloque.png "El h1 y el p se ordenan uno debajo de otro")

## **Uso**
Los elementos de bloque sólo deben aparecer dentro del elemento <body>.
Elementos en bloque vs. en línea
Hay un par de diferencias clave entre los elementos en bloque y elementos en línea:

## **Formateo**
De forma predeterminada, los elementos de bloque comienzan en una nueva línea, pero los elementos en línea pueden comenzar en cualquier parte de una línea.
Modelo de contenido

En general, los elementos en bloque pueden contener elementos en línea y otros elementos en bloque. Inherente a esta distinción estructural es la idea de que los elementos en bloque crean estructuras "más grandes" que los elementos en línea.

La distinción entre elementos en bloque frente a elementos en línea se utiliza en las especificaciones de HTML hasta la 4.01. En HTML5, esta distinción dual se sustituye por un conjunto más complejo de categorías de contenido. La categoría "en bloque" corresponde aproximadamente a la categoría de contenido dinámico en HTML 5, mientras que "en línea" se corresponde con contenido estático, pero hay categorías adicionales.

## **Elementos**
La siguiente es una lista completa de todos los elementos en bloque de HTML (aunque "en bloque" no se define técnicamente para los elementos que son nuevos en HTML5).

~~~html
    <address>
Información de contacto.

    <article> HTML5
Contenido de Articulo.

    <aside> HTML5
Contenido adicional.

    <audio> HTML5
Reproductor de audio

    <blockquote>
Bloque de "cita".

    <canvas> HTML5
Dibujo canvas.

    <dd>
Descripción de definición.

    <div>
División de documento.

    <dl>
Lista de definición.

    <fieldset>
Etiqueta de conjunto de campos.

    <figcaption> HTML5
Leyenda de figura.

    <figure> HTML5
Grupos contenido multimedia con una leyenda (ver <figcaption>).

    <footer> HTML5
Sección o pie de página.

    <form>
Formulario de entrada.

    <h1> (en-US), 
        <h2> (en-US), 
            <h3> (en-US), 
                <h4> (en-US), 
                    <h5> (en-US), 
                        <h6> (en-US)
Niveles de cabecera 1-6.

    <header> HTML5
Sección o cabecera de página.

    <hgroup> HTML5
Grupos información de encabezado.

    <hr>
Regla Horizontal (línea divisoria).

    <li>
Elemento de lista.

    <main>
Engloba el único contenido central del documento.

    <nav>
Contiene enlaces de navegación.

    <noscript>
Contenido para ser usado si los scripts no son soportados o permitidos.

    <ol>
Lista ordenada.

    <output> (en-US) HTML5
Formulario de salida.

    <p>
Párrafo.

    <pre>
Texto preformateado.

    <section> HTML5
Sección de una página web.

    <table>
Tabla.

    <tfoot> (en-US)
Pie de tabla.

    <ul>
Lista no ordenada.

    <video> HTML5
Reproductor de vídeo.

~~~

[Siguiente **&#129042;**](/markdown/009_Elementos_De_L%C3%ADnea.md "Resumen")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")