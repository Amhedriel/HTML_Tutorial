# Etiquetas importantes de línea

Revisaremos etiquetas en línea muy utilizadas en las páginas web actuales.

## span
Es un contenedor de línea, equivalente a `div`, se suele usar para ecerrar palabras o pequeños textos y darles estilo a través de CSS o localizarlos desde JavaScript. Semánticamente no significa nada.

~~~html
  <style>
    span {
      color: red;
    }
  </style>


</head>
<body>
  <p>Lorem ipsum dolor sit amet <span> consectetur adipisicing </span> elit. Illum rem eius eos dolorum dicta blanditiis accusantium impedit doloribus, molestias id, perspiciatis recusandae. Reprehenderit eaque, fugit ad velit perspiciatis quis dicta delectus quasi laborum culpa cupiditate quaerat fuga iure libero praesentium! Sapiente, aspernatur dicta libero quod quos illum eveniet nihil ad debitis dolore quibusdam et sunt eum explicabo ea officia quia exercitationem porro! Magni doloribus excepturi nostrum! Enim voluptas recusandae aliquid?</p>
</body>
~~~

Con este código de `style` coloreamos las palabras que estna encerradas en la etiqueta span.

La etiqueta `span` sirve para eso localizarlo desde JavaScript o para darle estilos desde CSS, a una palabra en concreto o que tenga que tener un estilo en particular o a un grupo de palabras.

## q
Es el equivalente de `blockquote`, significa *quote*, por eso el de bloque se llama *block - quote*. Sirve para poner citas pero en línea.

~~~html
<body>
  <q cite="">Yo soy Batman</q>
</body>
~~~

Es lo mismo que `blockquote` pero en línea, en este ejemplo coloca "Yo soy Batman".

## code
Sirve para encerrar código que queremos representar visualmente, suele ir unido con la etiqueta `pre`.

~~~html
  <pre>
    <code>
      span {
        color: red;
      }
    </code>
  </pre>
~~~
con este ejemplo vemos que será representado visualmente tal como esta escrito y con formato de código, con esto decimos al navegador que esto es código, lo usaremos cuando queremos representar código que queremos que se represente visualmente.

## Código ASCII
Son entidades especiales en HTML - Código ASCII

Si nosotros queremos representar código como por ejemplo:

~~~html
  <p>La etiqueta <code><h1></code> se utiliza para representar títulos de primer nivel</p>
~~~

El `h1` convertirá lo que le sigue automáticamente en un título y eso no es lo que queremos, entonces nos ayudaremos del código ASCII, haciendo que la representación visual de mayor y menor sin que se convierta en una etiqueta HTML, para ello tenemos la tabla de [código_ASCII](https://ascii.cl/es/codigos-html.htm)

~~~html
  <p>La etiqueta <code>&#60;h1&#62;</code> se utiliza para representar títulos de primer nivel</p>
~~~

Con esos códigos ASCII ahora podemos representar los símbolos de mayor y menor, ahora veremos la representación de Copyrigth de derechos reservados:

\&copy;
&copy;

Y en Visual Studio podemos escribir el andpersan (&) y presionamos CTRL + SPACE nos enseñará una lista larguísima de todos los símbolos que se pueden escribir.

