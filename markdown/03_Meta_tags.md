# HTML Meta Tags

Los metadatos son simplemente datos sobre datos. Normalmente (con excepciones) no aparece en la pantalla del navegador. En cambio, solo existe en código HTML para ser analizado por las máquinas. Una de estas máquinas, por supuesto, es el todopoderoso motor de búsqueda.

En SEO, las estrategias integrales son importantes. Mientras que la construcción de vínculos de retroceso mediante el uso de la etiqueta `<a>` es excelente para crear autoridad en el sitio web, también lo son las meta etiquetas HTML. Las meta etiquetas se pueden usar para muchos propósitos, desde la creación de diseños hasta informar a los motores de búsqueda dónde buscar qué en un sitio.

Por ejemplo, cuando buscas algo en Google, ahora genera automáticamente un fragmento de "respuesta" en la parte superior de tu SERP.

![Fragmento de respuesta](/media/Fragmento%20de%20respuesta.jpg "Fragmento de respuesta")

Si hace clic en ese resultado, Google lo llevará inmediatamente a la parte relevante de la página, resaltando la respuesta a su consulta.

![Parte Relevante](/media/Parte%20Relevante.jpg "Parte Relevante")

En esta sección, repasaremos las meta etiquetas más cruciales para SEO, su propósito y consejos sobre cómo optimizar su uso.

> *Nota: Si bien hay más de 90 categorías de meta etiquetas, no todas forman parte de las métricas de clasificación SEO.

## Meta ventana gráfica

La etiqueta meta viewport es responsable de representar correctamente su página en pantallas de diferentes tamaños. Esto es importante si desea que su sitio web sea accesible no solo en el escritorio sino también en una tableta, teléfono inteligente u otro dispositivo.

![Meta Viewport](/media/Viewport.jpg "Meta Viewport")

### Propósito SEO

Nadie quiere visitar un sitio web solo de escritorio en su teléfono. Después de todo, en 2019, más de la mitad del tráfico de Internet provino de dispositivos móviles. Google lo sabe, por lo que penalizan a los sitios web que no utilizan meta viewport y diseño receptivo.

> *Nota: Una etiqueta meta viewport no es suficiente para hacer que un sitio web sea compatible con dispositivos móviles. Como aprendiste en la sección de diseño web, el diseño receptivo lleva la peor parte del trabajo.

Ejemplo de código:

Esta es la forma más común de agregar una etiqueta meta viewport en su código HTML:

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

### Prácticas recomendadas

Agregue la etiqueta meta viewport a todas sus páginas web.

