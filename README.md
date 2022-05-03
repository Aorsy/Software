# Software



# Parte 1:
![image](https://user-images.githubusercontent.com/89556455/166562357-3e9a324b-fd7c-4644-8985-f423239ae252.png)
Idea básica al escribir y enviar un mail:

Escribimos el mail
Apretamos enter para enviar el mail.
2.1. Al apretar enter estamos enviando una señal eléctrica desde el teclado
2.2. Esta señal es enviada a la motherboard, la motherboard la envia al CPU
2.3. La CPU recibe la señal del teclado y la envia al sistema operativo
2.4. El sistema operativo (a través de drivers, que son softwares que interpretan las señales eléctricas de los periféricos) interpreta la señal eléctrica y la envía al navegador (pues sabe que nosotros queriamos enviarla ahí por donde apretamos el enter (mientras estabamos en el navegador)
2.5. Nosotros cuando estamos en una pestaña de chrome en realidad estamos en un html, un html posee uno o varios script, y ahí un script que esta preparado para hacer algo al momento de pulsar la tecla enter (al momento que ocurra el evento “Pulsar tecla enter”), el cual va a hacer pues hemos apretado a tecla enter.
2.6. Javascript entiende que al ocurrir el evento enter tiene que hacer algo con el mail que hemos escrito.
2.6.1. AJAX permite enviar datos al servidor (el mail en este caso) y que la pagina no se recargue. AJAX es un API (interfaz de programación), que, entre sus multiples funciones, encapsula los datos que deseamos enviar de una manera que luego el servidor comprendera. La forma de encapsular los datos se denomina formato. AJAX encapsula el mail en un formato llamado JSON
2.6.2. AJAX envía el mail en formato JSON a través del protocolo REST (es un conjunto de reglas de como se envían los datos a un servidor) a través de HTTP (esta incluido en REST).
2.6.3. HTTP y HTTPS son protocolos de transferencia de texto. HTTPS es más seguro porque permite que solo al servidor al cual estamos enviando los datos pueda interpretar la información, solo el receptor final podrá ver los datos que enviamos. De esta manera se evita que alguien se pueda meter en el medio de al transferencia y ver los datos. Los datos se envían a una dominio DNS, que es la dirección de un servidor
2.7. El servidor recibe los datos en forma de señales eléctricas, el sistema operativo del servidor (en general linux(muerte al capitalismo 😛 )) a través de ethernet, transforma los datos que están encapsulados según el protocolo TCP/IP. Este protocolo luego crea los datos hacia el protocolo HTTP, HTTP es recibido por un servidor de HTTP de linux.
2.8. El servidor HTTP ahora permite que los programas en el backend procesen la información recibida según corresponda. Los datos procesados son guardados en una base de datos para luego poder acceder a estos datos.
2.9. El mail ahora si es enviado al dominio que sigue al @.
2.10. El mail ahora va al servidor de mail del dominio que se envía, este lo envía a la base de datos del mail que corresponde (el que esta previo al @), es decir va a la bandeja del receptor.
2.11. La bandeja del receptor recibe una notificación
2.12. La bandeja envía una notificación a un servidor de notificaciones, el servidor de notificación avisa a nuestro celular que se ha recibido un mail.
El mail fue envía y el receptor fue notificado a su celular.
Más claro échale agua 😛

NOTA: Los DNS es una base de datos que relaciona un nombre con un IP

Cuando los datos viajan por la red para identificar el proceso existe lo que es llamado el modelo OSI que consta de 7 capas:
1.-Fisica
2.-Enlace de Datos
3.-Red
4.-Transporte
5.-Sesión
6.-Presentación
7.-Aplicación

Al realizar la comunicación los datos van subiendo o bajando las capas que los van encapsulando en el protocolo según sea el caso.
La Capa 4 de Transporte utiliza los protocolos TCP y UDP en el que la diferencia es que TCP va orientado a la conexión confiable y la integridad de los datos.

Cuando mandas un correo o una imagen viaja por TCP porque tienen que llegar los bits completos, si algo se pierde en el camino, se vuelve a reenviar el datagrama.
Cuando realizas una videollamada o ves un video en Youtube los datos viajan por UDP ya que si se pierden datos en el camino son casi imperceptibles y estar reenviando los datos por cada error seria mas notable al verse lento un video.

AJAX: Asynchronous Javascript And XML
JSON: Javascript Object Notation
REST: Representational State Transfer
HTTP: Hypertext Transfer Protocol
FTP: File Transfer Protocol
SSH: Secure Shell
DNS: Domain Name System
TCP: Transmission Control Protocol
IP: Internet Protocol
SMTP: Simple Mail Transfer Protocol
POP3: Post Office Protocol
UDP: User Datagram Protocol
SoC: System on a Chip
ASCII: American Standard Code for Information Interchange




¿Qué tienen todos los computadores en común?

Disco Duro: Lo datos se guardan en discos que necesitan girar para ser leídos, hay otras tecnologías más avanzadas como los Discos Flash que no necesitan girar sino se hace a través de señales

RAM: Es un tipo de memoria pero no funciona para guardar datos permanentemente, nos ayuda a gestionar las cosas que necesitan almacenamiento volatil como, cuántas ventanas tenemos abiertas al mismo tiempo, la cantidad de recursos que necesita un programa para fucionar, etc. esos recursos los ofrece la memoria Ram.

CPU - Central Processing Unit: Procesador central (con marcas como Intel, AMD). Para conocer la capacidad de tu CPU te guías por los GHz (velocidad a la que procesan una instrucción) y Cores (# de CPU’s en un mismo chip, cuantas instruccionespueden hacer al mismo tiempo).

BIOS: Chip especial que está instalado en la tarjeta madre, es un sistema operativo de arranque. Cuando arranca intenta detectar todas las cosas que están conectadas a un computador.

Disco Duro: Es dónde se guarda toda la información, es dónde está el sistema operativo.

RAM - Random Access Memory: Es un tipo de intermediario entre el Sistema Operativo que está en el disco duro y el CPU. Es una memora de alta velocidad (memoria volátil), sólo funciona cuando hay electricidad.

Memristor: Pieza electrónica que logra guardar la onda eléctrica que pasa por ella incluso cuando se desconecta. Es posible que sea el reemplazo del disco duro y la memoria RAM en el futuro.

Periféricos: Pantalla, teclado, mouse, puertos, etc.

Drivers: Convierte la interacción de los accesorios periféricos en Bits y Bytes para que el computador pueda entender las instrucciones que les damos a través de ellos.

GPU: Canal de comunicación entre la pantalla y el CPU. Es quién se encarga de mostrar todo en la pantalla, desde que arranca hasta reproducir videos y videojuegos.

el Disco Duro no es un tipo de memoria, es un dispositivo de almacenamiento que usa un tipo de “memoria” que realmente guarda todo de manera magnética, a diferencia de discos basados en EEPROM o flash que son un circuito integrado.

tipos de memoria hay varias

-RAM
-ROM
-PROM
-etc

la RAM no necesariamente es volátil, la RAM volatil es la DRAM la cual necesita constantes ciclos de refresco, como puede estar la SRAM que puede ser no volátil y se usa en memoria como la cache.

Aspectos importantes a tener en cuenta de la clase:
Discos duros:

Forma en que organizan datos:

Persistente
Secuencial
Estructurada (Depende del sistema de archivos, que a su vez depende del S.O. que esté en el disco duro):
Windows: FAT16 - FAT32, NTFS
Linux: Ext3 - Ext4
Mac OS: HFS, APFS
Forma de localizar y leer archivos:
En la parte superior de los Discos Duros existe una cabecera, la cual guarda el indice de todos los archivos, esto permite que en el momento de lectura desde la cabecera, se conozca en dónde está ubicado el archivo en cuestión.

Borrado de archivos:
Por tal motivo, cuando se “borra” un archivo, lo que realmente se esta haciendo es eliminando el indice en la cabecera que está relacionado con el archivo. Determinados tipos de software permiten la recuperación de estos archivos, leyendo detalladamente toodo el disco duro. Sin embargo algunas practicas de borrado (Sheredder) permiten borrar el archivo por completo, incluso ejecutando el borrado determinado número de repeticiones, lo que imposibilita el trabajo de forenses para la recuperación de datos o archivos.

Memoria RAM (Random access memory)

Procesos:
La memoria RAM, siendo tan rápida, tiene la capacidad de ejecutar varios procesos paralelamente. El SO es uno de esos procesos ejecutados por la RAM. Sin embargo la opciones que nos ofrece el SO son muchas y no siempre se utilizan todas, por lo tanto la RAM solo carga aquellas tareas que realmente necesitamos y estamos usando frecuentemente.

Localización de procesos:
A diferencia de los discos duros, la memoria RAM hace uso de un indice compartido con la CPU que es ultra veloz. Esto facilita y permite una localización de los procesos por parte de la CPU de una manera increíblemente rápida.

CPU (Central process unit):

Dentro de este asombroso chip, no encontramos con un espacio que recibe por nombre Memoria Caché. En ella se guardan y almacenan cierto tipo de datos de uso frecuente, para que sea más fácil y rápido el acceso a ellos. Por ejemplo una parte del SO siempre estará almacenada en la Memoria Caché para que sea rápido acceder a él.

Comunicación:

Ram:
Para lograr la efectiva comunicación entre la CPU y la RAM existe lo que se conoce como un bus de datos o bridge (puente). Un bus de datos en algunas ocaciones es un cable delgado y ancho. En otros casos esta conexión está establecida como circuito en la placa madre (mother board).
Disco Duro:
Para la conexión entre en disco duro y la CPU, el bus de datos recibió inicialmente el nombre ATA, que en una versión posterior se llamó SATA. Hay otro tipo de bus de datos para el disco duro mejor que SATA, que se llamó IDG.
