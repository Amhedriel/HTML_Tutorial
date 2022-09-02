# Atributos

En esta sección veremos los atributos en HTML.

Son valores adicionales que configuran los elemntos y/o ajustan su comportamiento.

En términos generales hay dos tipos de atributos

* Comunes:
  
  Su sintaxis es -> `atributo="valor"`

* Booleanos:

  Su sintaxis es -> `atributo`

  Esto sucede porque en html hay ciertos atributos, que si existen se dan como verdaderos y si no existen se dan como falsos, por lo tanto no necesitan que se les asigne un valor, si existe funciona y si no existe no funciona.
---

## Atributos ya utilizados

Observemos:
~~~html
  <html lang="es">

  </html>
~~~

Los atributos son valores adicionales que configuran los elemntos y/o ajustan su comportamiento.

En este caso lo que estamos haciendo es configurar el documento HTML diciendole que su idioma es en español = es, en inglés = en, en alemán = de, etc...

En `head` tenemos el `meta charset`

~~~html
<head>
  <meta charset="UTF-8">

</head>
~~~

Aqui tenemos una **etiqueta** `meta` y como configuración tenemos `charset` que es un **atributo** que declara la codificación de carateres de la página, en este caso es `"UTF-8"` que sería el **valor**.

