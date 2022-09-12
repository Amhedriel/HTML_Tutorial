# Listas Anidadas

Debemos saber que se pueden construir listas anidadas metiendo en uno de los `li` otro `ul` o un `ol` según sea necesario:

~~~html
<body>
  <h1>Combinando rutas de estudio para frontend</h1>
  <ol>
    <li>
      HTML
      <ul>
        <li>Estrucutura</li>
        <li>Sintaxis</li>
        <li>Etiquetas</li>
      </ul>
    </li>
    <li>CSS</li>
    <li>JavaScript</li>
  </ol>
</body>
~~~

Esta lista se ve en pantalla de la siguiente forma:

![Listas_anidadas](/media/Listas_Anidadas.png "Lista de ruta de estudio para frontend")

---

## Atributos de las listas

<pre>
* <b>ul</b> 
    type: Estilo de los items (disc, square, circle)
    
* <b>ol</b>
    type: Estilo de numeraación (1, A, a, I, i)
    start: Inicio de la secuencia (un número)
</pre>

En los `ul` solo tenemos un tipo ``(type)`` de lista

~~~html
  <h2>Atributos en las Listas</h2>
  <ul type="square">
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
  </ul>
~~~
Cambiará los puntos por cuadrados:

![square](/media/Listas_square.png "Lista desordenada con cuadrados en lugar de puntos")

Sin embargo esto lo haremos preferiblemente con CSS, ya da más opciones de cambio a las formas y es buena práctica.

Con `ol` tenemos algo más de opciones:

~~~html
  <h2>Atributos listas ordenadas "type"</h2>
  <ol type="I">
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
  </ol>
~~~

Con la opción de ``I`` le estamos indicando que queremos un orden a base de números romanos en mayúsculas.

![Numeros_romanos_mayúsculas](/media/Listas_romanos.png "Lista ordenada mediante números romanos")

Y las opciones son distintas con cada uno de los indicados ``A, a`` son ordenados por el abecedario con letras en Mayúsculas o minúsculas; ``I, i`` Números romanos igualmente con mayúsculas o minúsculas y por números ``1``.

Si añadimos el atributo de `start` agregaremos la opción de en que número o letra queremos que inicie el conteo para las listas.

~~~html
  <h2>Atributos listas ordenadas "type" y "start"</h2>
  <ol type="a" start="3">
    <li>Item</li>
    <li>Item</li>
    <li>Item</li>
  </ol>
~~~

Estamos indicando que la lista empiece por la tercera letra del abecedario, en este caso la c en minúsculas.

![Letras_ordenadas_c](/media/Listas_abecedario_desde_c.png "lista con letras ordenadas desde la c")



