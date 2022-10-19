# Aside

Se utiliza para representar contenido indirectamente relacionado pero que no forma parte del contenido principal.

El elemento HTML ``<aside>`` representa una sección de una página que consiste en contenido que está indirectamente relacionado con el contenido principal del documento. Estas secciones son a menudo representadas como barras laterales o como inserciones y contienen una explicación al margen como una definición de glosario, elementos relacionados indirectamente, como publicidad, la biografía del autor, o en aplicaciones web, la información de perfil o enlaces a blogs relacionados.

### **Notas de uso:**

No utilices el elemento ``<aside>`` para etiquetar *texto entre paréntesis*, ya que este tipo de texto se considera parte del flujo principal.

Es decir nosotros tenemos una web donde hablamos de curso de desarrollo web gratuitos y aqui podemos tener nuestras tarjetas con links que te lleven a los sitios de esos cursos. un contenido relacionado pero que no forma parte del contenido principal podría ser un menú con links a cursos de pago, links de recursos personales, etc. esto sería un contenido indirectamente relacionado, habla de lo mismo pero no es parte del principal, en cuestiones de semántica y donde colocarlo, tanto la W3C como la MDN no tiene ningún problema que esté fuera del `main` o dentro del `main`, dado la definicion de `aside` y teniendo que cuenta que es un contenido relacionado pero que no forma parte del contenido principal normalmente lo de dejaríamos fuera.

~~~html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=, initial-scale=1.0">
    <title>Aside</title>
</head>
<body>
    <header>
        <h1>Cursos de desarrollo web gratuitos</h1>
    </header>
    <aside>Visita mi canal de YouTube</aside>
    <aside>Nuestros cursos premiun</aside>
    <main>
        <h2>Curso introductorio de HTMl 5</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad deserunt sint ea, inventore enim odio at voluptatibus possimus? Adipisci, expedita. Corporis harum mollitia, amet iure tempore eos et itaque aliquam. Recusandae eligendi, suscipit ipsa illum dolorum rem consequuntur odio placeat odit voluptas provident sunt voluptatum eum accusantium eos, quaerat inventore veritatis. Et debitis nulla facilis quia veniam. Reiciendis earum excepturi, quos reprehenderit vel blanditiis enim! Aut facilis eveniet adipisci voluptatem aspernatur impedit aliquid magni harum suscipit veniam natus provident, inventore consectetur repellat enim mollitia excepturi, sed error! Aperiam, quam est.</p>
    </main>
</body>
</html>
~~~

Revisando lo escrito arriba veremos que es semanticamente correcto en la W3C.

![aside](/media/Aside_correcto.png "Ejemplo aside correcto")


[Siguiente **&#129042;**](/markdown/008_Elementos_Bloque.md "Resumen")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")