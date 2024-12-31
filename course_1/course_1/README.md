# Fundamentos de Internet

## Introducción

En este curso el alumno conocerá los principios básicos del funcionamiento de internet y de la WWW.

Se profundizará en los protocolos de comunicación más usados, los principales navegadores y su funcionamiento. Nos adentraremos en la terminología y los elementos que conforman el entramado de las transferencias de datos entre computadoras. Conceptos como nodo, paquetes, puertos, latencia, etc...Sabremos cómo funcionan las redes de intercambio de información, los tipos de redes más usados, los componentes físicos y lógicos que conforman una red.Hablaremos de los protocolos de transferencia y de cómo funciona realmente internet.Qué es el HTTP. La comunicación cliente-servidor, las DNS, las direcciones IP.Se describirán las herramientas que posibilitan que una página WEB sea visible. Los tipos de hosting, alojamiento, dominios y los diferentes navegadores existentes y su funcionamiento.

Al final del curso el alumno tendrá una idea clara del entramado de elementos que han posibilitado que internet sea la red de intercambio de información que ha cambiado nuestro mundo.

### Contenidos

1. ¿Cómo funciona internet?
2. ¿Que es HTTP?
3. Los navegadores y su funcionamiento
4. El DNS y su funcionamiento
5. ¿Qué es el nombre de dominio?
6. ¿Qué es el alojamiento web?


## Desarrollo

### 1. ¿Cómo funciona internet?

Las redes son la tecnología que permite que las computadoras se comuniquen entre sí, es decir, que puedan enviar y recibir datos entre ellas. Gracias a las redes existe casi todo lo que conocemos de la tecnología actual como internet, podemos usar las redes sociales, trabajar de manera remota, hacer videoconferencias etc. 

Las posibles aplicaciones son enormes, por ejemplo: si trabajamos en cloud computing, entender cómo funcionan las redes de servidores es importantísimo; si somos programadores, nos va a permitir entender mejor el funcionamiento de las aplicaciones de red o de las aplicaciones web. 

Internet es la red más grande que hay. Es global y descentralizada, es decir, no hay un dueño o empresa que pueda manejarla; no hay un aparato que se desenchufe y todo el mundo se quede sin internet, es imposible; podrían fallar algunos aparatos y dejar sin internet a cierta zona geográfica (una ciudad o un país a lo sumo), pero no hay una forma para que internet se desconecte totalmente, porque es descentralizado, son redes que se conectan entre ellas alrededor del mundo.

#### Algunos términos que debemos tener en cuenta

Los términos que deben sonarnos familiares del mundo de las redes son:

1. Protocolos

Son el conjunto de reglas que las computadoras deben seguir y respetar para poder comunicarse, por ejemplo: si yo hablo español e intento conversar con alguien que habla chino, no va a poder establecerse una comunicación fluída; de la misma manera, si las computadoras no respetan los mismos protocolos, no podrían comunicarse.

Existen diversos protocolos en función del tipo de comunicación que se establece entre las máquinas:

- **FTP**: Para la transferencia de ficheros
- **POP y SMTP**: Para el envío y recepción de correo electrónico
- **TELNET**: Para la conexión con terminales remotos
- **GOPHER, WAIS y HTTP**: Para el acceso a servidores de información

El **protocolo HTTP** (HyperText Transfer Protocol) es la base de la World Wide Web o telaraña mundial, abreviada WWW y más conocida como Web.

2. Paquetes

**Los paquetes son los trozos en los que se dividen los datos para ser enviados.**

Si quisiéramos enviar un gigabyte de datos, no vamos a enviarlo de golpe; los dispositivos de red lo dividen en paquetes para poder enviarlo y hacerle seguimiento, es decir, saber si llegaron correctamente, si hay que reintentar el envío, si llegaron en el orden correcto, etc.

3. Nodo

**Un nodo es una computadora conectada a una red.**

Tenemos computadoras y tenemos dispositivos de red, que son los que le permiten la comunicación, entonces, cada computadora conectada a una red se conoce como nodo.

4. Puertos

Son las interfaces que permiten la conexión. Hay de dos tipos:

- **Los puertos físicos**: son los puertos donde conectas el cable o la antena que permite conectarse a una red inalámbrica.

- **Los puertos lógicos**: si nosotros tuviéramos una sola conexión física (por ejemplo: un cable conectado a la computadora) no podríamos navegar por internet y a la vez escuchar una canción por Spotify o visualizar un video por Youtube, porque necesitaríamos dos conexiones. Los puertos lógicos son los que nos permiten a través de una sola conexión física, abrir varias conexiones simultáneamente.

