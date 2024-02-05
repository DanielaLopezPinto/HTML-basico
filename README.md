
# HTML Básico

Guia de Html básico

La estructura del Html basico es la siguiente:
 
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
    </body>
    </html>


# Anidamiento

 <main></main>

Esto se llama anidamiento. Los elementos anidados deben colocarse dos espacios más a la derecha del elemento en el que están anidados. Este espacio se llama sangría (indentación en programación) y se utiliza para facilitar la lectura de HTML.


# Atributos 

Los atributos HTML son palabras especiales usadas dentro de la etiqueta de apertura de un elemento para controlar el comportamiento del elemento. 


**src**

El atributo src en un elemento img especifica la URL (donde se localiza la imagen).


**alt**

Todos los elementos img deben tener un atributo alt. El texto del atributo alt es utilizado por lectores de pantalla para mejora la accesibilidad y es mostrado en caso de que la imagen falle en cargar.


**target**

un atributo target con el valor _blank en la etiqueta de apertura <a> hace que el enlace abra en una nueva pestaña.


**id**

El atributo id se utiliza para identificar elementos HTML específicos. Cada atributo id debe tener un valor único, diferente a los demás valores id de la página.


**name**

Para hacer que al seleccionar un radio button, el otro sé deseleccione automáticamente, ambos botones deben tener un atributo name con el mismo valor.
Por ejemplo:

    <label><input id="indoor" type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input id="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>


**value**

El atributo value es usado para definr el valor enviado por el checkbox. El atributo checked se usa para indicar que el elemento está seleccionado.







# Elementos 

**<h#></h#>**

Los elementos de encabezado h1 a h6 se utilizan para indicar la importancia del contenido por debajo de ellos. Entre menor sea el número, el contenido será más importante.


**<a></a>**

Por ejemplo:

    <a href="https://www.freecodecamp.org">click here to go to freeCodeCamp</a> 

es un enlace con el texto "click here to go to freeCodeCamp".

Se puede meter un enlace dentro de una oración, parrafo, frase, etc.

Por ejemplo:

    <p>See more <a href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>

Esto hace que en cat photos quede el enlace.



**<section></section>**

representa una sección genérica de un documento. Sirve para determinar qué contenido corresponde a qué parte de un esquema. Piensa en el esquema como en el índice de contenido de un libro; un tema común y subsecciones relacionadas.


**<figure></figure>**

El elemento figure representa contenido independiente y te permitirá asociar una imagen a una descripción.



**<figcaption></figcaption>**

Un elemento (figcaption), se utiliza para añadir una descripción o leyenda para describir una imagen anidada en un elemento figure. Por ejemplo,

    <figcaption>A cute cat</figcaption> 
añade la descripción "A cute cat".



**<em></em>**

Enfatiza la palabra envolviendola en un elemento énfasis em.



**<strong></strong>**

El elemento strong se utiliza para indicar que una parte de un texto es importante o urgente.


**<button></button>**

Utiliza el elemento button para crear un botón cliqueable. Por ejemplo, 

    <button>Click Here</button> 

crea un botón con el texto Click Here


**<fieldset></fieldset>**

El elemento fieldset se utiliza para agrupar elementos input y label relacionados dentro de un formulario web. Los elementos fieldset son elementos de nivel de bloque, lo que significa que aparecen en una nueva línea.

**<legend></legend>**

El elemento legend actúa como una leyenda/descripción, para el contenido del elemento fieldset. Le da a los usuarios un contexto sobre lo que deben ingresar en esa parte del formulario.





# Listas

**<ul></ul>**

ul de "unordered list" -lista no ordenada . crea una lista no ordenada.

**<li></li>**

Utiliza la etiqueta (li - list item) para agregar elementos a una lista. Aquí  hay un ejemplo de una lista de objetos en una lista desordenada:

    <ul>
    <li>milk</li>
    <li>cheese</li>
    </ul>

