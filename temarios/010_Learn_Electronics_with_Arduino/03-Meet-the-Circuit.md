# Chapter 3: Meet the Circuit

* The Circuit: Building Block of Electronics
* The Schematic
* Using a Breadboard
* Building a Circuit
* A Look at the Battery
* Power for Our Circuit: Electricity
* Debugging the Circuit
* The Multimeter
* Using the Multimeter
* Back to Debugging Our Circuit
* Summary

# Conoce el circuito

En el último capítulo, aprendiste un poco sobre Arduino y sus partes. También le presentaron algunos de los componentes y herramientas que utilizará para completar los proyectos de este libro. En este capítulo, aprenderá algo de la práctica y la teoría de la electrónica que necesitará saber para construir circuitos usando Arduino. Todavía no usaremos un Arduino, pero volveremos a eso en breve.

## EL CIRCUITO: BLOQUE DE CONSTRUCCIÓN DE ELECTRÓNICA

El circuito es el bloque de construcción básico para todos los proyectos de electrónica que construiremos con Arduino.

Puede construir muchos tipos diferentes de proyectos con un Arduino; solo está limitado por su imaginación. Aunque existen muchos tipos diferentes de proyectos, todos los proyectos de este libro se construyen utilizando circuitos.

Primero, veremos qué es un circuito; luego, construirás tu primer circuito. También veremos técnicas para representar circuitos electrónicos visualmente y le mostraremos cómo probar sus circuitos.

La Figura 3-1 ilustra algunos proyectos de Arduino. Puede ver que los circuitos en estos proyectos toman diferentes formas. En el robot de cartón, no se puede ver el circuito, pero eso es lo que controla al robot.

![03-01](images/03_01.png)

***Figura 3-1***: Algunos ejemplos de proyectos que usan Arduino como parte de un circuito

Veamos más de cerca qué es un circuito.

### ¿QUÉ ES UN CIRCUITO?

Si alguna vez has estado en una carrera de autos, sabes que se refieren a la pista como un circuito. Un circuito simplemente significa que hay un circuito cerrado completo, como se muestra en los circuitos de la Figura 3-2. Los coches pasan desde la línea de salida y terminan en el mismo lugar.

![03-02](images/03_02.png)

***Figura 3-2***: Pistas del circuito

Lo mismo ocurre con los circuitos electrónicos. Un circuito electrónico describe un circuito cerrado y completo. Un circuito incluye todos los componentes electrónicos necesarios para una tarea, así como cables u otro material que permitirá que la electricidad fluya entre los componentes conectados, como puede ver en la Figura 3-3.

![03-03](images/03_03.png)

***Figura 3-3***: El flujo del circuito comienza y termina con la fuente de energía.

### ¿POR QUÉ ESTAMOS HACIENDO CIRCUITOS?

Piense por un momento en los interruptores de luz de su hogar como modelo. Para encender o apagar un interruptor, debe estar en contacto físico con el interruptor. En nuestros proyectos, Arduino controlará el comportamiento de los componentes electrónicos. Nuestros componentes electrónicos estarán dispuestos en un circuito, y Arduino debe ser parte de ese circuito para que pueda controlar el comportamiento.

