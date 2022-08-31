# Etiquetas de sección de contenido

Veremos la diferencia de usar ``<section>``, ``<article>`` y ``<aside>``.

## \<section>\</section>
Es un contenedor genérico que agrupa contenido que está relacionado. Cuando creamos bloques cuyo contenido es parte de un bloque total usaremos section.

El elemento HTML ``<section>`` representa una sección independiente genérica de un documento, que no tiene un elemento semántico más específico para representarlo. Las secciones siempre deben tener un encabezado, con muy pocas excepciones.

## \<article>\</article>
Es un contenedor que representa contenido independiente, es decir, podemos leer ese fragmento en cualquier otro sitio y tendría sentido por sí mismo.

El elemento HTML ``<article>`` representa una composición autónoma en un documento, página, aplicación o sitio, que está destinada a ser distribuible o reutilizable de forma independiente (por ejemplo, en sindicación). Los ejemplos incluyen: una publicación en el foro, un artículo de revista o periódico, o una entrada de blog, una tarjeta de producto, un comentario enviado por el usuario, un widget o gadget interactivo, o cualquier otro elemento de contenido independiente.

## \<aside>\</aside>
Se utiliza para representar contenido relacionado pero que no forma parte del contenido principal.

El elemento HTML ``<aside>`` representa una parte de un documento cuyo contenido solo está relacionado indirectamente con el contenido principal del documento. Los apartes se presentan con frecuencia como barras laterales o cajas de llamadas.

## Anidamiento:
Un section puede contener ``<article>``,por ejemplo, si tenemos varios artículos que hablan sobre noticias, deben ir dentro de un ``<section></section>``, ya que es contenido relacionado entre sí, y los ``<article></article>`` serían contenido independiente porque podríamos leer uno sin haber leido el resto, y seguiría teniendo sentido.

El `<article></article>` es definido como un componente de la página de contenido independiente, esto implica que esta etiqueta pueda tener un `<header></header>` y un `<footer></footer>` propios.

También existe el caso en el que un `<article></article>` contenga varias secciones, el artículo independiente podría ser navegadores y este contener dentro secciones como navegadores más utilizados en 2022.

```html
<body>
  <Header>
    <h1>NOTICIAS NACIONALES</h1>
  </Header>
  <main>
    <section>
      <h2>Noticas del día</h2>
      <article>Noticia 1</article>
      <article>Noticia 2</article>
      <article>Noticia 3</article>
    </section>
  </main>
  <footer>David A. Beltrán R. de C. 30 - 08 - 2022</footer>
</body>
```
Este sería un ejemplo sencillo, pero esto semánticamente es incorrecto, podemos detectar los errores en una págia ofical "validator.w3.org" (revisarlo en [recursos](/markdown/Recursos.md "Apartado para el uso de herramientas"))

![Validator](/media/Error_article.png)

Como pòdemos observar no está marcando **Warning** nos dice que los `article` necesitan un `<header></header>` que no son capaces de identificar los `header` en los artículos; es decir, como los **artículos** son contenido independiente deben tener su propio **header** y su propio **footer** por lo tanto:

