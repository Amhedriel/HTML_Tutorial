# Elemento select avanzado

Veremos distintos tipos de mascotas y quremos usar una etiqueta para englobarlas y que al usuario le sea más fácil elegir.

Para ello si tenemos mucgas opciones podemos ordenarlas por catogorías a través de la etiqueta `<optgroup></optgroup>` que es (option group) y básicamente sirve para agrupar opciones y con `label` nombraríamos la categoría.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="mascotas" id="">
      <option value="perro">Perro</option>
      <option value="gato">Gato</option>
      <option value="hamster">Hamster</option>
      <option value="conejo">Conejo</option>
      <option value="loro">Loro</option>
      <option value="canario">Canario</option>
      <option value="serpiente">Serpiente</option>
      <option value="tarantula">Tarántula</option>
    </select>
  </form>
</body>
~~~

Este sería un select normal pero agregando `optgroup` tenemos.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="mascotas" id="">
      <optgroup label="4 patas">
        <option value="perro">Perro</option>
        <option value="gato">Gato</option>
        <option value="hamster">Hamster</option>
        <option value="conejo">Conejo</option>
      </optgroup>
      <option value="loro">Loro</option>
      <option value="canario">Canario</option>
      <option value="serpiente">Serpiente</option>
      <option value="tarantula">Tarántula</option>
    </select>
  </form>
</body>
</html>
~~~

<body>
  <h2>Elementos seleccionables</h2>
  <form action="">
    <select name="mascotas" id="">
      <optgroup label="4 patas">
        <option value="perro">Perro</option>
        <option value="gato">Gato</option>
        <option value="hamster">Hamster</option>
        <option value="conejo">Conejo</option>
      </optgroup>
      <option value="loro">Loro</option>
      <option value="canario">Canario</option>
      <option value="serpiente">Serpiente</option>
      <option value="tarantula">Tarántula</option>
    </select>
  </form>
</body>
</html>

Veremos que al desplegar tendremos categorías.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <select name="mascotas" id="">
      <optgroup label="4 patas">
        <option value="perro">Perro</option>
        <option value="gato">Gato</option>
        <option value="hamster">Hamster</option>
        <option value="conejo">Conejo</option>
      </optgroup>
      <optgroup label="aves">
        <option value="loro">Loro</option>
        <option value="canario">Canario</option>
      </optgroup>
      <optgroup label="otras">
        <option value="serpiente">Serpiente</option>
        <option value="tarantula">Tarántula</option>
      </optgroup>
    </select>
  </form>
</body>
</html>
~~~

<body>
  <h2>Elementos seleccionables</h2>
  <form action="">
    <select name="mascotas" id="">
      <optgroup label="4 patas">
        <option value="perro">Perro</option>
        <option value="gato">Gato</option>
        <option value="hamster">Hamster</option>
        <option value="conejo">Conejo</option>
      </optgroup>
      <optgroup label="aves">
        <option value="loro">Loro</option>
        <option value="canario">Canario</option>
      </optgroup>
      <optgroup label="otras">
        <option value="serpiente">Serpiente</option>
        <option value="tarantula">Tarántula</option>
      </optgroup>
    </select>
  </form>
</body>
</html>

Ahora cada elemento está en su respectivo grupo.

[Siguiente **&#129042;**](/markdown/032_Datalist_Select_Element.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")