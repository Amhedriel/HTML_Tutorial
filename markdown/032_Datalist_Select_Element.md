# Datalist

Otro elemento seccionable, `datalist` son muy similares a los `select` pero incluyen un filtro para poder buscar de una forma más sencilla.

Crearemos un `input type="list"` que nos permitrá hacer el filtro, ahora debemos darle una lista de la cual debemos utilizar `list="pets"`.

Ahora debemos crear nuestra ``datalist``, que será la lista que utilizaremos para trabajar, en este caso "pets", como este `datalist` es la "lista" necesitamos un `id` que se corresponda con la lista que escribimos en `list="pets"` por lo tanto será `id="pets"`.

Luego, lo que funciona por dentro es exactamente igual que un `select`.

~~~html
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <input type="list" list="pets">
    <datalist id="pets">
      <option value="perro">Perro</option>
      <option value="gato">Gato</option>
      <option value="hamster">Hamster</option>
      <option value="conejo">Conejo</option>
      <option value="loro">Loro</option>
      <option value="canario">Canario</option>
      <option value="serpiente">Serpiente</option>
      <option value="tarantula">Tarántula</option>
    </datalist>

  </form>
  
</body>
~~~
<body>
  <h1>Elementos seleccionables</h1>
  <form action="">
    <input type="list" list="pets">
    <datalist id="pets">
      <option value="perro">Perro</option>
      <option value="gato">Gato</option>
      <option value="hamster">Hamster</option>
      <option value="conejo">Conejo</option>
      <option value="loro">Loro</option>
      <option value="canario">Canario</option>
      <option value="serpiente">Serpiente</option>
      <option value="tarantula">Tarántula</option>
    </datalist>

  </form>
  
</body>

Podemos observar que cuando colocamos el puntero sopbre el recuadro tendremos la opción múltiple representada con una flecha y nos salen los 2 valores `value="perro">Perro<`, si nosotros en `value` cambiamos, entonces al desplegar la primera opción que sale es el `value` y por debajo sale un peuqeña descripción si la necesitáramos.

Bien podríamos no tener nada escrito fuera del `value` y utilizarlo para hacer algo así como una descripción `value="perro">En este caso un labrador<`.

La parte más significativa de utilizar un `datalist` en lugar de un `select` es el recuadro de filtro que tenemos al pincharlo, recordemos que no usca por el inicio alfabético de la palabra, lo que hace es mostrarnos todos los resultados que contengan dichas letras.

## Conclusión

Asi que en los casos que queramos hacer un `select` con un filtro y que al usuario le resulte más cómodo encontrarlos esta es un opción muy buena.





[Siguiente **&#129042;**](/markdown/Recursos.md "")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")