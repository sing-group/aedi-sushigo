# PROYECTO DE ALGORITMOS Y ESTRUCTURAS DE DATOS I

**Curso 2020-2021**

# El Juego: Sushi Go!

**Historia y Contexto**

Sushi Go! es un juego de cartas creado por Phil Walker-Harding en el año 2013. En este juego, el jugador asume el rol de un comensal en un restaurante  de sushi que intenta coger las mejores combinaciones de platos según pasan por delante, de modo que el jugador que coja los mejores platos será el  ganador. Cada plato puntuará de forma distinta, e incluso algunos pueden ser combinados para dar más puntos. 

En Sushi Go! cada carta representa a un plato distinto y en cada turno cada jugador escogerá una carta para quedarse con ella, representando que ha cogido un plato. Además, este juego se basa en la mecánica card-drafting que consiste en que, al final de cada turno, los jugadores le darán su mano
de cartas a otro jugador (esto es, las cartas rotan de mano).

# Bases del Juego

**Inicio del Juego**

Iniciar el juego es tan sencillo como barajar todas las cartas.

**Desarrollo del Juego**

El juego se divide en tres rondas, que se desarrollan de la misma manera.
Cada ronda comienza repartiendo cartas a los jugadores desde la baraja. Cada jugador solo podrá ver las cartas de su mano y no deberá mostrárselas a  los oponentes. Dependiendo del número de jugadores, el número de cartas a repartir será el siguiente:

- **2 jugadores**: 10 cartas a cada jugador.

- **3 jugadores**: 9 cartas a cada jugador.

- **4 jugadores**: 8 cartas a cada jugador.

- **5 jugadores**: 7 cartas a cada jugador.

  

Una vez se han repartido las cartas, cada ronda se jugará en turnos simultáneos donde cada jugador seleccionará una carta con la que se quiere quedar  de su mano actual. 

Cuando todos los jugadores hayan seleccionado una carta la pondrán de forma simultánea sobre la mesa, de modo que todos los jugadores verán sus  cartas y las seleccionadas por el resto de oponentes. Las cartas mostradas así permanecerán visibles toda la ronda. 

Tras revelar las cartas seleccionadas, los jugadores pasarán las cartas de su mano al jugador que tengan a la izquierda y comenzará un nuevo turno.
Esto se repetirá hasta que no queden más cartas en las manos de los jugadores, momento en el cual se puntuará la ronda según indican las cartas. Una vez puntuada la ronda, se descartarán todas las cartas de la mesa (no participarán en las siguientes rondas), exceptuando las de Pudding, cuyo funcionamiento se explica más adelante.

**Cartas**

Las cartas que forman parte del juego son las siguientes

- **Nigiri de calamar**: Vale 3 puntos.

- **Nigiri de salmón**: Vale 2 puntos.

- **Nigiri de tortilla**: Vale 1 punto.

- **Wasabi**: Si hay una carta de Wasabi sobre la mesa cuando se coge un Nigiri, la carta de Nigiri puede colocarse sobre el Wasabi triplicando su valor (p.ej. si se coloca un Nigiri de Salmón sobre un Wasabi, valdrá 6 puntos en lugar de 2). Tan solo se puede colocar un Nigiri sobre un Wasabi y un Wasabi por sí solo no vale ningún punto.

- **Maki**: En cada carta de Maki puede aparecer 1, 2 o 3 rollitos. El jugador con más rollitos al final de la ronda ganará 6 puntos. Es necesario tener al menos un rollito para puntuar. Si dos o más jugadores empatan en el mayor número de rollitos, los 6 puntos se dividen entre ellos, redondeando hacia abajo.

- **Tempura**: Cada pareja de Tempuras vale 5 puntos. Una Tempura sola no vale ningún punto.

- **Sashimi**: Cada trío de Sashimis vale 10 puntos. Uno o dos Sashimis solos no valen ningún punto.

- **Gyoza**: Cuantas más Gyoza más puntos valdrán. El valor de las Gyoza, dependiendo del número de cartas de Gyoza que hayamos cogido, será el  iguiente:

​		**Gyoza**     1       2       3       4       5 o más

​		**Puntos**   1       3       6      10     15

- **Palillos**: Los Palillos no valen ningún punto, pero permiten coger más de una carta por turno. Un jugador que tenga una carta de palillos en mesa, tras haber cogido la carta correspondiente del turno, podrá devolver una carta de palillos de la mesa a su mano para coger una segunda carta.

- **Pudding**: Los Pudding se puntúan únicamente al final del juego (tras la tercera ronda) y permanecen en la mesa de los jugadores entre rondas. El  jugador con más cartas de Pudding ganará 6 puntos, mientras que el jugador con menos cartas de Pudding perderá 6 puntos. Si varios jugadores empatan en la primera o última posición, dividirán los puntos ganados o perdidos, redondeando hacia abajo.

​	Si todos los jugadores tienen el mismo número de Pudding, nadie ganará puntos por ellos. En las partidas de 2 jugadores, ningún jugador pierde 	puntos por los Pudding.

La baraja se compone de un total de 108 cartas, distribuidas de la siguiente manera:

* Nigiri de calamar: 5
* Nigiri de salmón: 10
* Nigiri de tortilla: 5
* Wasabi: 6
* Maki de 1 rollo: 6
* Maki de 2 rollos: 12
* Maki de 3 rollos: 8
* Tempura: 14
* Sashimi: 14
* Gyoza: 14
* Palillos: 4
* Pudding: 10



