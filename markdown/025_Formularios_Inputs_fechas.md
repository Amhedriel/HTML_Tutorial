# Inputs para fechas

## input type:

Ahora veremos algunos tipos de input que existen:
* button -> Se comporta igual que un botón \<button><button>.
* color -> Se utiliza para especificar un color.

* date -> Se utilizapara introducir una fecha.
* datetime -> OBSOLETO.
* datetime-local -> Fecha y hora, no funciona en firefox.
* time -> Se utiliza para introducir una hora.
    - Se recomienda usar datetime-local y time para seleccionar fecha y hora
* month -> Se utiliza para introducir un mes.
* week -> Se utiliza para introducir el número de semana del año.

* hidden -> Campo oculto, puede contener valor pero no se mostrará.
* email -> Se utiliza para introducir un email.
* number -> Se utiliza para valores numéricos.
* password -> Se utiliza para contraseñas
* range -> Se utiliza para establecer un rango.
* reset -> Se utiliza para resetear el formulario.
* search -> Se utiliza para las barras de búsqueda.
* submit -> Se utiliza para enviar el formulario.
* tel -> Se utiliza para introducir números telefónicos.
* text -> Valor por defecto.
* url -> Se utiliza para introducir URLs.

## **inputs de fecha**

Veremos algunos tips:

## date
Es un campo que se utiliza para introducir *día/mes/año*

~~~html
<body>
  <form>
    <input type="date">
  </form>
</body>
~~~
<body>
  <form>
    <input type="date">
  </form>
</body>

## datetime

OBSOLETO

## datetime-local

Esto es para fecha y hora, pero no funciona en Fire Fox.

~~~html
<body>
  <form>
    <input type="datetime-local">
  </form>
</body>
~~~

<body>
  <form>
    <input type="datetime-local">
  </form>
</body>

Al desplegar se ve muy parecido al otro pero, tiene el añadido para poder añadir horas y minutos.

Por este mismo efecto se recomienda utilizar el `<input type="date">`sumando `<input type="time">`.

~~~html
<body>
  <form>
    <input type="date">
    <input type="time">
  </form>
</body>
~~~


<body>
  <form>
    <input type="date">
    <input type="time">
  </form>
</body>

Con esto arreglaríamos el problema de Fire Fox u otros navegadores que no soportan `datetime-local`

## month

Se utuiliza para introducir el mes.

~~~html

<body>
  <form>
    <input type="month">
  </form>
</body>
~~~

<body>
  <form>
    <input type="month">
  </form>
</body>

## week

Un tipo no muy utilizado hoy en día pero debemos tener presente que existe.

~~~html

<body>
  <form>
    <input type="week">
  </form>
</body>
~~~

<body>
  <form>
    <input type="week">
  </form>
</body>

Con lo cual podremos escoger una semana del año.

[Siguiente **&#129042;**](/markdown/026_Formularios_Inputs_M%C3%B3viles.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")