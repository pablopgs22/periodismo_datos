# EXAMEN 19-01-2022

### 4. Qué medio de comunicación inglés es fundamental en el periodismo y la visualización de datos?

The Guardian es un diario referente en el mundo del periodismo de datos, en especial desd que cuentan con el equipo Datablog, constituido por Simon Rogers y Paul Bradshaw.
El Data Blog de The Guardian es la biblia del periodismo de datos.

### 5. Qué lenguajes informáticos conoces. Razona la respuesta.

Entendemos por lenguaje informático aquel lenguaje que entiende o puede entender el ordenador, a través de software. Por un lado, están los lenguajes estructurados, como puede ser HTML, cuya función es estructurar documentos. Están también los lenguajes de programación, los cuales sirven para programar acciones en el ordenador. Algunos ejemplos de lenguajes de programación son: Java, Python o Javascript. Este último es muy usado en la web, por el hecho de que aporta interactividad.

### 7. ¿Qué fue determinante para el nacimiento del periodismo de datos moderno?

El periodismo de datos moderno o actual nace entre 2006 y 2008 debido a una confluencia de factores: abundancia de software de código abierto, HTML5 y Open Data.

### 14. ¿Qué relación tiene el formato CSV con Excel?

Microsoft Excel es un programa informático gráfico que sirve para visualizar datos tabulados y trabajar con ellos. CSV (comma-separated values) es un formato de datos; también  están, por ejemplo, los TSV (tab-separated values). La relación está en que Excel puede abrir y operar con archivos que estén en formato csv, aunque no es el único software que puede hacerlo. De hecho, para trabajar con archivos csv, nosotros hemos usado Open Refine, el cual, a diferencia de Excel, es un software de código abierto.

### 25. Si quisieras ver la web theguardian.com, ¿cómo lo harías desde la línea de comandos?

Para ver la web de The Guardian desde la terminal, habría que usar Lynx, un navegador en línea de comandos. Sería tan fácil como ejecutar el comando lynx con https://theguardian.com como argumento. 

### 26. ¿Cómo te descargarías la web theguardian.com desde la línea de comandos?

Para descargar la web theguardian.com desde la línea de comandos, usaríamos de nuevo lynx, pero con la opción "source". Quedaría así: `lynx -source theguardian.com`

### 27. ¿Cuál es la versión de Shell qué utilizas?

GNU bash, version 3.2.57(1)-release (x86_64-apple-darwin18)

(Esto es lo que sale al introducir en la terminal lo siguiente, para consultar la versión de la shell: 
`bash --version`)

### 29. Cuál es el primer comando que deberías usar en la terminal. Explica tu respuesta.

Antes de empezar a trabajar con la terminal, hay que saber dónde estoy, para lo que debe usarse el comando `pwd` (print working directory). Dicho comando me devuelve mi ubicación en el sistema de ficheros de mi ordenador.

### 30. ¿Como te mueves por el árbol de directorios de tu sistema de ficheros? Razona tu respuesta.

Para moverme por el árbol de directorios de mis sistema de ficheros, es útil comprobar primero cómo está este organizado. Para ello, puede usarse el comando `tree`. Sin embargo, si lo que quiero es navegar y moverme de un directorio a otro, usaré el comando `cd` (change directory), al que añadiré la ruta del fichero al que quiero moverme. Para volver al directorio padre, usaré `cd ..`

### 31. Si quisieras clonar un repositorio git, ¿qué pasos tendrías que dar? ¿Cómo comprobarías que ha funcionado?

