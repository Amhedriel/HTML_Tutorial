# Móviles

Ahora veremos algunos tipos de input que existen:

* search -> Se utiliza para las barras de búsqueda.
* tel -> Se utiliza para introducir números telefónicos.
* email -> Se utiliza para introducir un email.
* password -> Se utiliza para contraseñas
* url -> Se utiliza para introducir URLs.

Estos `inputs` son bastante importantes, lo que pasa es que estos mismos `inputs` en un móvil se ven de manera distinta.

Ahora crearemos los `input` de este tipo teniendo una vista previa del móvil de lo que estamos haciendo aquí y veremos el cambio del teclado dependiendo del campo que estemos utilizando.

~~~html
<body>
  <form>
    <!-- Utilizaremos label para tenerlos identificados y saber a que corresponde cada cosa -->
    <label> search
      <input type="search">
    </label>
    <label> teléfono
      <input type="tel">
    </label>
    <label> email
      <input type="email">
    </label>
    <label> password
      <input type="password">
    </label>
    <label> url
      <input type="url">
    </label>
  </form>
</body>
~~~

<body>
  <form>
    <!-- Utilizaremos label para tenerlos identificados y saber a que corresponde cada cosa -->
  <div>
    <label> search
      <input type="search">
    </label>
  </div>
  <div>
    <label> teléfono
      <input type="tel">
    </label>
  </div>
  <div>
    <label> email
      <input type="email">
    </label>
  </div>
  <div>
    <label> password
      <input type="password">
    </label>
  </div>
  <div>
    <label> url
      <input type="url">
    </label>
  </div>  
  </form>
</body>

---
* password: La diferencia en móviles con password es que al escribir en ese espacio no muestra lo que estamos escribiendo, lo que muestra es texto oculto. Pero este modo de "oculto" no es seguro para nada, solo esconde el texto para quien lo mira sin inspeccionar la página.

Ahora describiremos las diferencias en un móvil.

1. search   : Aparecerá el teclado qwerty con un botón de búsqueda agregado.
2. tel      : Aparecerá el teclado numérico para facilitarel manejo del teléfono.
3. email    : Teclado qwerty con botón agregado de arroba @.
4. password : Qwerty normal con numérico en la parte de arriba y una llave que sugiere contraseñas seguras y administrar contraseñas.
5. url      : Qwerty normal pero en el historial de búsquedas nos sugerirá urls.

Por temas de accesibilidad es muy importante colcar el campo correspondiente para lo que necesitamos, debido a que el movil ayuda al usuario en base a la información que debe insertar.








