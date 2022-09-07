## Rutas absolutas

Suelen tener un protocolo HTTP o HTTPS y són unicas en la red, se suelen utilizar para rutas externas.

~~~html
<a href="http://google.com">Ir a Google</a>
~~~

Esto es lo que se considera una ruta absoluta, tenemos que salir de nuestro proyecto para buscar dicha dirección.

---

## Rutas relativas

Tenemos 2 tipos de rutas relativas:

* Relativas al punto donde nos encontramos.

* Relativas a la raíz del proyecto.

~~~html
<body>
 <h1>HOME</h1>
  <a href="contacto.html">Ir a contacto</a>
</body>
~~~
Esto es una ruta relativa al punto donde nos encontramos, si nosotros estuvieramos ne el ``index.html`` y colocaramos esto mismo de `contacto.html` el buscaria dentro de nuestra carpeta, dentro de nuestros archivos, entonces daría un error porque no lo encuentra.

Si nosotros queremos enlazar otro documento HTML que no se encuentre en la misma carpeta debemos escribir la dirección en donde se encuentra.

~~~html
<body>
 <h1>HOME</h1>
  <a href="paginas/contacto.html">Ir a contacto</a>
</body>
~~~

Debemos tener presente que tanto para entrar como para salir de los documentos HTML mediante las rutas relativas tenemos que indicar la ruta correcta, en caso de que un Documento esté una carpeta antes debemos colocar `../` en los documentos que no estén ubicados en dicha carpeta para que puedan retroceder y encontrar el documento desdeado.

~~~html
<body>
 <h1>HOME</h1>
  <a href="../index.html">Ir a inicio</a>
</body>
~~~

En este caso nosotros queremos volver de la página de contacto.html que esta en la carpeta de `paginas`a index.html.

### **Ruta relativa a la Raíz**

Para estabecer una ruta relativa a la raíz lo que tenemos que hacer es empezar la ruta con una barra `href="/"` con esto le estamos diciendo que e vaya al punto más alto que se pueda y que desde ahí empiece a contar.

~~~html
<body>
 <h1>HOME</h1>
  <a href="/index.html">Ir a inicio</a>
</body>
~~~

En este ejemplo podríamos volver al documento de `index.html` desde cualquier otro documento ubicado en cualquier de nuestro proyecto actua

Si en la ruta solo pusieramos la barra inclinada `"/"` entonces volveríamos a `index.html` sin la necesidad de especificar esto es asi porque, es el archivo que por defecto intentarán cargar todos los navegadores.

