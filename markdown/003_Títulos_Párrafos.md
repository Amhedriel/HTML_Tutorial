# Títulos y párrafos

Ahora veremos los encabezados en HTML.

## \<h1> Encabezados

Los elementos ``<h1>`` y ``<h6>`` especifican encabezados. Se puede utilizar un encabezado para titular el documento de la página web o partes de su contenido. Úsalos para señalar títulos y nombres de contenido.

~~~html
<h1>Heading text - Level 1. Most Important Heading</h1>
<h2>Heading text - Level 2</h2>
<h3>Heading text - Level 3</h3>
<h4>Heading text - Level 4</h4>
<h5>Heading text - Level 5</h5>
<h6>Heading text - Level 6. Least Important Heading</h6>
~~~

Los *elementos* de **encabezado** implementa seis niveles de encabezado del documento, `<h1></h1>` es el más importante y se recomienda tener solo uno por página, y `<H6></H6>` el menos importante.
Un elemento de encabezado describe brevemente el tema de sección que presenta.



~~~html
<body>
	<h1>Harry Potter</h1>
	<h2>Sinopsis</h2>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed, aspernatur. Voluptas dolor aliquam necessitatibus doloribus obcaecati. Ducimus eum eveniet molestias praesentium deleniti, sunt, animi assumenda molestiae pariatur eos et est?</p>

	<h2>Novelas</h2>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet repellendus, iste est libero unde quo ut quia perspiciatis, quos officiis doloribus quas reprehenderit officia nihil suscipit distinctio culpa.</p>

	<h3>Harry Potter y la Piedra Filosofal</h3>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea corporis magnam sed pariatur, non aliquid tempora placeat animi assumenda perspiciatis. Dolorem, tempore commodi minima, consequatur odit voluptatum doloremque dolorum quas inventore aliquam optio, deleniti nemo nisi nam est iusto ea? Quisquam vitae sequi sunt omnis commodi veritatis sed dolorum ex esse voluptas eveniet voluptatem, accusantium error alias voluptatibus asperiores impedit a ab tenetur perspiciatis. Maxime molestias necessitatibus voluptas repellendus commodi atque sint deleniti magni ipsam est eos rerum porro recusandae tenetur fugit eius, aliquam delectus iusto dignissimos accusamus sed. Veritatis sint reprehenderit minus inventore quos consequatur adipisci, illum dolore! Velit!</p>
    
</body>
~~~

Por la semántica podemos decir que `h3` es parte de `h2`que tenemos por encima que sería Novelas y así al principal que es el `h1`.

Lo principal es: que un h3 debe pertenecer a un contenido que tenga un h2 y un h2 debe pertenecer a un contenido que tenga un h1.

---

## \<p>: El elemento Párrafo (paragraph)

El elemento HTML ``<p>`` representa un párrafo. Los párrafos generalmente se representan en medios visuales como bloques de texto separados de bloques adyacentes por líneas en blanco y / o sangría de primera línea, pero los párrafos HTML pueden ser cualquier agrupación estructural de contenido relacionado, como imágenes o campos de formulario.

Los párrafos son elementos de nivel de bloque y, en particular, se cerrarán automáticamente si se analiza otro elemento de nivel de bloque antes de la etiqueta de cierre. Consulte "Omisión de etiquetas"``</p>``.

~~~html
<body>
	<h1>Harry Potter</h1>
	<h2>Sinopsis</h2>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed, aspernatur. Voluptas dolor aliquam necessitatibus doloribus obcaecati. Ducimus eum eveniet molestias praesentium deleniti, sunt, animi assumenda molestiae pariatur eos et est?</p>

	<h2>Novelas</h2>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet repellendus, iste est libero unde quo ut quia perspiciatis, quos officiis doloribus quas reprehenderit officia nihil suscipit distinctio culpa.</p>

	<h3>Harry Potter y la Piedra Filosofal</h3>
	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea corporis magnam sed pariatur, non aliquid tempora placeat animi assumenda perspiciatis. Dolorem, tempore commodi minima, consequatur odit voluptatum doloremque dolorum quas inventore aliquam optio, deleniti nemo nisi nam est iusto ea? Quisquam vitae sequi sunt omnis commodi veritatis sed dolorum ex esse voluptas eveniet voluptatem, accusantium error alias voluptatibus asperiores impedit a ab tenetur perspiciatis. Maxime molestias necessitatibus voluptas repellendus commodi atque sint deleniti magni ipsam est eos rerum porro recusandae tenetur fugit eius, aliquam delectus iusto dignissimos accusamus sed. Veritatis sint reprehenderit minus inventore quos consequatur adipisci, illum dolore! Velit!</p>
    
</body>
~~~

> *Nota: Los párrafos HTML no tienen ningún formato; Debe agregarse manualmente.

---

## \<pre> (Texto HTML **pre***formateado*)

Representa texto preformateado.

El texto en este elemento típicamente se muestra en una fuente fija, no proporcional, exactamente como es mostrado en el archivo. Los espacios dentro de este elemento también son mostrados como están escritos.

~~~html
    <!-- Un podo de código CSS -->
    <pre>
    body{
        
        color: red;
    }

    a   {

        color:green;
    
    }
    </pre>
~~~
RESULTADO:

~~~css
    body{
        
        color: red;
    }

    a   {

        color:green;
    
    }
~~~

Esta etiqueta mostrará un resultado igual al escrito dentro.

[Siguiente **&#129042;**](/markdown/004_Header_Main_Footer.md "Resumen")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")