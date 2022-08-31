# Article encerrando section

Ahora veremos un `article` que encierra `section` en su interior.

~~~html
<body>
  <main>
  <header>
    <h1>NOTICIAS NACIONALES</h1>
  </header>
	<article>
		<h2>Navegadores más utilizados en 2022</h2>
	</article>
	</main>
	<footer>David A. Beltrán R. de C. 30 - 08 - 2022</footer>
</body>
~~~

~~~html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sección de contenido 2</title>
</head>
<body>
  <main>
  <header>
    <h1>NOTICIAS NACIONALES</h1>
  </header>
	<article>
		<h2>Navegadores más utilizados en 2022</h2>
	</article>
		<section>
			<h3>Chrome</h3>
			<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, excepturi commodi cumque odio provident nihil quia, esse voluptatum illum rem quidem inventore itaque, accusantium sunt adipisci beatae doloribus eveniet eligendi quae iure quibusdam aspernatur maxime culpa? Laudantium dicta ab ullam animi quidem impedit vitae doloribus sed quae harum alias commodi libero quas voluptatibus officiis soluta, numquam placeat! Enim quia impedit expedita ducimus perspiciatis laborum nam corrupti. Harum.</p>
		</section>
		<!-- Después hablaremos de Fire Fox, por lo tanto esto sería otra sección, divide  el contenido pero sigue perteneciendo al mismo `article` que son "Navegadores más utilizados 2022" -->
		<section>
			<h3>Fire Fox</h3>
			<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos saepe inventore asperiores earum sed ducimus tenetur, amet dicta, porro nisi voluptate voluptatum est adipisci alias eligendi minima sunt quasi? Amet sapiente, recusandae cupiditate eaque beatae consequuntur vero at aut fugit architecto fuga debitis modi? Perspiciatis fugit beatae veritatis! Doloremque error exercitationem architecto repellat neque veritatis officiis dolor voluptatibus soluta voluptate.</p>
		</section>
	</main>
	<footer>David A. Beltrán R. de C. 30 - 08 - 2022</footer>
</body>
</html>
~~~

Este sería nuestro `article` principal donde vamos a encerrar todo el contenido independiente que hable sobre navegadores, pero cada una de las secciones que hable de un navegador ese `section` lo que hará es dividir cada una de las partes.

Tenemos un `article` con su título y un `section` que también tiene un título y una descripción.

En este caso también podríamos crear un `header`y debajo colocar un `footer`

~~~html
<body>
  <main>
  <header>
    <h1>NOTICIAS NACIONALES</h1>
  </header>
	<article>
		<h2>Navegadores más utilizados en 2022</h2>
	</article>
		<section>
			<header>
				<h3>Chrome</h3>
			</header>
				<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae, excepturi commodi cumque odio provident nihil quia, esse voluptatum illum rem quidem inventore itaque, accusantium sunt adipisci beatae doloribus eveniet eligendi quae iure quibusdam aspernatur maxime culpa? Laudantium dicta ab ullam animi quidem impedit vitae doloribus sed quae harum alias commodi libero quas voluptatibus officiis soluta, numquam placeat! Enim quia impedit expedita ducimus perspiciatis laborum nam corrupti. Harum.</p>
				<footer>Creado por Google</footer>
		</section>
		<!-- Después hablaremos de Fire Fox, por lo tanto esto sería otra sección, divide  el contenido pero sigue perteneciendo al mismo `article` que son "Navegadores más utilizados 2022" -->
		<section>
			<h3>Fire Fox</h3>
			<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos saepe inventore asperiores earum sed ducimus tenetur, amet dicta, porro nisi voluptate voluptatum est adipisci alias eligendi minima sunt quasi? Amet sapiente, recusandae cupiditate eaque beatae consequuntur vero at aut fugit architecto fuga debitis modi? Perspiciatis fugit beatae veritatis! Doloremque error exercitationem architecto repellat neque veritatis officiis dolor voluptatibus soluta voluptate.</p>
		</section>
	</main>
	<footer>David A. Beltrán R. de C. 30 - 08 - 2022</footer>
</body>
~~~

Ahora observamos que al hacer la revisión de nuestro html no encontrará ningun error al ser validas las opciones que indicamos por la W3C.

![Article](/media/Article_Encerrando_Section_sin_error.png "Article encerrando section correcto")


