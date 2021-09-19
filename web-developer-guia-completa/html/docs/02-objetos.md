# HTML 02: Una pequeña introducción a "objetos".
Previo a que nosotros entremos en materia y empecemos a crear nuestra primer página html considero necesario entender un poco de teoría de los "objetos".

Probablemente si el lector no tiene una noción de qué es un objeto se pregunte, ¿A qué se refiere con "objetos"? Literalmente un objeto en definición textual de la [RAE](https://dle.rae.es/objeto):

> _Todo lo que puede ser materia de conocimiento o sensibilidad de parte del sujeto, incluso este mismo._

Esto quiere decir que todo lo que podamos observar o describir se puede tomar como un objeto, incluso el lector mismo. Si nosotros ejemplificamos a un objeto como un café, debemos pensar, cómo le explicaríamos a una persona que nunca ha bebido un café, qué es, o a nuestro hijo de 1 año, o a un extraterrestre. Sin complicarnos mucho la existencia, podemos decir que denominamos "café" a una bebida que se obtiene a partir de los granos de una planta llamada "Cafeto" y se puede preparar de múltiples formas, así que podríamos decir que casi ningún café es igual.

Entonces, ¿Cómo podría saber que tipo de café estoy tomando? Si nosotros partiéramos que nuestro café es nuestro objeto a describir, nuestro objeto `café` tiene ciertas propiedades que lo hacen diferentes a otros objetos `café`, algunas propiedades como el `origen` que quiere decir, de qué país provienen los granos, el `tipo` de grano, la `acidez` que contiene, el grado de `tueste` que tiene el grano, entre otras características.

Aterrizando un poco nuestro ejemplo del objeto `café`, los objetos en HTML reciben el nombre de etiqueta, si hiciéramos nuestro objeto `café` en HTML podríamos hacer lo siguiente:

```html
<cafe>Agua</cafe>
```

La forma de declarar nuestro objeto en HTML es con picoparéntesis o símbolos de "menor qué" y "mayor qué" `<` `>`, la etiqueta consiste en una "apertura" y un "cierre", la apertura es cuando le indicamos al navegador dónde iniciará nuestra etiqueta y el cierre dónde termina, lo que existe enmedio de la apertura y el cierre es el "contenido" de nuestra etiqueta, en este caso, lo único que contiene nuestro café es Agua y ese texto "Agua" será procesado para ser nuestro café.

La apertura consiste en el nombre de nuestro objeto rodeado de nuestro picoparéntesis, si habláramos de un párrafo, éste es la etiqueta con apertura `<p>`.

El cierre consiste en __casi exactamente la misma apertura__, con la diferencia de tener con prefijo al nombre del objeto una "diagonal" o "barra" `/`, para el caso del párrafo, sería `</p>`.

El contenido de la etiqueta será lo que nuestro navegador reconocerá y formateará como el objeto. En el caso del párrafo, el objeto es un párrafo, sin embargo, el contenido de éste iría dentro de la apertura y el cierre, por ejemplo: `<p>Este es un párrafo</p>`. El navegador mostrará únicamente el texto `Este es un párrafo`, pero formateado como párrafo.

Regresando a nuestro ejemplo del café y sus propiedades, podríamos escribir nuestro café de la siguiente forma:

```html
<cafe origen="Mexico" tipo-de-grano="Bourbón" acidez="alta" tueste="natural">Agua</cafe>
```

Aquí no solamente es un café cualquiera, estoy diciendo que mi café es diferente al resto, agregándole sus propiedades que mencionamos anteriormente y esta es la forma en la que podemos agregar propiedades a nuestras etiquetas en HTML, el nombre de la propiedad usualmente se escribe en minúsculas y separados por guiones (Kebab case). El "valor" de nuestra propiedad se coloca inmediatamente después de la propiedad con un igual `=` y entre comillas dobles `"` quedando como resultado `origen="Mexico"`. Las propiedades __siempre__ van en la apertura de nuestra etiqueta separadas con un espacio.

Para el navegador no sabe que quiere decir la etiqueta `<cafe>`, únicamente se usó como ejemplo para comprender la estructura de una etiqueta, pero hay técnicas avanzadas para hacer que sí lo reconozca y haga algo similar al párrafo, pero esa será una conversación para el futuro. Para efectos de nuestro tutorial, debemos conocer que HTML ya tiene definidos un listado de diversas etiquetas con sus propiedades opcionales que tienen un efecto en lo que envuelven.
