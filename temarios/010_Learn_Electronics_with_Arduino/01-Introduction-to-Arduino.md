# Chapter 1: Introduction to Arduino

* Physical Computing
* Prototyping
* What Will I Need and Where Can I Get It?
* Parts and Tools
* Resources
* Summary

Quizás haya visto el Arduino en un minorista local, escuchado sobre él de un amigo que compró uno, o simplemente vio un proyecto genial en Internet que despertó su interés. ¿Qué es el Arduino? De manera más simple, es una computadora simple, asequible y de pequeña escala que se enfoca en la interacción con el mundo exterior (Figura 1-1).

La mayoría de las computadoras con las que está familiarizado se controlan casi exclusivamente a través del teclado y el mouse, la pantalla táctil o el panel táctil. Un Arduino le permite tomar información del mundo exterior con sensores que miden la temperatura, los niveles de luz y sonido, o incluso las vibraciones debajo de sus pies, y convierten estas medidas en movimiento, sonido, luz y más.

![01-01](images/01_01.png)

***Figura 1-1***: El logotipo de Arduino

El Arduino fue desarrollado originalmente por profesores para que sus estudiantes de diseño que no eran ingenieros pudieran crear objetos y entornos interactivos. Desde que se lanzó el Arduino original en 2005, se estima que se han vendido más de 1 millón. Diseñadores, educadores, ingenieros, aficionados y estudiantes han construido todo tipo de proyectos que sienten y responden al mundo con Arduino.

Hay muchas versiones de Arduino y cada una está diseñada para una función específica. La Figura 1-2 muestra algunas de las placas Arduino.

Hemos escrito este libro en el espíritu del equipo de Arduino. No asumimos que ya sabe programación o electrónica; le mostraremos lo que necesita saber para comenzar a utilizar Arduino. Te ayudará si eres bueno construyendo y retocando, y tienes una naturaleza determinada.

![01-02](images/01_02.png)

***Figura 1-2***: Hay muchas versiones de Arduino, cada una diseñada para una función diferente.

## COMPUTACION FISICA

El Arduino se utiliza para construir proyectos de computación física. ¿Qué significa eso? La computación física se refiere a tomar información del mundo que nos rodea mediante el uso de entradas como sensores e interruptores y responder a esa información con salidas de algún tipo. Podría ser tan simple como encender un LED cuando una habitación se oscurece, o podría ser un sistema complejo de sonido y luz que responde a la posición de una persona en una habitación. Un Arduino puede actuar como el "cerebro" de este tipo de sistema, manejando la información que ingresa y la respuesta que sale.

El Arduino es parte del movimiento de hardware de código abierto. Veamos lo que eso significa.

### ¿QUÉ ES EL HARDWARE DE CÓDIGO ABIERTO?

El Arduino se define en su sitio web como una plataforma de creación de prototipos de electrónica de código abierto. En el movimiento del hardware de código abierto, los tecnólogos comparten su hardware y software para fomentar el desarrollo de nuevos proyectos e ideas. Los diseños de origen se comparten en un formato que puede modificarse y, siempre que sea posible, se utilizan materiales fácilmente disponibles y herramientas de código abierto para crear los diseños.

Al fomentar el intercambio de recursos, el movimiento de hardware de código abierto facilita el desarrollo de nuevos productos y diseños. Los proyectos de código abierto enfatizan la importancia de la documentación y el intercambio, lo que hace que la comunidad de usuarios sea un gran recurso para los estudiantes.

## PROTOTIPOS

El Arduino es una plataforma de creación de prototipos. ¿Qué es la creación de prototipos? Está construyendo un modelo de sistema. Puede involucrar muchas fases, desde bocetos iniciales a través de planos detallados y una serie de refinamientos, hasta la construcción de un modelo completamente funcional que se puede replicar. O puede ser algo único y rápido que se ensambla rápidamente para probar una idea.

## ¿QUÉ NECESITARÉ Y DÓNDE PUEDO CONSEGUIRLO?