Dentro del elemento ul anida tres elementos li para mostrar tres cosas que aman los gatos:

**<ol></ol>**

El elemento ol permite definir listas o viñetas ordenadas ("Ordered List"), bien con numeración o alfabéticamente.




# Etiquetas de autocierre (self-closing tag)

**<img>**

Los elementos img tienen una etiqueta de apertura sin una etiqueta de cierre. La etiqueta de un elemento que no necesita etiqueta de cierre se conoce como etiqueta de autocierre (self-closing tag).

Podemos crear una imagen con un link agregando la etiqueta <a> antes y poniendo el atributo href con el link que se desea colocar.


**meta** (dentro de <head>)

Puede configurar el comportamiento del navegador agregando elementos meta de cierre automático en el head. Aquí hay un ejemplo:

    <meta attribute="value">
Indique al navegador que analice el marcado en varios idiomas creando un elemento meta como hijo del elemento head. Establece su atributo charset en UTF-8.




# Formularios

    <form></form>

Con este elemento form añadiras un formulario web para recolectar información de los usuarios.

**action**

El atributo action indica, dónde deben enviarse los datos del formulario. Por ejemplo, 

    <form action="/submit-url"></form> 

le dice al navegador que los datos del formulario deben ser enviados a la ruta /submit-url


**input**

El elemento input te permite recolectar datos desde un formulario web de diferentes formas. Los elementos input son de auto-cierre y no necesitan etiquetas de cierre.

**Type**

*Type text:* Este tipo de input toma un valor de "texto", por lo que crea una sola línea de entrada de texto.

    <input type="text" placeholder="Introduce nombre" />


*Type Password:* Como su nombre lo indica, una entrada con un tipo de contraseña crea una contraseña. Es automáticamente invisible para el usuario, a menos que sea manipulado por JavaScript.

    <input type="password" placeholder="Enter your password" />


*Type Email:* Cualquier entrada con el tipo de correo electrónico define un campo para ingresar una dirección de correo electrónico.

    <input type="email" placeholder="Enter your email" />


*Type Number:* Este tipo de entrada permite al usuario insertar solo números.

    <input type="number" placeholder="Enter a number" />


*Type Radio:* A veces, los usuarios tendrán que elegir una de las numerosas opciones. Un campo de entrada con sus atributos de tipo establecidos en "radio" le permite hacer esto.

    <input type="radio" />

*Type Checkbox:* Por lo tanto, con un tipo de entrada de radio, los usuarios podrán elegir una de numerosas opciones. ¿Qué pasa si quieres que elijan tantas opciones como sea posible? Eso es lo que una entrada con un atributo de tipo establecido en checkbox hace.

    <input type="checkbox" />


*Type Submit:* Utilice este tipo para agregar un botón de envío a los formularios. Cuando un usuario hace clic en él, envía automáticamente el formulario. Toma un atributo de valor, que define el texto que aparece dentro del botón.

    <input type="submit" value="Enter to Win" />


*Type Button:* Una entrada con un tipo establecido en button crea un botón, que puede ser manipulado por el tipo de detector de eventos onClick de JavaScript. Crea un botón como un tipo de entrada de envío, pero con la excepción de que el valor está vacío de forma predeterminada, por lo que debe especificarse.

    <input type="button" value="Submit" />


*Type File:* Esto define un campo para el envío de archivos. Cuando un usuario hace clic en él, se le solicita que inserte el tipo de archivo deseado, que puede ser una imagen, un PDF, un archivo de documento, etc.

    <input type="file" />


