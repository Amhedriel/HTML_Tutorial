# Listas
Las listas en HTML sirven para listar el contenido, en función del contenido que vayamos a listar tenemos 3 tipos de **listas**:

* ***ul*** -> unordered list; Se utilizan cuando el orden de los elementos no influye.

* ***ol*** -> ordered list; Se utilizan cuando el orden de los elementos es importante.

* ***dl*** -> definition list; Se utilizan para hacer una lista de definiciones (diccionario).

Cada elemento de la lista se representa con la etiqueta `<li></li>`, tanto en las `ul` cómo las `ol`.

## ul listas desordenadas

Para poder crear una lista desordenada nosotros debemos colocar un `ul` y dentro colocar los items de esa lista, para poder colocar esos items debemos utilizar la etiqueta `<li></li>` que significa *list item* es decir elemento de lista.

~~~html
<body>
  <h1>Listas</h1>

  <ul>
    <li>Pan</li>
    <li>Huevos</li>
    <li>Azúcar</li>
    <li>Leche</li>
    <li>Aceite</li>
  </ul>
  
</body>
~~~
Con esta lista podemos indicar los items que necesitamos colocados en cualquier orden, no tienen prioridad de mayor a menor entre ellos en sí.

Un caso real en el uso de `ul` es en los menús.

En esl siguiente ejemplo, por cuestión de semántica colocaremos el `nav` por sobre de `ul` un `nav` tiene mayor categoría.

~~~html
<body>
  <h1>Listas</h1>

  <nav>
    <ul>
      <li><a href="/html/Web-demo/paginas/blog.html#post-1">Post 1</a></li>
      <li><a href="/html/Web-demo/paginas/blog.html#post-2">Post 2</a></li>
      <li><a href="/html/Web-demo/paginas/blog.html#post-3">Post 3</a></li>
      <li><a href="/html/Web-demo/paginas/blog.html#post-4">Post 4</a></li>
      <li><a href="/html/Web-demo/paginas/blog.html#post-5">Post 5</a></li>
    </ul>
  </nav>

  <ul>
    <li>Pan</li>
    <li>Huevos</li>
    <li>Azúcar</li>
    <li>Leche</li>
    <li>Aceite</li>
  </ul>
  
</body>
~~~
Este sería un ejemplo semánticamente correcto en comparación al ejemplo de la anterior sección.

Todos los menús de navegación se construyen de esta forma: `<nav></nav>`, dentro un `<ul></ul>` y sus respectivos `<li></li>` con los corrspondientes `<a></a>` y `href=""`; esto es la correcta construcción semántica de un **menu**.

---

## Listas ordenadas

La semantica de las listas ordenadas es practicamente la misma que las desordenadas.

~~~html
  <h2>Orden de aprendizaje en el desarrollo web</h2>
  <ol>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
  </ol>
~~~

Aqui en este caso concreto si es importante este orden, no podemos aprender diseño para una estructura que no conocemos, al igual que no podemos aprender interactividad para un elemento o arquitectura que no tenemos.

Visualmente se puede arreglar todo con CSS, pero lo importante es la estructura con HTML.

---
## Listas de definición

Las listas de definición que se representan con `<dl></dl>` (Definition List) y cada elemento de una lista de definición lleva 2 etiqueas:

* dt -> Definition term: El término que vamos a definir.

* dd -> Definition description: La descripción del término.

~~~HTML
  <h2>Lenguajes para el desarrollo web </h2>
  <dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language: Es un lenguaje de marcado que se usa para estructurar datos en una página web.
    </dd>

  </dl>
    <dl>
    <dt>CSS</dt>
    <dd>Cascade Style Sheets: Es un lenguaje de diseño que se utiliza para dar estilos a HTML.</dd>
  </dl>

  <dl>
    <dt>JavaScrip</dt>
    <dd>Es un lenguaje de programación para dar interactividad a un sitio web.</dd>
  </dl>
~~~

[Siguiente **&#129042;**](/markdown/016_Listas_Anidadas_Y_Atributos.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")