Los circuitos permiten que Arduino se conecte a los componentes eléctricos, apagando y encendiendo una variedad de objetos (parlantes, LED, motores, etc.) o tomando información del mundo exterior ("¿Qué temperatura hace?"; "¿Está el interruptor encendido? ? ”; Etc.). Siempre que averigüemos cómo conectar Arduino al objeto, podemos controlarlo con electricidad y, más tarde, con programación.

### ¿QUÉ COMPONE A UN CIRCUITO?

Hay dos partes principales que componen un circuito: ***líneas conductoras*** y ***componentes***.

#### Líneas conductoras

Aunque la mayor parte del enfoque de un circuito se coloca en los componentes, no puede tener un circuito sin algún tipo de conexión entre los componentes. Nuestras computadoras y dispositivos electrónicos contienen placas de circuito impreso (PCB). Los PCB, que no conducen electricidad, están compuestos por capas base de material sobre las que se han aplicado líneas finas de material conductor, como se ve en la Figura 3-4. Las líneas conductoras conectan componentes que están soldados a la PCB. Si miras una PCB, notarás las líneas plateadas brillantes que se extienden entre los componentes, conectándolos. Estas líneas son como cables pegados a una superficie plana.

![03-04](images/03_04.png)

***Figura 3-4***: Detalle de placa de circuito impreso

#### Componentes

Los componentes son el otro requisito para un circuito completo. Observamos una lista completa de componentes para comprar en el Capítulo 1, "Introducción a Arduino". Los componentes forman las ubicaciones que deben conectarse dentro de un circuito (Figura 3-5).

![03-05](images/03_05.png)

***Figura 3-5***: Los circuitos están hechos de componentes.

En la Figura 3-6, puede ver que los cables de los componentes actúan como líneas conductoras.

![03-06](images/03_06.png)

***Figura 3-6***: La electricidad fluye a través de líneas conductoras.

### ¿POR DÓNDE EMPEZAMOS?

***El primer circuito que vamos a construir juntos es una linterna de bombilla LED que funciona con una batería***. Este circuito es un gran proyecto para principiantes porque la luz que se enciende confirma visualmente que el circuito está funcionando. El circuito de la linterna también demuestra las técnicas básicas de construcción de circuitos que necesitará en todos los proyectos de este libro.

La Figura 3-7 es un dibujo del circuito una vez completado, con las partes anotadas. Explicaremos lo que hacen las partes en detalle, parcialmente en este capítulo y también en los próximos capítulos. Por ahora, sepa que este circuito se construirá a partir de un LED, una resistencia, un puente, una batería de 9 V y una tapa de batería dispuesta en una placa de pruebas, componentes que conoció en el Capítulo 1.

Hay muchas formas diferentes de representar o dibujar circuitos para transmitir la información necesaria. En la Figura 3-7, hemos hecho una aproximación de cómo se verá el circuito cuando lo construya. Esta no es siempre la forma más clara de ver lo que está sucediendo; algunos circuitos tienen muchas partes que están conectadas de formas complejas. Los esquemas son una excelente manera de hacer un dibujo de un circuito que tiene partes simplificadas y mostrar cómo están conectadas. Echemos un vistazo más de cerca a cómo funcionan los esquemas.

![03-07](images/03_07.png)

***Figura 3-7***: El circuito que construiremos

## EL SCHEMATIC - ESQUEMA

***Un esquema es un diagrama de las relaciones de los componentes electrónicos en un circuito***. En un esquema, verá los componentes que forman parte del circuito y cómo se unen entre sí. Comencemos mirando un esquema simple que representa nuestro circuito básico. Pronto entraremos en detalles sobre lo que significa cada símbolo en el esquema, pero por ahora echemos un vistazo rápido. La figura 3-8 compara un esquema del circuito que estamos a punto de construir con un dibujo del circuito.

![03-08](images/03_08.png)

***Figura 3-8***: Esquema del circuito con un dibujo del circuito.

### ¿POR QUÉ ES IMPORTANTE APRENDER A LEER UN ESQUEMA?

La mayoría de los proyectos y componentes electrónicos están representados por esquemas, no necesariamente por dibujos o fotografías. A medida que avancen sus habilidades electrónicas y desee crear sus propios proyectos fuera de este libro, deberá poder leer y dibujar esquemas para investigar sus proyectos, así como describirlos y construirlos.

Comenzamos con esquemas simples; construiremos representaciones más complejas a medida que construimos proyectos más complejos en el libro. Al mirar los esquemas en línea o en otra documentación, puede notar que a veces hay variaciones en la forma en que se dibujan o organizan los símbolos. No se preocupe si todos los símbolos esquemáticos no se ven exactamente iguales, como se muestra en la Figura 3-9.

![03-09](images/03_09.png)

***Figura 3-9***: Símbolos esquemáticos para LEDs

### DIAGRAMA DE SU CIRCUITO: EL ESQUEMA

Ha aprendido que un esquema es la forma estándar de representar las relaciones eléctricas en un circuito. Todos los componentes electrónicos de uso común tienen un símbolo para representarlos dentro de los diagramas esquemáticos electrónicos para dejar en claro lo que se adjunta dentro del circuito. La figura 3-10 muestra un circuito básico de un LED, una resistencia y una batería. El LED tiene una orientación, un cable positivo (ánodo) y un cable negativo (cátodo), como se menciona en el Capítulo 1.

Los esquemas se preocupan principalmente por diagramar cómo se conectan los componentes en el circuito, y sacrificarán la claridad en cómo se configuran físicamente los componentes para demostrar mejor cómo se conectan electrónicamente.

![03-10](images/03_10.png)

***Figura 3-10***: Esquema anotado del circuito.

La Tabla 3-1 muestra los símbolos de los componentes que están en nuestro primer circuito. La página de Wikipedia sobre símbolos electrónicos es un buen lugar para obtener una descripción general de muchos de los símbolos utilizados en los esquemas: https://en.wikipedia.org/?title=Electronic_symbol.

***Tabla 3-1***: Componentes con sus símbolos esquemáticos

COMPONENTE | DESCRIPCIÓN | SIMBOLO EN EL ESQUEMA
-----------|-------------|----------------------
![UF_03_01](images/UF_03_01.png) | Batería | ![UF_03_02](images/UF_03_02.png)
![UF_03_03](images/UF_03_03.png) | LED (diodo emisor de luz) | ![UF_03_04](images/UF_03_04.png)
![UF_03_05](images/UF_03_05.png) | Resistencia | ![UF_03_06](images/UF_03_06.png)

También hay algunas otras formas en que se pueden dibujar los símbolos de una fuente de energía, como puede ver en la Figura 3-11. Cubriremos los conceptos de *Potencia* y *Tierra* más adelante en el capítulo, pero reconocer estos símbolos lo ayudará a comprender lo que está sucediendo en nuestro circuito.

![03-11](images/03_11.png)

***Figura 3-11***: Símbolos esquemáticos de potencia y tierra.

### DIBUJAR UN ESQUEMA

Ha visto un ejemplo de un esquema, así como los símbolos que se utilizan en el esquema de nuestro primer circuito. ¿Cómo se conectan los símbolos para dibujar un esquema?

Comenzaremos con el símbolo de una resistencia en la Figura 3-12. Recuerde que la resistencia no tiene una orientación positiva-negativa, por lo que no importa qué extremo es cuál.

![03-12](images/03_12.png)

***Figura 3-12***: Símbolo esquemático de una resistencia

A continuación, dibujaremos el símbolo del LED y lo conectaremos a la resistencia con una línea continua. ¿Por qué la línea es sólida? Recuerde que estamos representando la conexión física entre los componentes del circuito, al igual que las líneas plateadas conductoras en la PCB.

El extremo positivo, o ánodo, se conecta a la resistencia como lo hará en el circuito cuando lo construyamos, como se ve en la Figura 3-13. Cuando conectamos la batería, la energía fluirá a través de la resistencia hasta el extremo positivo del LED.

![03-13](images/03_13.png)

***Figura 3-13***: Resistencia conectada al ánodo del LED

Ahora agregamos el símbolo de la batería y lo conectamos a los símbolos de LED y resistencia, como se muestra en la Figura 3-14. El extremo negativo del LED, o cátodo, se conecta al extremo negativo de la batería.

![03-14](images/03_14.png)

***Figura 3-14***: Esquema del circuito

Podemos ver en este esquema que un extremo de la resistencia está conectado a la alimentación, o el signo más en la batería. El otro extremo de la resistencia está conectado al extremo positivo del LED. El extremo negativo del LED está conectado a tierra, o el signo menos. Nuestro esquema representa el bucle completo de nuestro circuito.

## USANDO UN BREADBOARD

¿Cómo conectamos los componentes para construir un circuito? Si observa la Figura 3-15, puede ver que hay una placa de pruebas debajo de todos los componentes.

¿Por qué usamos una placa de pruebas? El breadboard nos permite conectar todos nuestros componentes. Nunca podríamos unir todas las piezas con los dedos, y no queremos unirlas permanentemente entre sí inicialmente. Sabemos que un circuito es un bucle y que los componentes deben estar conectados. La placa de pruebas nos permite conectar nuestros componentes entre sí rápidamente y nos da la flexibilidad de ajustar fácilmente nuestros circuitos. El uso de una placa de pruebas nos permite crear rápidamente un prototipo de nuestros proyectos.

![03-15](images/03_15.png)

***Figura 3-15***: El circuito que estaremos construyendo, con la placa de pruebas

> **Nota**
> 
> El uso de una placa de pruebas nos permite unir componentes entre sí rápidamente y realizar ajustes en nuestro circuito.

### CONCEPTOS BÁSICOS DEL BREADBOARD

Has visto imágenes de una placa de pruebas y circuitos montados en una placa de pruebas. También sabe que el uso de una placa de pruebas le permite crear prototipos de circuitos rápidamente y probarlos. ¿Cómo se construye una placa de pruebas? Veamos una vista de "rayos X" de una placa de pruebas.

> **Advertencia**
> 
> En realidad, no retire el respaldo; hacerlo podría arruinar su placa de pruebas.

Una placa de pruebas tiene tiras de metal recubiertas de plástico con una rejilla de agujeros en la parte superior. Los agujeros, llamados puntos de unión, se colocan a intervalos regulares y se organizan en filas y columnas.

En la Figura 3-16, puede ver las tiras de metal dispuestas sobre filas y columnas de puntos de unión. Todos los puntos de unión que están conectados a una de las tiras de metal están conectados entre sí.

![03-16](images/03_16.png)

***Figura 3-16***: Una vista de "rayos X" de una placa de pruebas

Las filas y las columnas están organizadas en patrones para facilitar la construcción de circuitos con componentes electrónicos estándar.

Las columnas largas en el extremo izquierdo y derecho de la placa que se muestra en la Figura 3-17 están unidas por convención a la alimentación y la tierra, y se denominan buses de alimentación y de tierra. Hay un signo más (+) o un signo menos (-) en la parte superior de cada columna. Se adjuntarán a los signos más y menos de la batería. A menudo hay una línea roja cerca del bus de energía y una línea verde, azul o negra al lado del bus de tierra. Algunas placas de prueba, particularmente las más pequeñas, no tienen estos buses de potencia.

![03-17](images/03_17.png)

***Figura 3-17***: Buses de alimentación y tierra en una placa de pruebas

Explicaremos más sobre la alimentación y la tierra más adelante. Por ahora, solo necesita saber que conectaremos una batería a los buses en un lado del tablero, y los buses del lado izquierdo y derecho no están conectados. Izquierda o derecha, no importa a qué lado de la placa de pruebas conecte la alimentación y la tierra, aunque conectaremos la batería al lado izquierdo de la placa. Es una buena idea ser coherente en la forma en que configura su breadboard.

### HACER CONEXIONES

Generalmente existe un espacio, conocido como zanja, en el medio; tiene el mismo ancho que algunos componentes, para facilitar su conexión al circuito. Los puntos de unión en cada fila a cada lado de la zanja están conectados, lo que le permite hacer conexiones entre los componentes cuando los coloca en la placa. La Figura 3-18 muestra que *no* se conectan a través de la zanja; cada fila de puntos de unión a cada lado de la zanja es una fila discreta.

![03-18](images/03_18.png)

***Figura 3-18***: Fila de puntos de amarre en el breadboard

> **Nota**
> 
> Las filas en una placa de pruebas no se conectan a través de la zanja.

Los componentes se pueden conectar entre sí colocándolos en la misma fila de puntos de unión, como se muestra en la Figura 3-19.

![03-19](images/03_19.png)

***Figura 3-19***: Componentes conectados en protoboard

> **¿Preguntas?**
> 
> P: ¿Necesito una placa de pruebas nueva para cada circuito que construyo?
> R: Lo mejor de las placas de prueba es que es muy fácil cambiar las partes de un circuito o hacer uno nuevo por completo. Podrías hacer todos los circuitos del libro simplemente reutilizando una placa. Si desea tener más de un circuito configurado a la vez, es útil tener una placa adicional.

## CONSTRUYENDO UN CIRCUITO

¡Vamos a construir nuestro primer circuito! Necesitará estas piezas y herramientas:

* Breadboard
* Batería de 9V
* Tapa de la batería
* 1 LED
* Resistencia de 330 ohmios (bandas de color naranja, naranja, marrón, dorado)
* Cables de puente (Jumper wires)
* Pinzas de punta de aguja

Reúna todas sus piezas para comenzar a construir el circuito de la Figura 3-20.

![03-20](images/03_20.png)

***Figura 3-20***: El circuito

### 🔋 INSTRUCCIONES DE CIRCUITO PASO A PASO

Lo guiaremos a través de los pasos para hacer el circuito básico que le mostramos a lo largo del capítulo. Es posible que todavía no comprenda exactamente cómo funcionan juntas todas las partes del circuito. No se preocupe por esto, le explicaremos más sobre la electricidad en un circuito y sobre cada componente a medida que avanzamos. Por ahora, solo sigue los pasos.

Las primeras partes que necesitará son la placa de pruebas y la resistencia de 330 ohmios. Más adelante aprenderá más sobre resistencias, pero ahora solo necesita una resistencia que tenga cuatro bandas con los colores naranja, naranja, marrón y dorado.

Elija una esquina de la placa de pruebas; comenzamos con la esquina superior izquierda. (No importa si elige los buses de la derecha o la izquierda, pero es preferible ser consistente). Primero coloque un extremo de la resistencia de 330 ohmios (con bandas de color naranja, naranja, marrón y dorado) en el bus de energía (marcado con el signo +) de su breadboard y el otro extremo en una fila de su breadboard. Tendrás que doblar un poco los cables para poder meterlos en el board.

Las resistencias no tienen una dirección hacia adelante o hacia atrás en un circuito, por lo que no importa cuál sea la orientación. Cada ventaja o pierna es la misma. La figura 3-21 muestra cómo se conecta la resistencia.

> **Tip**
> 
> Los componentes deben sentirse como si estuvieran presionados en su lugar. A veces es difícil introducir los componentes completamente en la placa. Sea paciente. A algunas personas les resulta más fácil usar alicates de punta fina para pegar componentes en el board, mientras que otras solo usan sus manos. Vea qué es más fácil para usted.

![03-21](images/03_21.png)

***Figura 3-21***: Primero agregue la resistencia.

Luego agregue un LED (Figura 3-22). El ánodo (cable largo) va en la misma fila de puntos de unión que la resistencia. El cátodo (cable corto) pasa a la siguiente fila.

La Figura 3-23 muestra cómo un extremo de la resistencia está en la misma fila de puntos de unión que el ánodo del LED.

![03-22](images/03_22.png)

***Figura 3-22***: Agregue el LED.

![03-23](images/03_23.png)

***Figura 3-23***: LED colocado correctamente

A continuación, debe colocar un puente que conecte el bus de tierra (marcado con el signo -) al cátodo del LED, como se muestra en la Figura 3-24. El uso de un puente negro indicará que va a tierra. El puente está ahí para hacer una conexión entre el cátodo y el bus de tierra.

![03-24](images/03_24.png)

***Figura 3-24***: Agrega un puente a la tierra.

Agregue la tapa de la batería en el bus de alimentación y tierra de la placa de pruebas (Figura 3-25). Tiene extremos de metal que encajarán en el bus de alimentación y de tierra.

> **Tip**
>
> Asegúrese de obtener un ajuste seguro en la placa de pruebas. Hacerlo puede ser complicado; a veces, puede ayudar torcer el cable en el extremo de la tapa de la batería.

![03-25](images/03_25.png)

***Figura 3-25***: Agregue la tapa de la batería a la placa de pruebas.

## UNA MIRADA A LA BATERÍA

Echemos un vistazo más de cerca a la batería de 9 V y la tapa de la batería. La parte superior de la batería tiene dos terminales que se conectan a los conectores a presión en la tapa de la batería, como se muestra en la Figura 3-26. El más pequeño, junto al signo más (+), es el terminal de alimentación. La terminal más grande, junto al signo menos (-), es la terminal de tierra.

![03-26](images/03_26.png)

***Figura 3-26***: Batería de 9 voltios de cerca

Dé la vuelta a la tapa de la batería y observe los dos conectores a presión. El conector pequeño se conectará al terminal de tierra y el conector grande se conectará al terminal de alimentación, como se ve en la Figura 3-27.

![03-27](images/03_27.png)

***Figura 3-27***: La tapa de la batería

Los conectores a presión solo se acoplarán correctamente si la batería está correctamente orientada, como se muestra en la Figura 3-28. La tapa o el soporte de la batería pueden verse diferentes, pero seguirán las mismas convenciones.

![03-28](images/03_28.png)

***Figura 3-28***: Colocación de la tapa en la batería

### ¡HAGA LA LUZ!

Ahora coloque la batería en la tapa. Su LED debería encenderse (Figura 3-29). ¡Has hecho tu primer circuito!

![03-29](images/03_29.png)

***Figura 3-29***: ¡Tu LED se enciende!

Este es solo el primero de muchos LED en el libro, pero se siente bien por haber encendido este primero. A continuación, veamos cómo la batería proporciona energía a nuestro circuito.

> **¿Preguntas?**
> 
> P: ¿Qué pasa si no tengo la resistencia que sugieres?
> R: Recomendamos comprar una amplia gama de resistencias inicialmente para asegurarse de que tiene todas las resistencias sugeridas para los primeros proyectos y capítulos del libro. Aunque hay formas de combinar resistencias para cambiar su valor, no las cubriremos en detalle en este libro. Por lo general, es mejor tener una variedad para empezar.

## POTENCIA PARA NUESTRO CIRCUITO: ELECTRICIDAD

El término ***potencia*** tiene un significado específico cuando se habla de electricidad, que explicaremos más adelante. Por el momento, la potencia aquí se refiere al hecho de que la electricidad proviene de nuestra batería, pasa a través de la resistencia al LED y se enciende. Echemos un vistazo más de cerca a cómo se indica esto tanto en nuestra batería como con el color de los cables en nuestro circuito. Observamos brevemente los símbolos más y menos en la batería al colocar la tapa de la batería; ahora veremos los símbolos con más detalle.

### UNA PALABRA SOBRE LOS SÍMBOLOS DE PODER

Como puede ver en la Figura 3-30, hay un lado + (positivo) y un lado - (negativo) en una batería, los símbolos convencionales que se usan para marcar qué lado de la batería produce energía (positivo) y qué lado es el lado de tierra (negativo). (Y ha visto los signos más y menos en los autobuses en la placa de pruebas). También vio que el lado positivo de la batería conectado al cable rojo en la tapa de la batería y el lado negativo conectado al cable negro de la batería gorra.

![03-30](images/03_30.png)

***Figura 3-30***: Los lados positivo y negativo de una batería

#### Power

El signo +, o el positivo, marca el lado de alimentación de la batería. La convención es que la energía fluye desde este lado de la batería, y todas las rutas en su circuito deben remontarse al lado de la energía. Los estándares también establecen que todos los cables que están conectados al lado positivo son rojos. De esta manera, cualquier persona que necesite revisar o reparar su circuito puede saber inmediatamente desde dónde ingresa la energía a su circuito.

#### Ground

El - es el lado negativo de la batería, también conocido como lado de tierra. Así como todos los caminos en el circuito deben comenzar con el lado de potencia, todos deben terminar en el lado de tierra si los trazas a lo largo de toda la longitud. Se puede pensar en la tierra como el lado "cero", el lugar donde se ha agotado toda la energía. Todos los cables que regresan a la parte de tierra del circuito deben ser negros; eso hará que sea más fácil trabajar en sus circuitos y saber de un vistazo qué partes están conectadas a tierra.

Hemos mirado un poco la potencia y la tierra, y tú construiste tu circuito. Pero, ¿qué pasa si su LED no se enciende? ¿Qué pasos puede tomar para encontrar su problema y arreglar su circuito?

> **¿Preguntas?**
> 
> P: ¿Necesito usar una batería nueva para encender mi LED? ¿Puedo usar una batería vieja que encontré o pedí prestada en mi casa?
> R: Sí, puede, pero es probable que sus luces no brillen tanto como cuando usa una batería nueva. Las baterías se agotan con el tiempo.

## DEPURACIÓN DEL CIRCUITO

¿Algo salió mal o no funciona bien? ¿Qué pasa si el LED no se enciende? ¿Qué podría estar mal? ¡Depurando!

Verificar su circuito para ver qué está mal se llama ***depuración***. La depuración no se trata solo de resolver el problema inmediato, sino también de crear una lista de verificación de posibles problemas y resolverlos uno por uno. A veces, la solución "obvia" es la más difícil de encontrar y, al seguir una lista de verificación, es seguro que no se perderá nada.

### ¿ESTÁN CONECTADOS A TIERRA Y ALIMENTACIÓN AL BREADBOARD?

Asegúrese de haber conectado correctamente los cables de la tapa de la batería a los buses de alimentación y de tierra en la placa de pruebas, como se muestra en la Figura 3-31. Recuerde: Conecte el cable rojo al bus con la línea roja al lado con un signo más (+) en la parte superior y el cable negro al bus de tierra con una línea verde, azul o negra (dependiendo de su tablero) y un signo menos (-) en la parte superior de la placa.

![03-31](images/03_31.png)

***Figura 3-31***: Conduce desde la tapa de la batería colocada correctamente en los buses de alimentación y de tierra

### ¿ESTÁ ORIENTADO CORRECTAMENTE EL LED?

Verifique para asegurarse de haber colocado el LED correctamente en la placa de pruebas. Recuerde que tiene un cable positivo (ánodo) y un cable negativo (cátodo) y la corriente fluye solo si el LED está orientado correctamente. El cable positivo es más largo que el negativo, como se muestra en la Figura 3-32.

![03-32](images/03_32.png)

***Figura 3-32***: Cables positivo (ánodo) y negativo (cátodo) del LED

### ¿UTILIZÉ LA RESISTENCIA CORRECTA?

A continuación, compruebe si utilizó la resistencia correcta. Discutiremos cómo seleccionar una resistencia en capítulos posteriores, pero si ha usado una con demasiada resistencia, el circuito no tendrá suficiente energía para encenderse. Si usa uno que no tiene suficiente resistencia, puede destruir su LED. Para este circuito, la resistencia debe tener bandas de color naranja, naranja, marrón y dorado (Figura 3-33).

![03-33](images/03_33.png)

***Figura 3-33***: Una resistencia de 330 ohmios

Estos primeros pasos de depuración se basan en una cuidadosa observación y comprensión de los conceptos básicos del circuito que hemos cubierto hasta ahora. Algunos pasos de depuración también dependerán de herramientas para mejorar su conocimiento sobre lo que sucede en el circuito.

### LAZOS DEL CIRCUITO DE DEPURACIÓN: CONTINUIDAD

Quizás el error más común al construir un circuito usando un breadboard es colocar los componentes en los puntos de unión incorrectos en la placa para que no estén conectados. Como ha visto, los circuitos son bucles, y si los componentes no están conectados entre sí correctamente, el bucle se rompe. La continuidad es la propiedad que simplemente significa que las cosas están conectadas, como se muestra en la Figura 3-34.

![03-34](images/03_34.png)

***Figura 3-34***: Componentes que están conectados correctamente y componentes que no están conectados correctamente

Puede comprobar si sus componentes están conectados correctamente mirando de cerca su placa. Verifique cuidadosamente que los cables del LED, la resistencia y el puente estén en las filas correctas de puntos de unión en la placa de pruebas para que estén conectados correctamente.

Hay otra forma de probar la continuidad en un circuito en una placa de pruebas además de inspeccionarlo visualmente: puede probar la continuidad con un multímetro (Figura 3-35).

![03-35](images/03_35.png)

***Figura 3-35***: Un multimetro

> **¿Preguntas?**
> 
> P: ¿Tendré que memorizar los pasos para depurar?
> R: Buena pregunta. No es necesario (ni se espera) que memorice los pasos de depuración. Descubrirá que después de crear los circuitos en el libro, comenzará a recordar los pasos de depuración, ya que los usará con frecuencia. Haremos referencia a los pasos según sea necesario para el resto del libro.

## EL MULTÍMETRO

Otra forma de obtener información sobre sus circuitos es mediante el uso de un multímetro. Un multímetro es una herramienta crítica para verificar que nuestros proyectos electrónicos y Arduino estén funcionando correctamente y que todas nuestras piezas sean funcionales. Su multímetro será una excelente herramienta para usar en todos los proyectos de este libro para asegurarse de que todo funcione como se esperaba. A veces lo llamaremos multímetro y otras veces lo llamaremos medidor. Ahora le mostraremos cómo usarlo para probar la continuidad.

No usará un multímetro con el Arduino aquí, pero lo hará en capítulos futuros. ¿Por qué lo estamos mirando ahora? Le ayudará a depurar su primer circuito y será invaluable más adelante cuando sus proyectos se vuelvan más complejos y aprenda más formas de usarlo. La figura 3-36 muestra algunos multímetros diferentes.

Estamos usando el medidor de SparkFun (número de pieza SparkFun TOL-12966), que mencionamos en la lista de piezas en el Capítulo 1. Los dibujos del multímetro en este libro se basan todos en este modelo. Su medidor puede verse diferente, pero los principios para configurar el medidor y usarlo serán los mismos.

![03-36](images/03_36.png)

***Figura 3-36***: Los multímetros vienen en diferentes tamaños y colores.

### DESCRIPCIÓN GENERAL DEL MULTÍMETRO

La figura 3-37 muestra las partes de un multímetro: una pantalla que muestra el valor de la propiedad eléctrica que está midiendo y un dial que gira para determinar la propiedad eléctrica que está probando. Un extremo de las sondas toca los componentes que está probando en un extremo, mientras que el otro extremo está conectado al medidor en los puertos.

![03-37](images/03_37.png)

***Figura 3-37***: Partes de un multímetro

Algunos medidores tienen botones de apagado/encendido, mientras que este se enciende con el dial.

> **Advertencia**
> 
> Recuerde apagar el medidor cuando haya terminado para que no se agote la batería.

La mayoría de los multímetros funcionan con una batería de 9V. No incluimos instrucciones para insertar la batería en su medidor. Si obtiene este medidor, las instrucciones vendrán con él. Si compró o heredó un medidor diferente, las instrucciones para reemplazar la batería serán diferentes.

### PARTES DEL MULTÍMETRO: EL DIAL

La Figura 3-38 es un detalle del cuadrante de un multímetro típico marcado con algunas de las cantidades eléctricas que puede medir. Explicaremos todos estos símbolos y propiedades a medida que avanzamos en el libro. En este momento, solo sepa que hay diferentes propiedades que puede medir: voltaje de CA, voltaje de CC, resistencia, amperaje de CC y continuidad.

![03-38](images/03_38.png)

***Figura 3-38***: El dial de un multímetro con propiedades eléctricas que puede medir.

Volveremos a estas propiedades eléctricas y cómo medirlas con el medidor en el Capítulo 5, "Electricidad y medición".

### PARTES DEL MULTÍMETRO: LAS SONDAS

La Figura 3-39 muestra las sondas, la parte del multímetro que toca su circuito, componente o lo que sea que esté probando o midiendo. Las puntas metálicas de las sondas se colocan de manera que toquen el circuito o componente. El otro extremo de cada sonda encaja en los puertos del multímetro. Las sondas no se conectarán a los puertos cuando desembale el multímetro.

![03-39](images/03_39.png)

***Figura 3-39***: Sondas del multímetro

### PARTES DEL MULTÍMETRO: LOS PUERTOS

Ahora que hemos visto las sondas del multímetro, echemos un vistazo más de cerca a los puertos del medidor, que se muestran en la Figura 3-40.

Es importante que las sondas se coloquen en los puertos correctos cuando se utiliza un medidor. Para todas las mediciones, la sonda negra se coloca en el puerto COM central. La sonda roja tiene dos puertos diferentes en los que se puede colocar (los exteriores como están marcados). Generalmente, mantener la sonda roja en el puerto de la extrema derecha es una buena práctica.

![03-40](images/03_40.png)

***Figura 3-40***: Los puertos de un multímetro

## 🔋 USANDO EL MULTÍMETRO

La continuidad (Figura 3-41) es una propiedad eléctrica que muestra si existe una conexión entre las partes. Puede utilizar el medidor para probar esta propiedad. Es una buena forma de familiarizarse con las partes de su medidor. ¡Y lo usarás para depurar tu circuito!

![03-41](images/03_41.png)

***Figura 3-41***: Símbolo de continuidad

### CONFIGURACIÓN DEL MEDIDOR PARA PRUEBA DE CONTINUIDAD

Primero, le mostraremos cómo usar el multímetro para probar la conexión eléctrica entre las sondas en el medidor, verificando la "continuidad" entre las sondas (Figura 3-42). Luego pasaremos a probar la continuidad en su circuito.

![03-42](images/03_42.png)

***Figura 3-42***: Multímetro con las sondas tocando

Esta prueba es una buena manera de asegurarse de que su multímetro está funcionando y de familiarizarse con su uso. Si las sondas se tocan, forman un bucle eléctrico completo. La misma prueba se puede utilizar más adelante para comprobar si sus piezas están conectadas correctamente desde una perspectiva eléctrica.

### AJUSTES DEL MEDIDOR PARA PRUEBA DE CONTINUIDAD

Para probar la continuidad, la sonda negra va en el puerto marcado como COM y la sonda roja va en el puerto marcado como mAVΩ, como se ve en la Figura 3-43.

![03-43](images/03_43.png)

***Figura 3-43***: Configuración del puerto del medidor para probar la continuidad

A continuación, mueva el dial para que la perilla apunte hacia el símbolo de continuidad (Figura 3-44).

![03-44](images/03_44.png)

***Figura 3-44***: Gire la perilla al símbolo de continuidad.

### PRUEBA DE CONTINUIDAD

Cuando las sondas toquen los componentes que están conectados, el medidor reproducirá un tono si el medidor está configurado para probar la continuidad. Cuando las sondas están conectadas correctamente a los puertos, si se tocan forman un bucle eléctrico. Está haciendo un circuito con sus sondas para probar la continuidad.

Toque las dos sondas juntas ahora para probar esto, como se muestra en la Figura 3-45. Mientras las sondas se tocan, la pantalla mostrará ".000", aunque puede fluctuar ligeramente. También escuchará un tono que variará en sonido según su medidor. Para la continuidad, los números de la pantalla no son tan importantes como lo serán con las otras propiedades de las que hablaremos más en el Capítulo 5.

![03-45](images/03_45.png)

***Figura 3-45***: El multímetro con las sondas en contacto es una prueba de continuidad.

Cuando las sondas se toquen, como se muestra en la Figura 3-46, ¡debería escuchar un tono!

![03-46](images/03_46.png)

***Figura 3-46***: Las sondas se tocan y suena un tono.

La continuidad ayudará a solucionar problemas en circuitos más complicados al identificar cuándo los componentes no están conectados entre sí o si están conectados en un lugar incorrecto. Le mostraremos de manera más explícita cómo la continuidad puede ayudarlo a resolver problemas en el Capítulo 5.

## VOLVER A DEPURAR NUESTRO CIRCUITO

Volvamos a nuestro circuito básico. Ahora que ha desempaquetado su multímetro y comprende qué es la continuidad, apliquemos las sondas del multímetro a nuestro circuito y echemos un vistazo a nuestros resultados.

### PRUEBA DE CONTINUIDAD EN UN CIRCUITO

Su medidor ya está configurado correctamente para probar la continuidad si acaba de completar el último ejercicio. Los ajustes para el dial y las sondas se muestran en la Figura 3-47. Verifique para asegurarse de que el dial esté configurado en el símbolo de continuidad y que las sondas estén en los puertos correctos.

![03-47](images/03_47.png)

***Figura 3-47***: Configuración del medidor para probar la continuidad

Primero, retire su batería del circuito. Luego, encienda su medidor y coloque las sondas en uno de los cables del resistor y uno de los cables del LED, como se muestra en la Figura 3-48. No importa qué sonda de color toque qué cable.

![03-48](images/03_48.png)

***Figura 3-48***: Probando la continuidad del circuito

Si sus componentes están conectados, volverá a escuchar el zumbido y la configuración en la pantalla leerá .000 con una posible ligera fluctuación.

¿Qué pasa si no oyes ese zumbido? Verifique las conexiones en su breadboard entre cada componente para ver si están en los puntos de unión adecuados.

En la Figura 3-49, el LED no está conectado a ninguno de los otros componentes. La resistencia está conectada al riel de alimentación y el puente está conectado a tierra, pero ninguno está conectado al LED. Para arreglar el circuito, coloque los cables en los puntos de conexión correctos.

![03-49](images/03_49.png)

***Figura 3-49***: El multímetro prueba un circuito donde los componentes no están conectados

> **¿Preguntas?**
> 
> P: ¿Qué pasa con todos esos otros símbolos en el multímetro? ¿Cuándo usaremos el multímetro para medirlos?
> R: Explicaremos más sobre el multímetro y cómo medir las diversas propiedades eléctricas (resistencia, voltaje, corriente) en el Capítulo 5.
>
>P: ¿Qué sucede si mi medidor tiene una lectura diferente a .000 cuando estoy probando la continuidad?
> R: Con el medidor recomendado, lo más importante a lo que debe prestar atención al verificar la continuidad es escuchar el ruido creado por el medidor que indica que sus componentes están conectados eléctricamente. Los medidores sin sonido tendrán otras formas de indicar continuidad en la pantalla de visualización.

## RESUMEN

En este capítulo, aprendió cómo construir un circuito y cómo depurarlo. Le presentaron el multímetro y aprendió a usarlo para verificar si todos sus componentes estaban conectados. En el siguiente capítulo, configurará su Arduino para programarlo y luego lo conectará a una placa de pruebas para comenzar a usar su Arduino para controlar los componentes.

