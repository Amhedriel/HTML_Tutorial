# Elemento select básico
Ahora veremos cómo funcionan los `select` que no son del tipo `input` si no que son un elemento mezcla entre los radio y los checkbox porque nos permiten trabajar con una o con varias opciones.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="lenguajes" id=""></select>
  </form>
</body>
~~~

<body>
  <form action="">
    <select name="lenguajes" id=""></select>
  </form>
</body>

Observamos que nos aparece una flecha para desplegar sin embargo aún no tenemos opciones dentro.

Debemos desplegar `select` y escribir las opciones que queremos aparezcan desplegadas; cada oción debe ir dentro de la etiqueta `<option value=""></option>` el `value` equivale a este valor.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="lenguajes" id="">
      <option value="html">HTML</option>
    </select>
  </form>
</body>
~~~
<body>
  <form action="">
    <select name="lenguajes" id="">
      <option value="html">HTML</option>
    </select>
  </form>
</body>

Como se puede ver ya aprarece la primera opción.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="lenguajes" id="">
      <option value="html">HTML</option>
      <option value="css">CSS</option>
      <option value="javascript">JavaScript</option>
    </select>
  </form>
</body>
~~~

<body>
  <form action="">
    <select name="lenguajes" id="">
      <option value="html">HTML</option>
      <option value="css">CSS</option>
      <option value="javascript">JavaScript</option>
    </select>
  </form>
</body>

Ahora tenemos un menú de opciones seleccionables y podremos seleccionar una.

Tanto en los `radio` como en los `chekbox` teníamos que poner el `name=""` en el `input` y el `value=""` al que correspondía, en este caso, el `name` lo tiene el elemento `<select></select>` y los `value` en el elemento `<option></option>`

Si queremos que se pudiera seleccionar más de uno tenemos el atributo `multiple`

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="lenguajes" multiple>
      <option value="html">HTML</option>
      <option value="css">CSS</option>
      <option value="javascript">JavaScript</option>
    </select>
  </form>
</body>
~~~
<body>
  <form action="">
    <select name="lenguajes" multiple>
      <option value="html">HTML</option>
      <option value="css">CSS</option>
      <option value="javascript">JavaScript</option>
    </select>
  </form>
</body>

De esta forma en lugar de tener un desplegable tendremos una lista que nospermite seleccionar uno, pero si pulsamos la tecla CTRL os permite seleccionar más de uno.

Esta es la forma de trabajar con un `<select></select>` de forma simple.

[Siguiente **&#129042;**](/markdown/031_Formularios_Select_Avanzados.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")
