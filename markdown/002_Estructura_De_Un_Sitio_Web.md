# Estrucutura y comentarios

## Estructura

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

### \<!DOCTYPE html>

    <!DOCTYPE html>

Define que estandar de documento estamos siguiendo, esto representa que estamos utilizando el estandar de HTML5

### \<html lang="en">
~~~html
<!-- Inicio del documeto HTML -->
<html lang="en">
~~~
Esto significa que estamos estableciendo que el documento está en ingles.

Cambiar el `en` por `es` para volverlo al español.

## \<head> \</head>
El head representa una colección de metadatos del documento, estos datos le pasaremos al navegador para que interprete nuestra página web, esta no tendrá una representación visual pero el navegador lo entiende.

~~~html
<head>
    
</head>
~~~

## \<title> \</title>

`<title></title>` representaría lo que vemos en la pestaña cuando abrimos la página web.

~~~html
<!-- Datos que le pasamos al navegador con información de nuestra página web. -->
<head>
    <title>Document</title>    
</head>
~~~

## \<body> \</body>

Esta **etiqueta** representa todo el contenido de nuestra web, esta parte si es visible y lo oque escribamos dentro si lo podremos ver en nuestro navegador

~~~html
<!-- Representa todo el contenido visible de nuestra página web -->
<body>
    
</body>
~~~

## Comentario

Los comentarios son utilizados para poder tener algo de información en nuestro código sin que se vea reflejado en nuestra página.

~~~html
<!--establece el tipo de estandar del documento HTML5-->
<!DOCTYPE html>
~~~

Tecla rápida CTRL + Ç