*Type Color:* Este es un tipo de entrada elegante introducido por HTML5. Con él, el usuario puede enviar su color favorito, por ejemplo. El negro (#000000) es el valor predeterminado, pero se puede anular configurando el valor en el color deseado.

    <input type="color" />


*Type Search:* La entrada con el tipo de búsqueda define un campo de texto como un tipo de entrada de texto. Pero esta vez tiene el único propósito de buscar información. Se diferencia de escribir texto en que aparece un botón de cancelar una vez que el usuario comienza a escribir.

    <input type="search" />


*Type URL:* Cuando el atributo de tipo de una etiqueta de entrada se establece en URL, muestra un campo donde los usuarios pueden ingresar una URL.

    <input type="url" />


*Type Tel:* Un tipo de entrada de tel le permite recopilar números de teléfono de los usuarios.

    <input type="tel" />


*Type Date:* Es posible que se haya registrado en un sitio web donde solicitó la fecha de un evento determinado. La web probablemente usó una entrada con el valor de tipo establecido "date" para lograr esto.

    <input type="date" />


*Type Datetime-local:* Esto funciona como el tipo de entrada fecha, pero también le permite al usuario elegir una fecha con una hora en particular.

    <input type="datetime-local" />


*Type Week:* El tipo de entrada de semana permite al usuario seleccionar una semana específica.

    <input type="week" />


*Type Month:* La entrada con el tipo de mes completa los meses para que el usuario elija cuando se hace clic.

    <input type="month" />


*Textarea:* Hay ocasiones en las que un usuario necesitará completar varias líneas de texto que no serían adecuadas en un tipo de entrada de texto(ya que especifica un campo de texto de una línea).

textarea permite al usuario hacer esto porque define múltiples líneas de entrada de texto. Toma sus propios atributos, tales como cols – para el número de columnas, y rows para el número de filas.

    <textarea cols="50" rows="20"></textarea>


*Multiple Select Box:* Esto es como un botón de radio y una casilla de verificación en un solo paquete. Está incrustado en la página con dos elementos: un elemento select y option, que siempre está anidado dentro de select.

De forma predeterminada, el usuario solo puede elegir una de las opciones. Pero con múltiples atributos, puede permitir que el usuario seleccione más de una de las opciones.

    <select>
        <option value="HTML">Select a Language</option>
        <option value="HTML">HTML</option>
        <option value="CSS">CSS</option>
        <option value="JavaScript">JavaScript</option>
        <option value="React">React</option>
    </select>


*Cómo etiquetar entradas HTML:*
Es importante asignar etiquetas a los controles de formulario. Cuando están correctamente conectados al campo de entrada a través de su atributo for y el atributo id, es más fácil de usar para el usuario, ya que simplemente puede hacer clic en la etiqueta para acceder a la entrada.

    <label for="name">Name</label>
    <input type="text" id="name" /> <br />
    <label for="check">Agree with terms</label>
    <input type="checkbox" id="check" />


**name**

Para que los datos de un formulario puedan acceder al destino especificado en el atributo action, debes darle al campo de texto un atributo name y darle un valor que represente a los datos que están siendo enviados. Por ejemplo, puede utilizar la siguiente sintaxis para un campo de texto de dirección de correo electrónico:

    <input type="text" name="email">.


**placeholder**

Un texto provisional (placeholder) nos da una idea de que tipo de información debemos escribir en un elemento input. Por ejemplo, 

    <input type="text" placeholder="Email address">


**required**

Para evitar que un usuario entregue su formulario incompleto, necesitas añadir el atributo *required* al elemento *input*. El atributo *required* no necesita ningún valor. Simplemente necesitas añadir la palabra *required* al elemento *input*, asegurándote de que hay espacios entre ella y los otros atributos.

**label**

Los elementos label se utilizan para ayudar a asociar el texto a un elemento input con el propio elemento input (especialmente para las tecnologías de asistencia como los lectores de pantalla). Por ejemplo, 

    <label><input type="radio"> cat</label> 

hace que al hacer click en la palabra cat se seleccione el radio button correspondiente.

*for*

El atributo *for* te permite vincular la etiqueta directamente al campo de entrada.
   
    <input id="loving" type="checkbox"> <label for="loving"> Loving</label>