Hay varias versiones de Arduino; existe desde 2005 y está en constante evolución. A los efectos de este libro, nos ocupamos del Arduino Uno. Es posible que su Arduino no se vea exactamente como el Uno que se muestra en la Figura 1-3, porque hemos simplificado el dibujo para señalar las secciones que nos conciernen. Dado que Arduino es de código abierto, también puede comprar una placa que no provenga directamente de la organización Arduino. Solo sepa que para este libro nos enfocamos en Arduino Uno y placas compatibles.

![01-03](images/01_03.png)

***Figura 1-3***: Arduino Uno

## PIEZAS Y HERRAMIENTAS

También necesitaremos algunas partes electrónicas adicionales y algunas herramientas para construir proyectos con Arduino. Aquí hay una lista de las piezas que necesitará comprar para completar los proyectos de este libro. Le brindaremos más detalles sobre las piezas y lo que hacen a medida que construimos cada proyecto.

### LISTA DE PARTES

* Proto-board
* Cable USB A-B 
* Batería de 9 voltios
* Fuente de alimentación de 9 a 12 voltios
* Tapa o soporte para batería de 9 voltios
* LEDs surtidos, una variedad de colores
* Resistencias surtidas
* Potenciómetro de 10K
* 3 switches/buttons (interruptores/botones momentáneos)
* Photoresistor (Fotorresistencia)
* Speaker, 8 ohm (Altavoz, 8 ohmios)
* 2 servo motors (2 servomotores)
* Jumper wires (Cables de puente)


Las siguientes figuras, de la Figura 1-4 a la Figura 1-16, le muestran el aspecto de las piezas, junto con una breve descripción. Las partes electrónicas a menudo se denominan componentes porque son componentes de un circuito electrónico. Aprenderá más sobre circuitos en el Capítulo 3, "Conozca el circuito".

Una breadboard, que se muestra en la Figura 1-4, se usa para construir y probar circuitos rápidamente. Un cable USB A-B, que se muestra en la Figura 1-5, conecta el Arduino a una computadora para que pueda programarlo. También proporcionará energía. Una batería de 9 voltios, que se muestra en la Figura 1-6, puede proporcionar energía cuando el Arduino no está conectado a una computadora.

![01-04](images/01_04.png)

***Figura 1-4***: Breadboard

![01-05](images/01_05.png)

***Figura 1-5***: Cable USB A-B 

![01-06](images/01_06.png)

***Figura 1-6***: Batería de 9 voltios

![01-07](images/01_07.png)

***Figura 1-7***: Tapa de la batería

La tapa de la batería, que se muestra en la Figura 1-7, se utilizará para conectar una batería a una placa de pruebas. El adaptador de corriente, que se muestra en la Figura 1-8, puede alimentar su Arduino cuando no está conectado a su computadora. Los diodos emisores de luz (LED), que se muestran en la Figura 1-9, emiten luz cuando se aplica un voltaje.


![01-08](images/01_08.png)

***Figura 1-8***: Adaptador de corriente

![01-09](images/01_09.png)

***Figura 1-9***: LEDs

Las resistencias, como puede ver en la Figura 1-10, limitan el flujo de corriente en un circuito. Usaremos un botón pulsador momentáneo (momentary pushbutton), que se muestra en la Figura 1-11, para hacer o romper una conexión en un circuito. La figura 1-12 muestra un potenciómetro, una resistencia variable.

![01-10](images/01_10.png)

***Figura 1-10***: Resistencias

![01-11](images/01_11.png)

***Figura 1-11***: Botón pulsador momentáneo (momentary pushbutton)

![01-12](images/01_12.png)

***Figura 1-12***: Potenciómetro

Una photoresistor, que se muestra en la Figura 1-13, cambia su resistencia cuando se expone a diferentes niveles de luz. La Figura 1-14 muestra un altavoz de 8 ohmios, que reproducirá señales de audio. El servomotor es un motor de pasatiempo que se controla fácilmente, como puede ver en la Figura 1-15. Los cables de puente, que se muestran en la Figura 1-16, se utilizan para conectar componentes en una placa de pruebas. Puedes comprarlos o hacerlos tú mismo con pelacables.

![01-13](images/01_13.png)

***Figura 1-13***: Photoresistor (photoresistencia)