~~~html
<body>
  <Header>
    <h1>NOTICIAS NACIONALES</h1>
  </Header>
  <main>
    <section>
      <h2>Noticas del día</h2>
      <article>
        <h3>Noticia 1</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta libero debitis incidunt itaque illo magni? Reprehenderit beatae commodi placeat maxime ipsam in optio quia sunt rerum, vero corrupti? Repudiandae, mollitia.</p>
      </article>
      <article>
        <h3>Noticia 2</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut debitis, cupiditate deserunt quidem accusantium maxime facilis commodi, sed ipsa reprehenderit quasi sapiente tempore delectus animi tempora, magnam assumenda illo itaque deleniti accusamus laboriosam libero possimus. Quis, consectetur hic sequi natus accusamus commodi repellendus possimus! Rerum libero soluta, necessitatibus totam et quisquam ipsa vel qui dolor illo! Reiciendis, laborum iusto. Quidem excepturi quisquam corporis consectetur architecto culpa sunt ullam, rerum perspiciatis laborum nesciunt sint magnam voluptatum quasi tempore ducimus totam recusandae!</p>
      </article>
      <article>
        <h3>Noticia 3</h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt facere amet fugit ducimus perspiciatis odit aperiam, id at, eius, laboriosam commodi? Reprehenderit dicta iure est repellat nesciunt eius voluptate, at debitis, ut excepturi error voluptas ab modi? Eos saepe perspiciatis quo. Libero, totam architecto nobis nihil quam numquam atque, iure asperiores dolorum inventore perspiciatis, ex dicta nulla. Doloribus, alias. Iure.</p>
      </article>
    </section>
  </main>
  <footer>David A. Beltrán R. de C. 30 - 08 - 2022</footer>
</body>
~~~

![Validator](/media/Estructura_correcta_article.png)

Entonces podemos ver qoe el documento es completamente correcto, no hay ningún warning para mostrar.

Para los `article` el `header` y el `footer` no son obligatorios, pero, como los `article` son contenido independiente se les permite tener esto.

~~~html
<article>
        <header>
          <h3>Noticia 1</h3>
        </header>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta libero debitis incidunt itaque illo magni? Reprehenderit beatae commodi placeat maxime ipsam in optio quia sunt rerum, vero corrupti? Repudiandae, mollitia.</p>
        <footer>La noticia ocurrió en Buenos Aires.</footer>
</article>

~~~

Para agregar, podemos tener un ``section`` con más `section` dentro, es decir que en el `main` podriamos tener uh `h1` que pusiera **section** como contenedor y donde abrimos el `section` podríamos tener el `h1` como contenedor en lugar que fuera el título principal del
`main` y debajo de este `h1` tener un `section`. Esto es completamente valido semanticamente porque ``section`` lo que hace es agrupar contenido relacionado, por lo que en este caso todo lo que estamos agrupando son noticias por lo tanto es válido.

~~~html
<body>
  <header>
    <h1>NOTICIAS NACIONALES</h1>
  </header>
  <main>
    <section>
      <h2>Section como contenedor</h2>
      <section>
        <h2>Noticas del día</h2>
        <article>
          <header>
            <h3>Noticia 1</h3>
        </header>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta libero debitis incidunt itaque illo magni? Reprehenderit beatae commodi placeat maxime ipsam in optio quia sunt rerum, vero corrupti? Repudiandae, mollitia.</p>
        <footer>La noticia ocurrió en Buenos Aires</footer>
        </article>
        <article>
        <h3>Noticia 2</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aut debitis, cupiditate deserunt quidem accusantium maxime facilis commodi, sed ipsa reprehenderit quasi sapiente tempore delectus animi tempora, magnam assumenda illo itaque deleniti accusamus laboriosam libero possimus. Quis, consectetur hic sequi natus accusamus commodi repellendus possimus! Rerum libero soluta, necessitatibus totam et quisquam ipsa vel qui dolor illo! Reiciendis, laborum iusto. Quidem excepturi quisquam corporis consectetur architecto culpa sunt ullam, rerum perspiciatis laborum nesciunt sint magnam voluptatum quasi tempore ducimus totam recusandae!</p>
        </article>
        <article>
        <h3>Noticia 3</h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nesciunt facere amet fugit ducimus perspiciatis odit aperiam, id at, eius, laboriosam commodi? Reprehenderit dicta iure est repellat nesciunt eius voluptate, at debitis, ut excepturi error voluptas ab modi? Eos saepe perspiciatis quo. Libero, totam architecto nobis nihil quam numquam atque, iure asperiores dolorum inventore perspiciatis, ex dicta nulla. Doloribus, alias. Iure.</p>
        </article>
      </section>
    </section>
  </main>
  <footer>David A. Beltrán R. de C. 30 - 08 - 2022</footer>
</body>
~~~




