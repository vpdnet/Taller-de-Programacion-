
| Instrucción / Identificador | Descripción |
|---|---|
| `AsignarArea(robot, area)` | Asigna al robot un área de trabajo. Recibe dos parámetros: el robot y el área que debe asignarse. |
| `Iniciar(robot, avenida, calle)` | Instrucción primitiva que posiciona al robot en la esquina indicada, orientado hacia el norte. |
| `derecha` | Instrucción primitiva que cambia la orientación del robot en 90° en sentido horario respecto de la orientación actual. |
| `mover` | Instrucción primitiva que conduce al robot de la esquina en la que se encuentra a la siguiente, respetando la dirección en la que está orientado. Es responsabilidad del programador que esta instrucción sea ejecutada dentro de los límites de la ciudad. En caso contrario, se producirá un error y el programa será abortado. |
| `tomarFlor` | Instrucción primitiva que permite al robot recoger una flor de la esquina en la que se encuentra y ponerla en su bolsa. Debe ejecutarse solo cuando haya al menos una flor en dicha esquina. |
| `tomarPapel` | Instrucción primitiva que permite al robot recoger un papel de la esquina en la que se encuentra y ponerlo en su bolsa. Debe ejecutarse solo cuando haya al menos un papel en dicha esquina. |
| `depositarFlor` | Instrucción primitiva que permite al robot depositar una flor de su bolsa en la esquina en la que se encuentra. Debe ejecutarse solo cuando haya al menos una flor en la bolsa. |
| `depositarPapel` | Instrucción primitiva que permite al robot depositar un papel de su bolsa en la esquina en la que se encuentra. Debe ejecutarse solo cuando haya al menos un papel en la bolsa. |
| `PosAv` | Identificador que representa el número de avenida en la que el robot está actualmente posicionado. Su valor es un número entero en el rango 1..100. |
| `PosCa` | Identificador que representa el número de calle en la que el robot está actualmente posicionado. Su valor es un número entero en el rango 1..100. |
| `HayFlorEnLaEsquina` | Proposición atómica cuyo valor es V si hay al menos una flor en la esquina en la que el robot está actualmente posicionado, o F en caso contrario. Su valor no puede ser modificado por el programador. |
| `HayPapelEnLaEsquina` | Proposición atómica cuyo valor es V si hay al menos un papel en la esquina en la que el robot está actualmente posicionado, o F en caso contrario. Su valor no puede ser modificado por el programador. |
| `HayFlorEnLaBolsa` | Proposición atómica cuyo valor es V si hay al menos una flor en la bolsa del robot, o F en caso contrario. Su valor no puede ser modificado por el programador. |
| `HayPapelEnLaBolsa` | Proposición atómica cuyo valor es V si hay al menos un papel en la bolsa del robot, o F en caso contrario. Su valor no puede ser modificado por el programador. |
| `Pos(avenida, calle)` | Instrucción que requiere dos valores Av y Ca, ambos en el rango 1..100. Posiciona al robot en la esquina determinada por el par (Av, Ca) sin modificar su orientación. |
| `Informar(variable)` | Instrucción que permite visualizar en pantalla el contenido almacenado en una variable. También puede informar una expresión numérica o lógica. Ejemplo: `Informar(HayFlorEnLaEsquina)`. |
| `Random(variable, inf, sup)` | Instrucción que calcula un número aleatorio entre los límites inf y sup (ambos incluidos) y retorna su valor en variable. |
| `BloquearEsquina(avenida, calle)` | Instrucción para que el robot solicite acceso exclusivo a una esquina, compitiendo por el recurso con los demás robots solicitantes. Recibe el número de avenida y calle a bloquear. |
| `LiberarEsquina(avenida, calle)` | Instrucción para que el robot libere el acceso exclusivo a una esquina. Recibe el número de avenida y calle a liberar. |
| `EnviarMensaje(variable, robot)` | Instrucción que permite a un robot enviar un dato a otro. Recibe dos parámetros: el dato o variable a enviar y el robot que recibirá el mensaje. |
| `RecibirMensaje(variable, robot)` | Instrucción que permite a un robot recibir un dato de otro. Recibe la variable donde se almacenará el dato y el robot de quien espera el mensaje. Si el parámetro del robot es `*`, el mensaje puede recibirse de cualquier robot por orden de llegada. |
| `miVariable : tipoDeDato` | Declaración de una variable que puede ser de tipo numero, boolean o el nombre de un nuevo robot, declarado previamente en su sección correspondiente. |
| `miVariable := valor` | Forma de asignar un valor numérico, booleano o el contenido de otra variable. |
| `si (condicion)` | Estructura de control de selección. |
| `sino` | Bloque de ejecución alternativo de la estructura de control SI. |
| `mientras (condicion)` | Estructura de control de iteración condicional. |
| `repetir N` | Estructura de control de repetición. N es el número fijo de veces que se ejecutará el conjunto de instrucciones dentro de la estructura. |
| `V` | Representación del valor verdadero (true), que puede asignarse a una variable booleana. |
| `F` | Representación del valor falso (false), que puede asignarse a una variable booleana. |
| `~` | Símbolo de negación lógica. |
| `\|` | Conector lógico OR. |
| `&` | Conector lógico AND. |