![01-14](images/01_14.png)

***Figura 1-14***: Speaker, 8 ohm(altavoz de 8 ohmios)

![01-15](images/01_15.png)

***Figura 1-15***: Servo motor

![01-16](images/01_16.png)

***Figura 1-16***: Jumper wires

### UNA NOTA SOBRE LOS LEDs

Los LEDs vienen en una variedad de colores, estilos y tamaños. Usaremos LED en muchos de los proyectos de este libro porque ayudan a demostrar una serie de conceptos básicos de electrónica y Arduino de forma visual.

Una cosa importante para recordar acerca de los LED es que tienen una polaridad o dirección en la que deben colocarse para que funcionen en un proyecto. Si colocamos los LED al revés, no se encenderán. ¿Cómo sabemos la orientación de un LED?

Los LED tienen dos patas, o cables, que tienen diferentes longitudes, como puede ver en la Figura 1-17. El cable más largo se conoce como **ánodo**, el lado del LED que conectaremos a la alimentación. La pierna más corta se llama **cátodo**, que apuntará en dirección opuesta a nuestra fuente de energía. Le mostraremos cómo colocar los cables en un circuito cuando comencemos a construir uno, y siempre le recordaremos la polaridad en circuitos posteriores.

> **Nota**
> 
> Si coloca el LED al revés, no se encenderá, pero tampoco dañará nada en su proyecto.

![01-17](images/01_17.png)

***Figura 1-17***: Ánodo (cable positivo) y cátodo (cable negativo) de un LED

¿Qué sucede si tiene un LED usado que tiene cables recortados? En muchos LED, si siente la bombilla, un lado del borde en la parte inferior de la bombilla se siente más plano. El cable conectado a ese lado es el cátodo o lado negativo.

Ahora echemos un vistazo a algunas herramientas que necesitará para realizar estos proyectos.

### HERRAMIENTAS