Para clonar un repositorio git, lo primero que hay que hacer es ir a Github y copiar la dirección del repositorio. Por ejemplo: `https://github.com/flowsta/uc3m-periodismo-datos.git` (Es importante que al final de la dirección ponga ".git")
Después, desde la terminal, ejecutamos el comando `git clone` y añadimos la dirección anterior como argumento: `git clone https://github.com/flowsta/uc3m-periodismo-datos.git`
Esto creará en el directorio en el que estamos un directorio clon del repositorio remoto. Si quisiéramos, podríamos ponerle otro nombre (por defecto, se pone el nombre del repositorio remoto), aladiéndolo al final de la línea: `git clone https://github.com/flowsta/uc3m-periodismo-datos.git nuevo_repositorio` Nuestro directorio, en este caso, se llamaría "nuevo_repositorio".
Por último, para comprobar que efectivamente hemos logrado clonar el repositorio, lanzaremos el comando `ls`. Este nos devolverá todos los ficheros que hay en el directorio en el que estamos; si hemos hecho todo bien, el repositorio clonado deberá aparecer entre ellos. Si, además, queremos comprobar su contenido, podemos hacer: `ls nuevo_repositorio`.

### 38. ¿Qué hay que hacer para ver el valor de la variable de entorno de shell "PATH" con el comando "echo"?

Para saber el valor de PATH, necesito decirle al comando “echo” que se trata de una variable. Para ello, escribo en la terminal echo $PATH, donde el símbolo del dólar es lo que indica que se trata de una variable de entorno.

### 40. ¿Cómo creamos un directorio? ¿Y dos directorios? Razona tu respuesta

La creación de un nuevo directorio puede hacerse a través del comando `mkdir`. A este debe seguirle el nombre del nuevo directorio. Si queremos crear más de un directorio, simplemente añadiremos a continuación del primero y separados por un espacio los nombres de los demás directorios. Por ejemplo: `mkdir carpeta_1 carpeta_2`

### 42. ¿En qué se diferencian las rutas absolutas de las relativas? Pon ejemplos de ambas.

En el caso de las rutas absolutas, se incluye toda la dirección, incluido el directorio raíz. Por ejemplo, `/Users/pablo/periodismo_datos/README.md.` La ruta relativa, en cambio, prescinde del directorio raíz y te da la dirección desde el sitio en el que estés. Así, si esyoy ya en el directorio "pablo", la ruta relativa del archivo "README.md" sería esta: `periodismo_datos/README.md`.

### 44. Dado el significado que tienen las comillas para el comando =echo=, cómo harías para que devolviera una frase como: "Hola Mundo"