**Final de la Partida**

La partida finaliza tras la tercera ronda. En este momento, se calculará la puntuación de cada jugador sumando los puntos de cada ronda y los puntos  ganados o perdidos por los Puddings. 

El jugador con más puntos será el ganador. Si hay empate, el jugador con más Puddings será el ganador. Si el empate persiste, todos los jugadores que han empatado serán los ganadores.

**Información Adicional**

En la página http://www.adventurelandgames.com/SushiGoRules.pdf se pueden ver las reglas oficiales en inglés, en las cuales está basado este  documento. Un video ejemplo de cómo jugar se puede consultar en: https://www.youtube.com/watch?v=JlN8BvUoJ2k



# PROYECTO A ENTREGAR

1. El trabajo será **colaborativo**, es decir se realizará en grupo de 4/5 alumnos/as, que deben pertenecer al mismo grupo reducido de AEDI. La formación  de los equipos corre por cuenta de los alumnos e informarán a su profesor/a. Los alumnos no presenciales también deben realizar el proyecto y formarán grupo con otros alumnos no presenciales. Si tienen dificultad para formar grupo deben hablar con su profesor/a, que estudiará cada caso.

2. El trabajo consiste en desarrollar un proyecto que implemente el juego del **Sushi Go!** siguiendo las reglas anteriormente expuestas, utilizando el lenguaje de programación JAVA y el entorno NetBeans.

3. La estructura del proyecto, en la que están identificadas las clases implicadas en el diseño de la aplicación está disponible en Moovi, sección  Práctica:Proyecto/ <u>ProySushiGo</u>. El proyecto está organizado en 2 paquetes: IU y core. Algunas clases están completamente   implementadas y otras deben ser desarrolladas por el grupo.

4. El profesor/a repartirá el trabajo entre todos los miembros del grupo, de modo que cada uno de los miembros debe ocuparse de desarrollar  alguna/s de la/s clase/s. También sería preciso nombrar un **coordinador de grupo**, siendo el responsable de la coordinación del proyecto. Si algún miembro del grupo no cumple sus funciones, el coordinador del grupo debe comunicárselo al profesor/a.

5. Cada miembro del grupo debe ser responsable de su trabajo, de comunicarse con otros miembros del grupo y de conocer todas las partes del  proyecto. Además, debe reflexionar y desarrollar cada clase implementando los métodos. Se debe tener especial cuidado en controlar la visibilidad de los atributos, métodos, además de utilizar los algoritmos y las estructuras de datos adecuadas en cada caso.

6. Para facilitar la implementación, sólo se tendrán en cuenta las cartas: Nigiri (todos los tipos), Tempura, Sashimi, Gyoza, Wasabi y Maki, que hacen un total de 94 cartas. Por tanto, las cartas a repartir son:

   - **2 jugadores**: 9 cartas a cada jugador.
   - **3 jugadores**: 8 cartas a cada jugador.
   - **4 jugadores**: 7 cartas a cada jugador.
   - **5 jugadores**: 6 cartas a cada jugador.

7. Respecto al funcionamiento del juego, deben cumplirse las siguientes condiciones:

   - Al principio de la partida, deberá preguntarse por el número de jugadores y el nombre de cada uno.

   - Realizar la validación de datos de entrada por teclado.

   - La colocación de las cartas en la mesa se realiza de forma automática, si hay un Wasabi en la mesa, y el jugador selecciona un Nigiri se colocará encima de la carta Wasabi. También se apilarán cartas del mismo tipo; es decir, Tempuras, Sashimis, Makis y Gyozas. Los Nigiris no se apilarán entre sí.

   - En cada turno, se debe mostrar el estado de la mesa de todos los jugadores y la mano del jugador activo.

   - Al final de cada ronda debe mostrarse la puntuación de cada jugador en cada ronda y un total.

   - Al terminar el juego deben mostrarse los puntos de cada ronda y puntuación final, además, el nombre del ganador o ganadores.

8. La fecha tope para subir el proyecto a Moovi de forma individual (cada miembro subirá el proyecto completo) será **el viernes 14 de mayo de 2021 a las 23:00h**, a Moovi, sección Práctica:Proyecto/ <u>Entrega Proyecto SushiGo</u>.

9. Solo se admiten proyectos que compilen y que se ejecuten cumpliendo las reglas del juego.

10. **El descubrimiento de copias del proyecto supondrá el suspenso del mismo, tanto para el grupo con código original, como para el grupo con la copia**.



# EVALUACIÓN

La evaluación constará de dos partes: grupal, en forma de tutoría obligatoria, e individual en forma de examen en el ordenador.

1. **Evaluación grupal: tutoría obligatoria** para todos los miembros del grupo, en la que semostrará la evolución del proyecto y donde el profesor/a podrá preguntar a cada miembro del grupo sobre su trabajo o sobre el de sus compañeros; el profesor/a marcará con cada grupo cuándo se realizará la tutoría, que será entre **el 18 y 21 de mayo**. Esta tutoría es evaluable (sólo para los que siguen la modalidad de asistentes) y supondrá el 15% de la calificación final de la asignatura.
2. **Evaluación individual**: se realizará en ordenador el **7 de junio de 2021**. Supondrá <u>el 25% de la calificación final</u> de la asignatura para la modalidad de asistentes y el <u>40% de la calificación final</u> de la asignatura para la modalidad de no asistentes.