Un multímetro le dirá todo lo que necesita saber sobre las propiedades eléctricas de un circuito, propiedades que no son necesariamente visibles para su ojo. Le mostraremos cómo usarlo, comenzando en el Capítulo 2. El multímetro que se muestra en la Figura 1-18 está disponible en [SparkFun](https://www.sparkfun.com/) (número de pieza TOL-12966), pero puede encontrar otro que le guste. Cuando elija un multímetro, asegúrese de que sea digital y tenga cables extraíbles y de que esté fusionado.

![01-18](images/01_18.png)

***Figura 1-18***: Multimetro

Los alicates de punta fina, como se muestra en la Figura 1-19, son útiles para sacar componentes de la placa de pruebas cuando desee realizar cambios en un circuito. También son útiles para recoger componentes pequeños.

Los pelacables, ilustrados en la Figura 1-20, se utilizan para quitar el revestimiento aislante de plástico que se encuentra en varios grosores de alambre. Te harán la vida mucho más fácil cuando uses carretes de alambre, ya que podrás cortar y usar longitudes de alambre personalizadas.

![01-19](images/01_19.png)

***Figura 1-19***: Pinzas de punta de aguja

![01-20](images/01_20.png)

***Figura 1-20***: Pelacables

> **Tip**
> 
> Aunque puede comprar cables de puente precortados, recuerde que puede crear los suyos propios utilizando sus pelacables para quitar el recubrimiento de plástico en los extremos de un segmento de cable. El cable de conexión de calibre veintidós funciona bien en las placas de prueba.

### UNA PALABRA SOBRE HERRAMIENTAS: EL HIERRO DE SOLDADURA

Es posible que esté familiarizado con un soldador y su uso en electrónica para conectar componentes. En este libro hemos optado por utilizar una placa de pruebas para realizar conexiones en todos los circuitos enumerados. Esto significa que no es necesario que compre un soldador ni que aprenda a usar uno para completar los proyectos de este libro.

> **¿Preguntas?**
> 
> P: ¿Qué hace un soldador?
> R: Se utiliza un soldador para fundir un material conductor ("soldadura") para combinar componentes eléctricos de forma permanente. Este proceso se llama soldadura.
> 
> P: ¿Por qué no enseña a soldar en este libro?
> R: Soldar es una habilidad maravillosa y te ayudará a llevar tus dispositivos electrónicos al siguiente nivel, pero en este libro nos preocupamos principalmente por los conceptos básicos. Puede hacer circuitos completamente funcionales sin él.
> 
> P: La lista de componentes parece tener muchas partes. Las imágenes se ven bien, pero ¿realmente necesito comprar todos los elementos de esa lista?
> R: ¡Verás muchas más de esas fotos! Para responder a su pregunta, utilizará todas esas partes cuando cree los proyectos de este libro. Estas piezas también se pueden reutilizar para sus propios proyectos. Explicaremos qué hacen todas estas partes a medida que las usamos.
> 
> P: Mi amigo/hermano/padre/maestro/perro me dio un modelo más nuevo/antiguo de Arduino. ¿Tengo que usar Arduino Uno para los proyectos de este libro?
> R: Buena pregunta. Los proyectos en el libro pueden funcionar con su Arduino particular, pero tanto la programación como las habilidades del Arduino han cambiado con el tiempo y difieren según la versión. Todos los ejemplos de este libro se han probado con Arduino Uno y la última versión del software Arduino.
> 
> P: No reconozco ni sé cómo utilizar ninguna de las herramientas o componentes que me ha mostrado; ¿hay otro libro para mí?
> R: ¡No! Este libro está escrito para ti. Cubriremos detalles específicos sobre cómo usar todas las piezas y herramientas que hemos enumerado en los próximos capítulos. Siéntese tranquilo y siga leyendo.
> 
> P: No tengo ningún lugar en mi vecindario para comprar esas piezas. ¿Tiene alguna recomendación de lugares en los que pueda encontrar esas piezas en línea?
> R: ¡Gran pregunta! Estás listo para la siguiente sección.

## RECURSOS

Varios proveedores venden los componentes que necesitará. Aquí están las URL de los sitios web de muchos de ellos, y puede haber tiendas físicas u otros recursos en su comunidad.

### Maker Shed ([makershed.com](https://www.makershed.com/))

Selección de kits y componentes individuales de Arduino. Algunas partes electrónicas, enfocadas a la comunidad Maker.

### SparkFun Electronics ([sparkfun.com](https://www.sparkfun.com/))

Amplia gama de sensores y placas de conexión, Arduinos clásicos y su versión casera.

### Adafruit Industries ([adafruit.com](https://www.adafruit.com/))

Arduinos y placas de conexión, sensores, componentes electrónicos.

### Jameco Electronics ([jameco.com](https://www.jameco.com/))

Principalmente componentes electrónicos, botones e interruptores sin fin.

### Mouser Electronics ([mouser.com](https://www.mouser.es/))

Algunos Arduino, toneladas de electrónica, sensores y otros elementos.

### Digi-Key Electronics ([digikey.com](https://www.digikey.com/))

Ideal para pedir componentes, chips, etc.

### Micro Center ([microcenter.com](https://www.microcenter.com/))

Una fuente de componentes y Arduinos, tienen algunas tiendas físicas, así como un sitio web.

### KITS

Los kits están disponibles de algunos de los proveedores mencionados aquí que tienen la mayoría de las piezas que necesitará para completar los proyectos. Revisaremos exactamente lo que necesita para construir los proyectos en cada capítulo. Estos son algunos de los kits disponibles; encontrará que hay muchos más.

* Un kit desarrollado por el equipo de Arduino (https://store.arduino.cc/genuino-starter-kit). Puede adquirirse de varios proveedores.
* Este kit está disponible en Maker Shed https://www.makershed.com/collections/make-kit
* Adafruit Industries tiene algunos kits, incluido este: https://www.adafruit.com/product/193

## RESUMEN

Este capítulo lo puso en el camino para usar su Arduino. A estas alturas ya sabe dónde obtener los elementos necesarios, puede identificar varios componentes y herramientas que utilizará, y sabe algo sobre las contribuciones del movimiento de código abierto.

El siguiente capítulo analizará el Arduino Uno con más detalle y le mostrará cómo conectarlo a su computadora.
