# Introducción a los formularios

La parte más importante de los formularios es poder interactuar con los usuarios, hasta ahora nosotros presentamos información, estuctura de la página con títulos, párrafos, menus y ese tipo de cosas, con los formularios pedimos información al usuario.

Prácticamente todas las páginas web del mundo, salvo las informativas, tienen un formulario, ya sea para ingresar en la página, pagos online o solamente para apuntar correo electrónico y que lleguen noticias de un tema en concreto.

Este es un campo complejo y completo.


La estructura básica de un formulario se compone de 4 elementos.

## Estructura básica de un formulario

## form
Es la etiqueta que engloba nuestro formulario.


## label
Sirve para escribir el nombre del campo rellenar.


## input
Sirve para crear un campo que le permitirá al usuario interactuar.


## button
Crea un botón que permitirá enviar el formulario.

Crearemos un formulario sencillo como ejemplo.

~~~html
<body>
  <form>
    <label>Nombre</label>
    <input>
    <button>Enviar formulario</button>
  </form>
</body>
~~~
La cual muestra:

![Formulario_básico](/media/Formulario_basico.png "Formulari básico")

El comportamiento de un formulario es cojer la información rellenada y enviarla a un server mediante el `action=""`.

~~~html
<form action="enviar.html">
~~~

La página enviará un error porque no existe la ruta de "enviar.html" dentro de la carpeta formularios, entonces `action` lo que normalmente lleva o un documento de servidor que podría ser PHP o lo que se hace es bloquear el envio del formulario a través de JavaScript y una vez que se gestionó ese formulario una vez hechas las modificaciones necesarias, nosotros pausamos el envío con JS y después lo enviamos con JS.

[Siguiente **&#129042;**](/markdown/023_Formularios_Input_Label.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")