En este caso, habría que "escapar" las comillas, para que el comando entienda que no estoy usando esos caracteres de la manera en la que habitualmente los entiende. Los caracteres se "escapan" en la shell con el caracter `\`, con lo que quedaría así: `echo "\"Hola Mundo\""`.

### 49. ¿Cómo mandas la salida del comando =echo= a =lolcat=?

Podemos mandar la salida del comando `echo` a `lolcat` a través del caracter `|`: `echo "hola" | lolcat`

### 53. Pon un par de ejemplos de Google Dorks u "operadores de búsqueda"

-filetype: restringe los resultados de la búsqueda a un determinado tipo de archivo. Por ejemplo, podemos poner: `filetype:pdf`, si queremos buscar sólo archivos pdf.

-site: limita los resultados de la búsqueda a un sitio web específico. Por ejemplo, si queremos que la búsqueda sólo devuelva resultados de la página web de la Universidad Carlos III de Madrid, pondremos: `site:uc3m.es`

### 68. Como convertirías markdown a html desde pandoc

Tomamos como ejemplo un archivo md que se llame "archivo1.md". Para convertirlo a html con el comando `pandoc`, escribo lo siguiente: `pandoc archivo1.md -o archivo1.html`.

### 85. ¿Que significa TSV?

TSV es un formato de datos que significa, en inglés, tab-separated values. Implica que los valores, en lugar de por comas (como ocurre con los CSV), están separados por tabuladores. 

### 92. ¿Qué harías si al ejecutar un comando te salta el aviso "command not found"?

El aviso "command not found", que aparece a veces tras ejecutar un comando, quiere decir que no tengo el comando instalado o simplemente que dicho comando no existe. Si se trata de lo primero, podemos instalarlo; en el caso de la terminal de OSX, puedo instalarlo con `brew`, escribiendo en la terminal: `brew install lolcat`


### 19. ¿Qué programa sirve para gestionar programas en la terminal de OSX? 

Homebrew. 

### 20. ¿Qué es nano?

Nano es un editor de texto para la línea de comandos; es, por tanto, un CLI. 

### 71. Para qué usas cd y cómo.

Utilizamos `cd` para cambiar de directorio. Podemos usar rutas absolutas o relativas. Por ejemplo, si estamos en la carpeta "periodismo_datos" y queremos ir a la carpeta "apuntes", que está dentro de aquella, podemos usar la ruta relativa: `cd apuntes`.

### 72. Para qué usas cp y cómo.

El comando `cp` sirve para copiar ficheros. Hay que escribir el comando seguido del nombre del archivo que pretendemos copiar y, después, de la ruta donde queremos copiarlo. 

### 73. Para qué usas mv y cómo.

La función del comando `mv` es mover ficheros de una ubicación a otra dentro del sistema de ficheros. Funciona igual que `cp`, es decir, al comando le sigue el nombre del archivo que queremos mover y, detrás de este, la ruta a donde queremos moverlo. 

### 74. Para qué usas mkdir y cómo

`mkdir` sirve para crear un nuevo directorio, dentro del directorio en el que estamos. En la shell, escribiríamos lo siguiente: `mkdir carpeta1`. Si, en lugar de crear esta carpeta en el directorio en el que estamos, quisiéramos hacerlo en otra ubicación, escribiríamos la ruta. Por ejemplo: `mkdir periodismo_datos/carpeta1`.

### 79. ¿Qué es una API. Pon algún ejemplo.

API signfica, en inglés, Access Programming Interface (en español, interfaz de programación de acceso). Es un sistema de códigos para establecer comunicación con una página web. Un ejemplo es la API de Twitter. 

### 80. ¿Qué es Markdown?

Markdown es un lenguaje de marcado ligero creado por John Gruber. El objetivo que persigue este lenguaje es mejorar la facilidad de publicación de contenido, es decir, poder escribir más rápido y obtener un resultado mejor.

### 83. Apunta tres comandos que hayas utilizado y para qué.

`ls`: ista el contenido de un fichero determinado. 
`whoami`: me devuelve mi nombre de usuario.
`mkdir`: crear nuevos directorios. 

### 24. ¿Cuál es la estructura de las sentencias/instrucciones en la línea de comandos?

La secuencia es la siguiente: comando, opciones, argumento.

### 64. Qué es una Faceta de texto

Sirve para organizar, filtrar o agrupar datos de texto.

### 65. Qué es una faceta numérica


Sirve para organizar, filtrar o agrupar datos numéricos. 

### 66. Qué es una faceta temporal

Utilizamos una faceta temporal cuando queremos, por ejemplo, restringir los datos a un periodo de tiempo determinado. Naturalmente, la faceta temporal sólo puede aplicarse a datos que son fechas. 

### 50. ¿Cómo descargas el código fuente de una página web y se lo pasas a =lolcat=?

`lynx -source https://theguardian.com | lolcat `

### 100. ¿Quién es Philip Meyer?

Philip Meyer es considerado un pionero del periodismo de datos, debido a las aportaciones que en el campo del periodismo de investigación realizó a mediados de los años 60. Este tipo de periodismo fue también llamado Computer Assisted Reporting, debido al uso de computadoras aplicado al periodismo. Una de las investigaciones más famosas de Meyer, en las que utilizó la asistencia de computadores, tuvo que ver con los disturbios de Detroit de 1967. Su investigación, basada en encuestas analizadas por ordenador, demostró que las personas con educación universitaria tenían la misma propensión a amotinarse que los que habían abandonado la escuela secundaria. 

### 101. ¿Quién fue Florence Nightingale?

Florence Nightingale está también considerada una pionera del periodismo de datos. Esta enfermera del siglo XIX demostró, a través de una suerte de infografía (o protoinfografía), cómo las muertes de soldados en la Guerra de Crimea tenían sobre todo que ver con la falta de higiene. Por este motivo, puede considerársela una innovadara en la presentacion gráfica de datos estadísticos, favoreciendo su comprensión y, en última instancia, impulsando cambios políticos. 