A menos que esté familiarizado con la etiqueta viewport, use la versión más común (consulte más arriba).
Compruebe si su página es compatible con dispositivos móviles [con esta herramienta](https://search.google.com/test/mobile-friendly).

## Etiqueta de título

¿Conoces esos titulares en los que se puede hacer clic en tus SERP? Esta es la única meta etiqueta que realmente verá cuando mire un sitio web, ya que también aparece en la pestaña de su navegador. Se crea a través de la etiqueta <title>.


![Meta Title](/media/Meta%20Title.jpg "Meta Title")


> *Nota: Una página web solo puede tener una etiqueta <título>.

### Propósito SEO rating

No debes juzgar un libro por su portada, pero los usuarios suelen juzgar una página por su título. La etiqueta `<title>` es el contenido principal por el cual el usuario decide si desea o no visitar su página.

Ejemplo de código:

La etiqueta `<title>` se agrega al elemento `<head>` de esta manera:

```html
<head>
  <title>This is the title of the page.</title>
</head>
```
### Prácticas recomendadas

- Tenga un título único para cada página de su sitio web.
- KISS: mantenle corto y simple.
- Agregue palabras clave y haga coincidir los términos de búsqueda.
- Evita los títulos vagos.
- Atrae la atención pero evita los títulos clickbait-y.
- No más de 60 caracteres.

> *Note: Sometimes, Google might stray off and use a different title for your web page. This is usually done to increase perceived relevance to the user’s search.

## Meta description tag

Dentro del elemento `<head>`, encontrarás etiquetas `<meta>`, la forma típica de agregar información adicional para que los motores de búsqueda te entiendan.

La meta descripción se usa típicamente para los SERP junto al título: es la descripción justo debajo.

![Meta Description](/media/Meta%20Description.jpg "Meta Description")

> *Nota: Si bien las descripciones pueden usarse para los fragmentos de SERP, Google ha dicho que no usan la meta etiqueta de descripción en sus clasificaciones.

### Propósito SEO

Trátelo como un resumen general de su página web. Por encima de todo, es un lanzamiento: su objetivo principal es convencer al usuario de que visite su sitio en una o dos oraciones.

Ejemplo de código:

La etiqueta de meta descripción debería tener un aspecto similar al siguiente:

```html
<head>
  <meta name=”description” content=”Short description of the page”>
</head>
```

### Prácticas recomendadas

- Cada página de su sitio web debe tener una descripción única.
- Los resúmenes de contenido deben ser relevantes y precisos.
- ¡Incluye palabras clave!
- Use mayúsculas y minúsculas (comience la descripción con una letra mayúscula).
- Evite descripciones vagas o clickbait-y.
- La longitud óptima debe ser de alrededor de 140 caracteres.

## Meta robots tag

Meta robots ¿Recuerdas cómo los robots de los motores de búsqueda rastrean e indexan las páginas? Bueno, los desarrolladores también pueden proporcionar a estos bots pautas instructivas sobre cómo indexar información en páginas específicas. Por ejemplo, ¡puede indicar al robot que no indexe páginas enteras en absoluto!

Hay dos formas de hacerlo:
  1. A través de un archivo .txt robots,
  2. O usando una etiqueta meta robots.

> *Nota: Los robots también se conocen comúnmente como arañas: ¡son los robots que se arrastran por tus páginas!

## Robots.txt vs Meta robots tag

Cuando un robot quiere entrar en su sitio, primero verifica el archivo .txt sus robots o la información especificada en la etiqueta meta robots. Hay dos diferencias principales entre ellos:

  1. Mientras que los robots.txt emiten directivas (o sugerencias) sobre cómo indexar el contenido, las instrucciones de la meta etiqueta son más firmes. Sin embargo, con ambas opciones, los rastreadores no tienen que seguir las directivas, y las arañas más maliciosas podrían omitirlas fácilmente.

  2. Las etiquetas de los robots meta solo pueden decirle al rastreador que no indexe una página web específica, mientras que los archivos .txt robots tienen la opción de bloquear un sitio web completo.

### Propósito SEO

Si hace un mal uso de la etiqueta meta robots, su sitio podría enfrentar consecuencias desastrosas en las páginas de resultados de búsqueda. Hay dos valores principales que necesita saber:

  - index/noindex: informa a los motores de búsqueda si debe mostrar su página en sus resultados de búsqueda;

  - follow/nofollow: indica a los motores de búsqueda cómo deben actuar con los enlaces de tus páginas, es decir, si deben confiar y seguir los enlaces que has añadido.

> *Nota: Si desea agregar nofollow a un enlace individual, en lugar de una etiqueta meta robots, debe agregar ``rel="nofollow"`` a los atributos de la etiqueta ``<a>``.

Ejemplo de código:

Así es como puede combinar los valores mencionados anteriormente:

```html
<meta name=”robots” content="noindex, nofollow">

<meta name=”robots” content="index, follow">

<meta name=”robots” content="noindex, follow">

<meta name=”robots” content="index, nofollow">

<meta name=”robots” content="none">
```
> *Nota: De forma predeterminada, los meta robots están configurados para indexar, seguir. Escribir content="none" lo establecerá en sus valores predeterminados.

### Prácticas recomendadas

  - Las etiquetas de Meta robots solo deben usarse cuando no desea que una página se indexe / rastree.
  - No utilices la etiqueta meta robots en el archivo .txt robots.
  - Recuerde que los rastreadores maliciosos probablemente ignorarán sus directivas de meta robots. Si hay información sensible o confidencial involucrada, utilice mecanismos de seguridad alternativos (por ejemplo, protección con contraseña) para proteger su sitio web.

---

Las meta etiquetas se pueden utilizar para informar a Google de qué se trata el contenido, como por ejemplo: podemos indicar que esta página es solo para adultos:

   	<meta name=”rating” content=”adult”>

Hazle saber a Google que no quieres que se traduzca esta página:

    <meta name="google" content="notranslate">


Ahora que has intentado crear y formatear sitios web simples, diríamos que ya es hora de que subas tu juego y comiences a usar meta etiquetas. Después de todas estas lecciones, ¡(con suerte) sabes cómo!

---

[Siguiente **&#129042;**](/markdown/README.md "Ir a Readme")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")