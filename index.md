## SimonTEC

En esta tarea se va a demostrar como resolver el problema de crear un juego en el que se tiene que recordar una secuencia de colores y el jugador deberá seleccionar esa
secuencia y llegar lo más lejos posible. Si el jugador se equivoca tiene que comenzar de nuevo con una nueva secuencia aleatoria.

En esta imagen se muestra como es que se vería el juego.

![Interface](https://raw.githubusercontent.com/Soir31/Tarea-corta/main/Interface.PNG)

Una vez que se pulse el botón de "start" el juego comienza y el jugador tiene que darle click al color según se vaya generando la secuencia.

### Historias de usuario

Antes de comenzar a pensar en la solución del problema, primero hay que establecer historias de usuario para tener una idea general de qué es lo que se ocupa para resolver el
problema y que cosas serían las más importantes para poder hacer el juego satisfactoriamente.

Lo primero que se hizo fue identificar las principales características que ocupa el juego. Con esas características se establecieron historias de usuario simples las cuáles
se especifican a continuación:
* Crear un juego de memoria.
* Crear una interfaz gráfica para el juego.
* Crear una secuencia aleatoria de colores.
* Guardar una secuencia aleatoria de colores.
* Recordar una secuencia aleatoria de colores.
* Aumentar una secuencia aleatoria de colores.
* Reiniciar una secuencia aleatoria de colores.

Luego se le añadió un poco más de contexto a las historias anteriores. Luego de hacer algunos ajustes las historias de usuario quedaron de la siguiente forma:
* Yo como usuario quiero un juego de memoria que tenga temática de colores para así poder tener un juego bueno para la mente.
* Yo como usuario quiero que el juego esté en forma de ruleta y dividida en 4 espacios para que así sea más fácil recordar la secuencia.
* Yo como usuario quiero que la secuencia se genere aleatoriamente para así darle dificultad al juego.
* Yo como usuario quiero que la secuencia se vaya guardando para que así pueda recordar el patrón aleatorio de colores que han salido.
* Yo como usuario quiero que la secuencia vaya aumentando cada vez que acerte un color para que el juego se vuelva todavía más difícil.
* Yo como usuario quiero que la secuencia se reinicie cuando me equivoque para así poder empezar el jugo otra vez.

Para mostrar como se organizaron estas historias de usuario se van a utilizar las historias cortas que aparecen de primero.

### Clasificación de las historias

Después de que se definieron las historias principales es necesario clasificarlas según su criticidad y su frecuencia de uso. Para esto se realizaron dos diagramas. El primer
diagrama que se va a mostrar a continuación es el diagrama en el que se realiza la clasificación según la secuencia en que se realiza cada historia.

![Usage Sequence](https://raw.githubusercontent.com/Soir31/Tarea-corta/main/Usage_Sequence.PNG)

Como se puede ver en la imagen anterior lo primero que se debe hacer es crear el juego y su interfaz gráfica, luego se crea, guarda y recuerda la secuencia aleatoria, después se
aumenta la secuencia y por último se reinicia la secuencia si el jugador perdió el juego.

En la siguiente imagen se mostrará el diagrama realizado para la frecuencia de uso y la criticidad de las historias de usuario.

![Frequency and Criticity](https://raw.githubusercontent.com/Soir31/Tarea-corta/main/Criticidad.PNG)

En la imagen se puede apreciar que el juego y la interfaz solo se construyen una vez por lo que su frecuencia de uso es baja pero su criticidad es alta ya que sin ellos no hay
juego. Lo que es la parte de la lógica del juego todos tienen una frecuencia de uso alta porque se van ejecutando conforme avanza el juego y debido a ello su criticidad también
es alta. Por último la parte de reiniciar que también es parte de la lógica del juego, se colocó con frecuencia medio porque se espera que esta parte no se ejecute tanto ya que
la idea es que el jugador no pierda, y al igual que las demás partes de lógica del juego también su criticidad es alta.

### Minimal System Span

En el siguiente diagrama se ilustra el minimal system span del problema.

![Minimal System Span](https://raw.githubusercontent.com/Soir31/Tarea-corta/main/Minimal.PNG)

En este caso podemos ver que el minimal system span sería la parte lógica del juego ya que es lo mínimo que ocupa para funcionar.

### Plan de iteraciones

Para el plan de iteraciones se dividieron las historias de usuario en dos grupos. El primer grupo es el que se realiza primero y el segundo grupo es el que se realiza depués.
El primer grupo estaría compuesto por dos historias de usuario que serían:
* Crear un juego de memoria.
* Crear una interfaz gráfica para el juego.

El segundo grupo está conformado por las demás historias de usuario que serían:
* Crear una secuencia aleatoria de colores.
* Guardar una secuencia aleatoria de colores.
* Recordar una secuencia aleatoria de colores.
* Aumentar una secuencia aleatoria de colores.
* Reiniciar una secuencia aleatoria de colores.

### Diagrama conceptual

En el siguiente diagrama se muestra como es que serviría el juego con la secuencia generada aleatoriamente.

![Conceptual Diagram](https://raw.githubusercontent.com/Soir31/Tarea-corta/main/Conceptual%20Diagram.png)

Se puede observar la secuencia que seguiría el programa y cuando llega a su final y cuando es que seguiría ejecutándose.

### Diagrama de clases

Se elaboró un pequeño diagrama de clases para tener una idea general del funcionamiento del juego de memoria. El diagrama de clases se muestra en la siguiente imagen.

![Class Diagram](https://raw.githubusercontent.com/Soir31/Tarea-corta/main/Class%20Diagram.png)

### Made by:
* Erick Daniel Obando Venegas 2019057555