5. Latencia

**Es el tiempo que demora en llegar un paquete hasta su destino**. 

Por ejemplo: si nos conectamos a una página web que está en Rusia, nuestra petición va a tardar cierto tiempo en llegar a su servidor de destino y este servidor va a responder a nuestra solicitud enviándonos la página web. Otro ejemplo podría ser: cuando hacemos streaming, hay un tiempo de demora entre el emisor y los posibles receptores, esa es la latencia y va a depender de muchos factores, porque no es igual para todos receptores, algunos tendrán mejor conexión a internet que otros. 

En otras palabras: a menor latencia mayor velocidad de conexión.

6. LAN (Local Area Network)

Es una red de área local, la más básica que vamos a aprender, es una red en una casa o en una oficina, interconectada en un pequeño espacio geográfico. Normalmente usando una conexión por cable de red.

7. WLAN (Wireless Local Area Network)

Es lo mismo que LAN, pero conectada a través de redes wifi (redes inalámbricas).

8. WAN (Wide Area Network)

Si tenemos una LAN A y una LAN B y queremos conectar las dos, necesitaremos routers. Los routers nos permiten hacer el enrutamiento entre dos redes locales. Si sumamos tres, cuatro, cinco, seis o más redes, ya estamos en el concepto de WAN. Técnicamente hablando, internet es una WAN. Cuando nuestro proveedor de internet viene a nuestra casa, nos instala el cableado y un router, nos está conectado a internet y está haciendo que nuestra red local (la de nuestra casa) entre a una WAN.

9. VLAN (Virtual Local Area Network)

Es una red de área local, pero virtual, es decir, a través de los dispositivos de red podemos crear credes lógicas o redes virtuales.

#### ¿Cómo funcionan las redes?

Las redes funcionan en dos niveles, un nivel físico y un nivel lógico.

1. Nivel físico:

- Hosts: Son todos los dispositivos con los que el usuario interactúa, por ejemplo: computadoras, impresoras, teléfonos, servidores, etc.

- Dispositivos de red: Son los que permiten la conexión, por ejemplo: switches, routers, access point, antenas, etc.

- Adaptadores de red: Son dispositivos que están dentro de los hosts y permiten que ellos se conecten a la red. Un adaptador de red traduce la señal eléctrica si es cableado, o inalámbrica si nos conectamos a un wifi y la traduce a un tipo de señal que la computadora puede procesar.

- IOT: Internet of things (el internet de las cosas). Vivimos en una época en la cual disponemos de una infinita de dispositivos y electrodomésticos que pueden conectarse a internet, eso se llama IoT o internet de las cosas, cada dispositivo tendría un adaptador que le permitiría conectarse con el mundo.

2. Nivel lógico:

Por este lado tenemos el tema de los protocolos y del software.

- Protocolos: Como dijimos anteriormente, son el conjunto de reglas que tienen que seguir los dispositivos para conectarse a la red.

- Software: Es aquel que ya viene ya viene integrado en los mismos dispositivos de red, por ejemplo: un router viene con su propio sistema operativo y se puede configurar según las necesidades.

#### Funcionamiento de la web

La Web funciona siguiendo el denominado modelo cliente-servidor, habitual en las aplicaciones que funcionan en una red.

Existe un servidor, que es quien presta el servicio, y un cliente, que es quien lo recibe.

- Cliente web

El cliente web es un programa con el que el usuario interactúa para solicitar a un servidor web el envío de páginas de información. 

Estas páginas se transfieren mediante el protocolo HTTP. 

Las páginas que se reciben son documentos de texto codificados en lenguaje HTML. El cliente web debe interpretar estos documentos para mostrárselos al usuario en el formato adecuado. 

Además, cuando lo que se recibe no es un documento de texto, sino un objeto multimedia (vídeo, sonido, etc.) no reconocido por el cliente web, éste debe activar una aplicación externa capaz de gestionarlo, como Chrome, Netscape Navigator, Microsoft Internet Explorer…etc. 

La mayoría de ellos soportan también otros protocolos, como, por ejemplo:

- 


### 2. ¿Que es HTTP?

### 3. Los navegadores y su funcionamiento

### 4. El DNS y su funcionamiento

### 5. ¿Qué es el nombre de dominio?

### 6. ¿Qué es el alojamiento web?


