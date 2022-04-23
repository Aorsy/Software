# Software

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
