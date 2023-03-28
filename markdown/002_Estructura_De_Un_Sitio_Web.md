# Estructura y comentarios

## **Estructura del documento HTML**

Todos los documentos HTML tienen una estructura requerida que incluye la siguiente declaración con elementos de apertura y cierre:

```html
<!DOCTYPE html>

<html></html>
<head> </head>
<body> </body>
```
La declaración de tipo de documento ``<!DOCTYPE html>`` informa a los navegadores web qué versión de HTML se está utilizando. Se coloca al principio del documento HTML. Después de la declaración de tipo de documento, el elemento ``<html>`` marca el comienzo del documento.

Dentro del elemento `<html>`, el elemento `<head>` identifica la parte superior del documento. Sin embargo, el contenido dentro del elemento `<head>` no se muestra en la propia página web. En su lugar, debe incluir el título del documento, que se muestra en la barra de título de la ventana del navegador, enlaces a cualquier archivo externo o cualquier otra información beneficiosa.

Todo el contenido visible dentro de la página web caerá dentro del elemento ``<body>``.

Teniendo Visual Studio Code abierto, podemos pulsar SHIFT + 1 para poner una admiración hacia abajo y si presionamos ENTER se nos creará la estructura base de HTML.

~~~html
<!DOCTYPE html>
<html lang="en">
  <head>
    
  </head>
  <body>
      
  </body>
</html>
~~~

De momento utilizaremos esta estructura básica.

## ``<!DOCTYPE html>``

    <!DOCTYPE html>

La declaración conocida `<!DOCTYPE html>` es la declaración de tipo de documento, informa al navegador sobre el **tipo de documento** para cargar una página correctamente con html5 no distingue entre mayúsculas.

Define que estándar de documento estamos siguiendo, esto representa que estamos utilizando el estándar de HTML5.

Sin embargo se debe aclarar que a pesar de esto se considera una mala práctica combinar formato entre minúsculas y mayúsculas, las etiquetas se deben tratar siempre con minúsculas  que como un arreglo escrita por el mismo lenguaje de es una buena forma de codificación.

La primera línea de cada documento web debe contener una declaración ``<!DOCTYPE html>`` y a pesar de que estaba envuelto en corchetes angulares es una declaración no una etiqueta.
<br>
<br>

## **Ahora veamos los elementos básicos de una estructura HTML** 

## ``<html lang="en">``
~~~html
<!-- Inicio del documento HTML -->
<html lang="en">
~~~
Esto significa que estamos estableciendo que el documento está en ingles.

Cambiar el `en` por `es` para volverlo al español.

## ``<head></head>``
El head representa una colección de metadatos del documento, estos datos le pasaremos al navegador para que interprete nuestra página web, esta no tendrá una representación visual pero el navegador lo entiende.

~~~html
<head>
    
</head>
~~~

## ``<title></title>``

La página debe tener un título, lo que aparece en el título de la pestaña en su navegador. El elemento `<title></title>` define el título de la página HTML y representaría lo que vemos en la pestaña cuando abrimos la página web.

~~~html
<!-- Datos que le pasamos al navegador con información de nuestra página web. -->
<head>
    <title>Mi primera página web</title>    
</head>
~~~

## ``<body></body>``

Esta **etiqueta** representa todo el contenido de nuestra web, esta parte si es visible y lo oque escribamos dentro si lo podremos ver en nuestro navegador

~~~html
<!-- Representa todo el contenido visible de nuestra página web -->
<body>
    
</body>
~~~

---
<br>
<br>
<br>

## *Comentario*

Los comentarios son utilizados para poder tener algo de información en nuestro código sin que se vea reflejado en nuestra página.

~~~html
<!--establece el tipo de estandar del documento HTML5-->
<!DOCTYPE html>
~~~

Tecla rápida CTRL + Ç

## *Codificación*

Los acentos pertenecen a una codificación Latina que por defecto los navegadores no le entienden salvo que se lo digamos explícitamente.

Para ello en el `<head></head>` donde le pasamos los datos importantes para el navegador colocaremos `<meta charset="">` que sería el conjunto de caracteres y el que necesitamos es UTF-8. Con esto le estamos indicando que estamos utilizando el set de caracteres Latino.

[Siguiente **&#129042;**](/markdown/003_T%C3%ADtulos_P%C3%A1rrafos.md "Resumen")

---
[*Volver* **&ldca;**](/markdown/README.md "Ir a Readme") [*Subir* **&#11165;**](# "Ir al título")