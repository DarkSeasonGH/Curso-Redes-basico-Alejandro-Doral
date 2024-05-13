# Curso-Redes-basico-Alejandro-Doral
He hecho un curso basico en obsidian que trata sobre redes, protocolos, dispositivos... etc. Aqui esta el enlace: obsidian://open?vault=Obsidian%20Vault&amp;file=Redes%2FCurso%20redes%20Alejandro%20Doral



Si no os funciona el enlace os dejo el texto aqui:
Cuando hablamos de redes nos referimos a un conjunto de equipos conectados entre si, se conectan entre si para compartir informacion, recursos o servicios.
Para esta comunicacion hacen falta distintos protocolos para que la comunicacion tenga sentido.

Tipos de comunicacion:
-Unicast: En una comunicacion unicast un unico dispositivo fuente envia datos a otro dispositivo destino.
-Multicast: En una comunicacion multicast un dispositivo fuente envia datos a un grupo de dispositivos destino.
-Broadcast: En una comunicacion broadcast un unico dispositivo fuente envia datos a todos los dispositivos que esten en la misma red.
-Anycast: Se refiere a cuando se envia un paquete a una red en la que varios servidores tienen la misma direccion ip.

-Protocolo TCP/IP: Protocolo de red que permite la transmision de datos entre computadoras, contiene todas las reglas que deben seguir las computadoras para poder comunicarse.

-ICMP, o Protocolo de Mensajes de Control de Internet (Internet Control Message Protocol, en inglés), es un protocolo fundamental en el conjunto de protocolos de Internet (TCP/IP). ICMP se utiliza principalmente para la comunicación entre dispositivos de red para realizar funciones de diagnóstico y control.

-FTP: Es un protocolo estandar de internet utilizado para la transferencia de archivos entre dos computadoras mediante el protocolo TCP/IP

-SSH: Para controlar un dispositivo por control remoto.

DHCP: Protocolo para que un router reparta distintas direcciones ip a los dispositivos conectados en la red.

Existen diferentes organizaciones como IANA para mejorar estos protocolos y que cada vez haya menos problemas en la comunicacion.

Arpanet: Fue una red de compuptadoras creada en Estados Unidos en 1960 por el ministero de defensa para poder enviar recursos informaticos. Fue la columna vertebral del actual internet. Muchos de los protocolos que hay ahora se desarrollaron en Arpanet.

Internet: Conjunto de redes descentralizadas interconectadas que utilizan los protocolos TCP/IP para conectar los distintos dispositivos entre si y poder establecer una comunicacion a distancia.

Distintos tipos de redes:
-Red LAN: Una red local como puede ser una computadora conectada a otra, o un conjunto de ordenadores conectados a un mismo router.
-Red MAN: Conjunto de redes muy extenso que puede abarcar un pais o una ciudad.
-Red WAN: Son redes de computadoras que abarcan un area geografica extensa. Las redes WAN conectan distintos dispositivos por todo el mundo.
-Red PAN: Red para area personal, no tienen mucho alcance asi que requieren cercania, pero eso proporciona mas seguridad y privacidad.

El modelo OSI (Open Systems Interconnection) es un marco conceptual que describe las funciones de comunicación de un sistema de red. Tiene siete capas en total, cada una de ellas usa los servicios de la capa inferior y proporciona servicios a su capa superior. Estas son las siete:  
- **Capa de aplicación:** Proporciona servicios de red a las aplicaciones de usuario final, como correo electrónico y navegadores web.
    
- **Capa de presentación:** Se encarga de la representación y traducción de datos, incluyendo la encriptación y la compresión.
    
- **Capa de sesión:** Establece, administra y finaliza las conexiones de sesión entre dispositivos en una red.
    
- **Capa de transporte:** Ofrece la entrega de datos extremo a extremo, garantizando la fiabilidad y el orden de los datos transmitidos.
    
- **Capa de red:** Se encarga del enrutamiento de datos y del direccionamiento lógico de los dispositivos en la red.
    
- **Capa de enlace de datos:** Proporciona transferencia de datos confiable entre dispositivos conectados en la misma red local.
    
- **Capa física:** Se encarga de la transmisión física de datos a través del medio de transmisión, como cables o ondas de radio

Normas ASI/EIA/TIA: son los estandares, normas establecidas por las industrias de las comunicaciones y la electronica que sirven para estructurar cableado e instalar equipos electronicos. Fueron creados para garantizar la calidad y la seguridad de de productos y sistemas de telecomunicaciones.

Cableado estructurado
Con esto nos referimos a la distribucion de un cableado en el interior de un edificio para poder establecer una red de area local que pueda ser entendido por tecnicos y administradores de la red.
Con esto conseguimos una conexion con escabilidad, tolerancia a fallas y rendimiento optimo.

Elementos de cableado estructurado:
-Area de trabajo:Lugar donde los operarios van a estar trabajando.
Un terminal rj45 es un conector que se instala en la pared y proporciona un punto de conexion para cables Ethernet.
Un patch panel es un dispositivo de red que se utiliza para organizar y gestionar los cables de red. Va asociado con un rj45
En las areas de trabajo normalmente se suelen conectar los ordenadores al switch y del switch al router pero aqui hay una manera mejor de hacerlo:
Conectar del ordenador al terminal rj45, del terminal rj45 al patch panel, del patch panel al switch y del switch al router. Con esto conseguimos que el cableado sea menos probable de que se rompa y proporciona mas seguridad a la transmision de datos.

-Cable horizontal: En todas las oficinas se usan el cable ethernet. Tambien es conocido como el cable utp, es un cable de ocho hilos presentados en 4 pares trenzados. Existen varias categorias de este cable y se recomiendan la 5 o la 6 y es lo optimo para la capacidad de transferencia. Este cable debe de estar lejos de la corriente electrica y de fuentes que generen campos electromagneticos.

El area de trabajo es el que va desde el ordenador hasta el terminal rj45.
El cableado horizontal es lo que se denomina lo que va desde el terminal hasta el switch.
Este cableado debe de estar protegido por estructuras como bandejas y debe de estar bien organizado, se puede utilizar de guia las normas como ASI/EIA/TIA que propocionan informacion sobre esto. Este cableado termina en el switch.

IDF: un armario para meter routers switch y mas dispositivos de red. esto mantiene todo ventilado y organizado.

El cableado antes de conectarse al switch deberia de conectarse al patch panel. Protege los puertos del switch y es mas seguro. El cableado horizontal no debe de superar los 100 metros de longitud.

La atenuación de la señal se refiere a la disminución de la intensidad de una señal mientras viaja a través de un medio de transmisión, como un cable de red o una fibra óptica. Este fenómeno ocurre debido a varios factores, como la resistencia eléctrica del medio, la distancia recorrida, las interferencias electromagnéticas y la calidad del cableado.

-Cableado vertical
A todos los idf que estan conectados al mdf se le conoce como cableado vertical
MDF: es como un idf grande, todos los IDF se conectan al MDF, que es el centro de distribucion, en el suelen estar los servidores importantes.
En el MDF se encuentran tres cosas: Routers o switch multicapa(capa 3) los servidores y los POP
POP:es un lugar fisico que permite conectarse desde la calle hasta el edificio para brindar red

Se utilizan modelos teoricos de referencia para entender mejor como funciona la comunicacion separandola en capas, esto es lo que hace el modelo osi. Se divide en 7 capas y en cada una de ella hay dispositivos protocolos y tecnologia distinta.

Ethernet: es un estandar de redes de area local para computadoras. Define caracteristicas del cableado y tramas de datos y de enlace en el modelo osi.

Direccion Mac: Identificador de 48 bits de una tarjeta red de un dispositivo, viene por defecto del fabricante y no puede repetirse. Se la conoce tambien como direcion fisica.

NIC: es la tarjeta red de un dispositivo que permite conectarse a internet. Puede ser con un usb, una tarjeta dentro del dispositivo, inalambrico, alambrico... etc. Todas ellas vienen de fabrica con una direccion MAC que suele venir escrita en la etiqueta de la tarjeta.

Una direccion MAC se veria asi: 00:1e:c2:9e:28:6b
00:1e: Nos dice que pertenece al fabricante Apple
c2:9e:28:6b: el modelo del dispositivo

Podemos ver una direccion MAC yendo al CMD de Windows y escribiendo: ipconfig /all. Nos puede aparecer como Physical Address, que significa direccion fisica.

El encapsulamiento de datos es esencial para la comunicacion de los equipos.

Ethernet es la unidad de comunicacion en una red lan y es lo que envian y reciben los equipos para conectarse entre si. Si se quiere una red por cable se necesita un switch.

El switch utiliza una tabla conocida como CAM donde registra la mac que se encuentra en cada puerto conectada. Es decir todos los dispositivos que esten conectados al switch quedan registrados en la tabla CAM.

Direccion MAC origen: Si no existe mac agrega a la tabla la trama teniendo en cuenta el puerto por el que ingresó. Si existe: actualiza el tempporizador o el puerto si es que cambio.

Direccion MAC destino: Si no existe: envia la trama por todos los puertos menos el de la entrada.
Si existe: envia la trama por el puerto asociado.

Cuando ya tiene registrados todos los dispositivos conectados a cada puerto le resulta mas facil trabajar con la tabla CAM y de manera mas directa.

En una red local LAN no es necesaria la ip 100%, esta bien como identificador pero realmente lo que se necesita es la MAC. La ip si que es obligatoria para conectarse con dispositivos fuera de una red local.

Un equipo conectado a otro mediante un cable de red puede ser suficiente para tener conexion, tambien se puede.

Un wireless acces point(punto de acceso inalambrico) es un dispositivo que amplifica la conexion del router a los dispositivos para que se puedan conectar sin necesidad de un cable. Esto se suele usar en entornos donde no es muy conveniente el uso de cableado o simplemente es mas facil y comodo usar un wireless.

Router: es un dispositivo de red encargado de interconectar redes. Su funcion es la de establecer la ruta que destinara a cada paquete de datos que le llegue por parte de un dispositivo. En caso de que quieras conectar equipos dentro de una red lan usas un switch o un access wireless point.

IP: este es el protocolo de internet. Se asigna a cada dispositivo y es unico y privado. El direccionamiento ip consiste en el proceso de asignar direcciones ip a los dispositivos. El enrutamiento ip consiste en dirigir el trafico de red de una ip a otra ip.

Las computadoras leen las ip mediante codigo binario, cuatro bytes de 8 bits cada una pero por fortuna el protocolo esta pensado para que nosotros los humanos podamos trabajar de manera sencilla con ellos con decimales. El rango de cada byte es de 0 a 255.

Como puedo ver mi ip? En windows en el CMD ejecutamos: ipconfig. En linux ejecutamos: ip a, o tambien: ifconfig. La ip en windows se puede modificar desde la interfaz grafica.

Una direccion ip identifica a su red(los primeros 3 bytes) y al equipo(el cuarto byte). 

Para lograr la identificacion completa el protocolo necesita lo que se llama mascara de red, que es otra direccion con el mismo formato, tambien se procesa en binario. La mascara de red le esta diciendo a todos que nuestro dispositivo nuestro ip pertenece a nuestra red.

El router reenvia paquetes basao en las direcciones ip almacenadas en la tabla de enrutamiento. Una ip no solo identifica el equipo, una ip identifica a su red y a su equipo.

La mascara de red es fundamental para poder identificar a los equipos correctamente dentro de la red.

El encapsulamiento en redes consiste en enviar datos que pertenecen a un protocolo dentro de otro protocolo como el ejemplo de TCP/IP.

Los datos se van encapsulando en distintas estructuras dependiendo de los protocolos necesarios para la comunicacion. Cuando estos datos llegan encapsulados al router el lo que hace es abrir el sobre y ver los datos y ya se los envia al destinatario.

Basicamente: Ordenador A: Siwtch A: Router: Switch B: Ordenador x

Para que dos dispositivos se puedan comunicar en una red  hacen falta: La direccion fisica: La MAC y la direccion logica: La ip.

Siempre se necesita una MAC destino y una MAC origen para encapsular el dato. Normalmente un usuario se comunica con un dispositivo dentro de su red local utilizando la ip destino, pero internamente el equipo necesita la direccion MAC para establecer la comunicacion. El protocolo ARP se encarga de solucionar esto.

ARP: protocolo responsable de obtener la direccion MAC que corresponde a una direccion ip. Se encarga de mapear la direccion ip con la direccion mac del dispositivo. Mapear significa asociar una cosa con otra.

El protocolo ARP funciona mediante la emisión de un mensaje de solicitud de ARP (ARP Request) a toda la red local. En este mensaje, el dispositivo que necesita conocer la dirección MAC asociada a una dirección IP específica envía una solicitud de ARP con la dirección IP de destino. Todos los dispositivos en la red local reciben esta solicitud.

El dispositivo con la dirección IP solicitada responde al mensaje de solicitud de ARP con su dirección MAC correspondiente. Esta respuesta se llama respuesta de ARP (ARP Reply). El dispositivo solicitante recibe la respuesta de ARP y asocia la dirección IP con la dirección MAC obtenida.

Imaginemos que el ordenador A se quiere comunicar con el ordenador B pero solo sabe su direccion ip. Lo que va a hacer el equipo A es una solicitud a ARP, una ARP request. Las ARP request son de tipo de defusion, lo que significa que va a solicitar el mac a ARP por toda la red (FF-FF-FF-FF-FF-FF) En la request de A habran estos datos para ARP:
1)MAC destino y MAC de difusion(por toda la red)
2)Tipo de peticion de mensaje: ARP
3)Cual es la ip origen, cual es la ip destino y la MAC con una interrogacion para esperar una respuesta.
Basicamente se envia en broadcast para asegurar que la pregunta llega a todos los dispositivos de la red LAN. La razon por la que se envia en broadcast es para preguntar a cada uno de los dispositivos por la ip destino y si concide con la request ya podra obtener la MAC. El switch envia a todos los puertos activos menos el destino origen.
El ordenador B responde con una ARP replay. Y no es necesario un broadcast para la ARP replay por que la direccion destino ya conoce la direccion origen. Solo se responderia el ordenador B al ordenador A. Y A ya tiene la MAC que buscaba.

Todos los equipos tienen una tabla ARP donde almacenan las direcciones mac asociandolas a sus correspondientes direcciones ip. Esta tabla ARP la podemos ver en windows con el comando: 
arp -a

En whireshark podemos ver detalladamente quien esta preguntando por la MAC de que ip.

Con Cisco Packet Tracer podemos simular una red, simula el funcionamiento real de los dispositivos y la comunicacion en una red de datos. Si pinchamos en los dispositivos de packet tracer podemos ver los componentes de hardware y mas opciones.

Recordemos que el cable Ethernet es conocido tambien como UTP. La diferencia entre la version 5 y la version 6 radica en la rapidez de transmision de datos y la calidad de conexion. La version 6 generalmente ofrece velocidades mas altas y reduce la interferencia electromagnetica mejor.

Un host es un dispositivo que se encuentra conectado a una red local.
El comando ping usa el protocolo ICMP, protocolo de transmision de mensajes. ping 192.168.1.1 Esto solo enviaria 6 paquetes de 64 bytes.
Si ejecutamos: ping -t 192.168.1.1 y desconectamos 192.168.1.1, la conexion ping se pierde y deja de ejecutarse y si conectamos otra vez 192.168.1.1 ping resume la ejecucion de envio de paquetes.
Esto se usa para comprobar si tengo conexion con un dispositivo en mi red local.

Gateway: Dispositivo informatico que proporciona a las maquinas de una red lan conectadas a el un acceso hacia una red exterior, cuando queremos comunicarnos con alguien que no esta en nuestra casa por ejemplo. El router suele actuar como puerta de enlace predeterminada.
Ejemplo dos pares de ordenadores conectados a dos switch estos switch conectados a un router.
Todos los pcs deben saber la ip de su gateway o puerta de enlace predeterminada para comunicarse con el exterior.

Para entender mejor una ip: Imaginemos que tenemos varias casas en distintas calles en una ciudad. Si queremos identificar nuestra casa necesitamos dos cordenadas: Primero necesitamos la direccion de la calle y luego necesitamos el numero de nuestra casa. La ip primero identifica la red y luego el numero del dispositivo. Cuando vemos una ip vemos 4 conjuntos de numeros separados por cuatro puntos pero debemos recordar que por detras estos numeros son bits. Cada conjunto de numeros se llama octeto. Cada octeto me da 256 combinaciones distintas de bits.


Cuando escribimos: ip/24 estamos diciendo que los primeros 24 bits pertenecen a la red. Esto se conoce como CDIR, es un sistema de notacion que se utiliza para representar rangos de direcciones ip y subredes.

La direccion de broadcast es: "la ip".255 Ej: 192.168.121.255. Esta direccion no pertenece a ningun equipo porque se va a usar para comunicarse con toda la red a la vez.

En una red, el número de hosts posibles se determina por la cantidad de bits disponibles para los hosts en la dirección IP. Si tienes nn bits para los hosts, el número total de hosts posibles es 2n2n. Sin embargo, siempre se reserva una dirección para la red y otra para el broadcast, por lo que el número real de hosts utilizables es 2n−22n−2. Por ejemplo, si tienes 8 bits para los hosts, eso significa que puedes tener 28=25628=256 direcciones, pero solo 254 de ellas son utilizables para hosts, ya que una se usa para la dirección de red y otra para la de broadcast. Entonces solo se pueden 254 host porque 255 es para la direccion de red y 256 para el broadcast.

Si nos dan esta direccion: 50.50.50.130/27. 

-Para averiguar la mascara de subred:
11111111.11111111.11111111.11100000
1,2,4,8,16,32,64,128     32,64,128=224.
Por lo tanto: 255.255.255.224

-Para la direccion de red:
50.50.50.128/27
Este es el nombre de la red.

-Para el Broadcast:
Para el broadcast se va a usar la direccion mas alta posible en los bits de host. En este caso si los primeros 27 bits pertenecen a la red significa que los ultimos 5 perteneceran al host y como tienen que ser lo mas alto posible seran todos uno. Por lo tanto:
50.50.50.100.11111  Sumamos todos los 1 con la tabla y nos da como resultado 159.
50.50.50.159

-Para obtener el numero total de host que hay en la red:
Tenemos que ver el numero total de bits que nos deja la subred, en este caso son 5. Se haria:
2 elevado a 5 - 2 y esto es igual a 30 equipos en total.
Hacemos -2 porque hay que restar la direccion de red y la direccion de broadcast.

El rango seria: entre 50.50.50.129 y 50.50.50.159    159 - 129 es igual a 30. 30 host se pueden

Las subredes: Es un metodo para maximizar o aprovechar las ipv4 de 32 bits. Hay en total 4295967296 posibles ipv4-

Tenemos esta ip: 192.168.123.0/24 y queremos dividirlas en 4 subredes mas pequeñas.
2 elevado a 2 es 4 por lo tanto necesito 2 bits para crear 4 subredes.

Mascaras de subred de longitud variable(VLSM). Crear subredes de una red pero cada una de distinto tamaño para buscar el uso eficiente de las escasas direcciones ipv4.
Para hacer un VLSM: 
1.Ordenar de mayor a menor las subredes.
2.Modificar la mascara de red sabiendo los host.
3.La siguiente red sera igual al broadcast anterior +1

En el mundo somos 8000 millones de personas y hay 4.300 millones de ipv4 disponibles lo que significa que se acabaran pronto. El ipv4 salio en 1970 y el ipv6 salio en 1990.
Internet se abre al publico en 1969.

IANA distribuia las direcciones ip a distintas organizaciones RIRs, El total de direcciones ip se dividio en clases. Segun la clase de la ip, la mascara de subred era diferente,
Las ip se asignaban por bloques a diferentes gobiernos u organizaciones, segun sus mascaras de clase.
/8: unas 16 millones,
/16: unas 65000
/24: 256
El uso de clases con mascara fija al dia de hoy es inaceptable, debido a la limitada disponibilidad de espacio libre de las ipv4.
IANA creo unas direcciones privadas que no harian falta solicitar a ningun ISP o registro. Como:
-10.0.0.0
-192.168.0.0

Estas ips pueden repetirse a lo largo del mundo y obviamente pasa pero como son privadas y se usan en redes locales no hay problema con que se repitan. Una ip puede repetirse en varios LAN pero nunca sale a Internet asi que no importa.

Las ips que no se pueden repetir y son unicas son las publicas. Una ip  publica puede representar a varias privadas mediante el protocolo NAT. Las ips publicas nos la proporcionan nuestros ISP(provedores de servicios de internet)
Nosotros pagamos para poder usar una ip publica que represente a nuestra lan interna de cara a internet. 

Optimizacion de direcciones ipv4:
-Direccionamiento sin clase y mascaras variables.
-Direcciones ip privadas que pueden repetirse.
-Una sola ip publica puede representar a varias privadas.
IANA tiene sucursales en cada continente, en total son 5.
Podemos averiguar nuestra ip publica con paginas como "What is my ip?"
Las ip publicas van cambiando a lo largo del tiempo dependiendo de las politicas del ISP, esto permite gestionar mejor las escasas direcciones, cuando hay una ip publica que no se esta usando se le da a otro usuario. Si queremos que nuestra ip publica no cambie debemos de contratar un servicio especial con nuestro ISP, normalmente son pensados para un uso empresarial.

Las ips que no cambian son fijas y las que si que cambian son dinamicas.

Si mientras estamos comunicandonos con el exterior en internet y la ip publica cambia es posible que suframos un breve cambio en la conectividad. La ip publica suele cambiar en horarios que normalmente no se esta usando la conexion. De todas maneras no importa casi nada que la ip publica varie.

Por ejemplo si tenemos un servidor web y queremos que la gente de todo el mundo lo vea necesitamos tener una ip publica fija, porque en caso de que cambiara constantemente la gente no podria acceder a nuestro servicio.

NAT: es una tecnica de red que consiste en que una ip publica cuando se conecta a internet representa a todas las ip privadas de la red suya. Muchos routers estan preconfigurados para usar NAT de manera automatica. Es decir: en una red privada varios dispositivos con ip privadas pueden usar la misma ip publica, esto se utiliza para reciclar las ip publicas. Como solo puede haber una ip publica, al haber dos ip privadas con la misma ip publica, se necesita diferenciar a cada una, esto se consigue mediante PAT, PAT es el proceso, es la tecnica que consiste en asignar diferentes puertos a dispositivos con ip privadas que comparten la misma ip publica.

IANA:RIRs:ISP:cliente
1. **IANA (Internet Assigned Numbers Authority)**: Es la entidad responsable de la asignación global de recursos de direcciones IP y otros parámetros de protocolos de Internet. IANA asigna bloques de direcciones IP a las RIRs.
    
2. **RIRs (Regional Internet Registries)**: Son organizaciones regionales que gestionan y distribuyen direcciones IP en una región geográfica específica. Ejemplos de RIRs incluyen ARIN (América del Norte), RIPE NCC (Europa, Oriente Medio y parte de Asia Central), APNIC (Asia y el Pacífico), LACNIC (América Latina y el Caribe) y AFRINIC (África).
    
3. **ISP (Internet Service Provider)**: Son proveedores de servicios de Internet que suministran acceso a Internet a los usuarios finales y organizaciones. Los ISP reciben bloques de direcciones IP de las RIRs para asignar a sus clientes.
    
4. **Cliente**: Son los usuarios finales u organizaciones que reciben direcciones IP de su ISP para conectarse a Internet. Cada dispositivo en la red de un cliente, como computadoras, teléfonos inteligentes, impresoras, etc., puede tener una dirección IP asignada por el ISP.

Diferencias entre ipv4 y ipv6:
ipv4:
-Utiliza direcciones ip de 32 bits.
-Es el actual protocolo pero esta habiendo escasez de estas ip
-Los octetos se separan por .
-Hay 4300 millones de combinaciones posibles de estas ip
-Se creo en 1970, fue parte del proyecto ARPANET.

ipv6:
-Utiliza direcciones ip de 128 bits
-Se creo para la escasez de ipv4
-Hay 340 trillones de combinaciones posibles
-Los octetos se separan por :
-Mejora la seguridad y el rendimiento
-Se creo en 1990

DHCP: Protocolo de direccion dinamica
Cuando dos dispositivos se quieren comunicar por internet es esencial que a cada uno de ellos se le asigne una direccion ip y una mascara de red. Se puede configurar una red y asignar distintos direcciones ip a cada dispositivo pero seria una tarea tediosa, aqui es cuando entra en juego el protocolo DHCP. El servidor DHCP se encargara de brindar toda la configuracion necesaria, para que los demas equipos puedan trabajar en esa red. Un servidor DHCP puede ser un router, un acces point o una computadora mas dentro de esa red.


Neofetch es un comando de linux que muestra informacion de nuestro sistema y la distribucion de Linux en el terminal.

Un servidor es una computadora o sistema informático dedicado a proporcionar servicios, recursos o funcionalidades a otras computadoras, dispositivos o usuarios en una red. Estos servicios pueden incluir el almacenamiento y acceso a archivos, el alojamiento de sitios web, la gestión de correo electrónico, la ejecución de aplicaciones, entre otros.

Como instalar y configurar un server DHCP:
Para esto necesitaremos descargar fedora server, windows xp y mx_linux en virtual box y en configuracion tenemos que seleccionar que todos esten conectados al mismo switch, recordemos que estamos configurando una red local.
El servidor fedora con acceso a internet porque necesitamos descargar algunas aplicaciones y los tres dispositivos conectados al mismo switch. Aqui es cuando actua el protocolo DHCP. Le diremos al servidor fedora que a medida que los dispositivos se vayan conectando les vaya repartiendo direcciones ip.

Windows utiliza un protocolo de autoconfiguracion de ips privadas en caso de que no exista un servidor DHCP. como el protocolo APIPA.
El protocolo APIPA evita que las tarjetas se queden sin ip y hace que los dispositivos pertenezcan a una misma red cuando el servidor DHCP no se encuentra disponible. Windows tiene esto por defecto pero distribuciones como Linux hay que activar esto manualmente como AVAHI.
Una ip como esta: 169.254.X.X es señal de que no hay servidor de DHCP funcional.

Nos vamos al servidor de fedora y ejecutamos: dnf install dhcp-server
Necesitamos asignar una ip la interfaz del servidor DHCP. Para ello nos descargamos NMTUI(Network manager text user interface)
Ejecutamos: nmtui
Ejecutamos: dnf install NetworkManager-tui
Ejecutamos: nmutui
Le damos a edit conection y en ipv4 ponemos una ip como 192.168.0.100/24
Se pueden configurar tambien servidores DNS(Domain Name System) pero da un poco igual
Con esto la ip esta asignada en la interfaz, ahora hay que configurar el servicio. Los servicios en linux dependen de algun archivo de configuracion.
Ejecutamos: /etc/dhcp/dhcpd.confg Al ejecutar esto nos dara una ruta con un ejemplo de archivos para usar. Nos metemos en esa ruta usamos ls y vemos los archivos. Nos metemos al archivo y copiamos lo que nos interese. Y ya me perdi en el tutorial del  video xd.

Proceso por cual DHCP establece direcciones ip: Cuando una ip se conecta a una red manda un mensaje DHCP a toda la red a modo de broadcast, uno de los servidores DHCP recibe el mensaje y le manda unas ofertas al destino, este ve las ofertas y le manda una request de la oferta que quiere y DHCP responde con una reply aceptandolo, de esta manera un dispositivo consigue tener su propia ip

Proceso por el cual ARP establece direcciones MAC: Un dispositivo que conoce la ip de su ip destino pero no su MAC pregunta quien es esta ip? esta pregunta le llega a el dispositivo destino y lanza una respuesta mandandole su direccion MAC al que preguntó y este la recibe y la almacena en una tabla de ARP y con esto ya puede enviar datos al destino.

VLANS: Redes de areas local virtuales
son redes lógicas creadas dentro de una red física para segmentar y organizar dispositivos en grupos lógicos independientes, proporcionando segmentación de redes, aislamiento de tráfico, flexibilidad y escalabilidad, y optimización del rendimiento de la red.
En una red normal de cableado los distintos dispositivos se conectan a un switch y comparten conexion. Las VLANS pueden segmentar esta red segun los puertos del switch. Por ejemplo: el puerto de switch del 1 al 7 va a ser VLAN1, del 8 al 15 va a ser VLAN2 y etc.
Esto sirve para crear redes con mejor rendimiento y mejor administracion, es recomendable. Con esto se pueden usar redes conectadas por switches en sitios grandes como un edificio formando una misma red logica.

Switch multicapa: Un switch multicapa es un tipo de dispositivo de red inteligente que puede hacer dos cosas: primero, puede enviar datos a los dispositivos correctos en una red local (trabajo típico de un switch normal); segundo, puede enviar datos entre diferentes redes (como si fuera un router). Esto lo hace más versátil y útil en redes grandes y complejas. Ayuda a reducir la necesidad de tenere multiples dispositivos como routers y switches separados.
Con un ejemplo: La manera mala seria tener varios grupos de ordenadores conectados cada grupo a un switch y cada switch conectado al router. La manera buena seria usar un switch multicapa que maneje VLANS, redes individuales y que permita la conexion entre todas ellas sin la necesidad de usar varios switches. Con esto conseguimos reducir el costo, el cableado y mejores resultados de conectividad y comodidad.

Estamos en cisco packet tracer y tenemos dos pares de dos ordenadores conectados a un switch multicapa y con VLANs. Nos metemos en la confiiguracion del switch y en el codigo pponemos:
enable
configure terminal
# hastag vlan 10
#name SOPPORTE
#exit
vlan 20
#name ADMINISTRACION
#exit
De esta manera las VLANS ya estan creadas en el switch. ahora toca asignar cada una a los puertos del switch.
#inter
#interface r
#interface range fa
#range fastEhernet 0/1-10
#swi 
#switchport mode
#switchport mode access
#swi 
#switchport ac
#switchpport access vlan 10

En el contexto de las VLANs se puden configurar dos modos de acceso para los puertos de un switch.
-Modo acceso: Permitira el pasaje de solo una VLAN.
-Modo troncal: Permitira el pasaje de todas las VLANs.

Si queremos que el switch solo procese tramas de una via usaremos el modo acceso para indicarle los puertos especificos que queremos que pertenezcan a esa subred.

Enrutamiento: Enrutamiento es el proceso de enviar paquetes entre redes.

El enrutamiento estatico consiste en darle instrucciones a un router para donde tiene que enviar los datos a otras redes locales o lugares de Internet. Esto se consigue con un administrador de red que configura una ruta estatica de forma manual para alcanzar una red especifica.

Imaginemos que a la izquierda de nuestro cisco packet tracer tenemos dos pares de dos ordenadores por par y cada uno esta conectado a un switch(dos en total) y estos estan conectados a un router, y a la derecha tenemos exactamente lo mismo, es decir 8 ordenadores 4 switches y dos routers, los routers se quieren comunicar pero no pueden hacerlo asi como asi, entonces aqui es cuando usamos el enrutamiento estatico, le damos instrucciones al router como administrador de la ruta que tiene que seguir para enviar los datos de los ordenadores origen y hacerselo llegar a los ordenadores destino a traves de los switches y todo.

Router on a stick: Es un enrutador portatil a veces llamado enrutador de viaje o de bolsillo, es un dispositivo pequeño que ofrece internet en cualquier lugar donde lo necesites, Estos enrutadores suelen ser un USB.

El "modo trunk" es un término utilizado en redes informáticas, específicamente en la configuración de switches y enrutadores, para referirse a la configuración de un puerto que permite transportar múltiples VLAN (Virtual LAN) a través de él.

Cuando un puerto está configurado en modo trunk, puede transportar datos de varias VLAN simultáneamente, utilizando etiquetas de VLAN para distinguir qué tráfico pertenece a cada VLAN. Esto es útil en redes donde se necesita segmentar el tráfico en múltiples VLAN para organizar y asegurar la red de manera eficiente.
Si varias VLANs estan conectadas a un switch el puerto del switch que se conecte al router debe estar establecido en modo trunk, se deben utilizar etiquetas de VLAN para diferenciar que datos son de cada una de ellas.

IEEE (Institute of Electrical and Electronics Engineers) es una organización profesional técnica mundial dedicada al avance de la tecnología en numerosos campos relacionados con la ingeniería eléctrica, electrónica, computación, telecomunicaciones y otras áreas afines.

Establecida en 1963, el IEEE es conocido por sus estándares técnicos, que son ampliamente utilizados en todo el mundo para garantizar la interoperabilidad y la compatibilidad de productos y servicios en una variedad de industrias. Algunos de los estándares más conocidos desarrollados por IEEE incluyen:

1. **IEEE 802.11**: Estándar para redes locales inalámbricas (Wi-Fi).
2. **IEEE 802.3**: Estándar para redes de área local (LAN) por cable, como Ethernet.
3. **IEEE 802.15**: Estándar para redes de área personal inalámbricas (WPAN), como Bluetooth.

Dot 1Q presenta un mecanismo que permite a multiples redes compartir de forma transparente el mismo medio fisico sin problemas de interferencia entre ellas. Con Dot 1Q.
IEEE 802.1Q es un estándar que define el etiquetado de VLAN para redes Ethernet. Con Dot 1Q que es lo mismo que IEEE 802 1Q esta dicendo de MAC X para MAC Y. El objetivo de esto es que el router identifique que VLAN le esta llegando y que actue con una ip u otra.

El protocolo de vector de distancia (distance vector) se utiliza para determinar la mejor ruta para enviar información dentro de una misma red. Este protocolo es utilizado en redes internas (intranets) o en redes locales (LANs) para determinar la ruta más eficiente entre dos dispositivos dentro de la misma red.

El protocolo de vector de distancia calcula la distancia (o métrica) hacia un destino basándose en el número de saltos (nodos intermedios) que debe atravesar el paquete de datos. Cada router en la red mantiene una tabla de enrutamiento que contiene información sobre las rutas disponibles y sus métricas asociadas. Con esta información, el router puede seleccionar la ruta óptima para enviar los datos hacia su destino.

Por ejemplo RIP(Routing information protocol) es un ejemplo de vector de distancia

BGP (Border Gateway Protocol), o Protocolo de Puerta de Enlace de Borde, es el protocolo que ayuda a los routers a determinar la mejor ruta para alcanzar redes externas y sistemas autónomos en Internet. Les proporciona a los routers información sobre las rutas disponibles y los ayuda a seleccionar la ruta óptima para enviar los datos hacia su destino, asegurando así que la comunicación a través de Internet sea eficiente y confiable.

OSPF se utiliza principalmente para redes locales o redes gestionadas por una sola organización, como intranets corporativas o campus universitarios. Proporciona un enrutamiento eficiente dentro de una red y es ideal para entornos donde la topología de la red es conocida y estable. OSPF se suele utilizar para redes locales normalmente pero tambien se puede usar para Internet.

Un Sistema Autónomo (AS) puede ser una universidad, una empresa, una organización gubernamental o cualquier otra entidad que administre su propia red de manera independiente. Estas entidades pueden contratar los servicios de un ISP (Proveedor de Servicios de Internet) para obtener conectividad a Internet, pero siguen siendo consideradas sistemas autónomos porque gestionan sus propias políticas de enrutamiento y tienen un control administrativo sobre su red.

Por ejemplo, una universidad puede tener su propio sistema autónomo que consta de varias redes internas, como redes de estudiantes, redes de profesores, laboratorios de investigación, etc. Aunque la universidad pueda obtener servicios de conectividad a Internet a través de un ISP, todavía sería considerada un sistema autónomo porque tiene control sobre la gestión de su red interna y sus políticas de enrutamiento.

 UDP es un protocolo de transporte en la capa de transporte del modelo OSI.
 Proporciona una forma de enviar datos sin necesidad de establecer una conexión previa entre el emisor y el receptor, lo que lo hace más ligero y rápido que TCP.

Una tabla de enrutamiento es una base de datos que contiene información sobre las rutas disponibles en un sistema o dispositivo de red y cómo alcanzarlas. Proporciona información sobre los destinos disponibles en la red, las interfaces de red asociadas y las direcciones de los próximos saltos para llegar a esos destinos.

Un hub es un dispositivo de red que actúa como un concentrador de datos, retransmitiendo los datos recibidos a todos los dispositivos conectados a él. Aunque fue ampliamente utilizado en el pasado, ha sido reemplazado en gran medida por switches en redes modernas debido a sus limitaciones en términos de rendimiento y eficiencia. Es como un switch pero version antigua que no se utiliza a dia de hoy.

DNS(Domain Name System): Es un sistema que traduce los nombres de dominio de una web como puede ser por ejemplo: "hola.com" lo traduce a ip numericas web que son utilizadas para que los dispositivos y maquinas de red e internet se puedan localizar las web.

**NAT estático vs NAT dinámico**:

-NAT estático: Asocia una dirección IP pública fija con una dirección IP privada específica. Esta asociación es permanente y siempre asigna la misma dirección IP pública a la dirección IP privada correspondiente. Se utiliza cuando se necesita acceder a un dispositivo interno desde el exterior de la red y se requiere que la dirección IP pública asociada permanezca constante.
-NAT dinámico: Asigna direcciones IP públicas de una piscina de direcciones compartidas a las direcciones IP privadas internas de manera dinámica según sea necesario. Las asignaciones de direcciones IP pueden cambiar con el tiempo, ya que se basan en la disponibilidad de direcciones IP públicas en la piscina. Se utiliza cuando se tienen más dispositivos internos que direcciones IP públicas y cuando no es necesario mantener una dirección IP pública fija para un dispositivo específico

Una VPN (Virtual Private Network) es una conexión segura que se establece sobre una red pública, como Internet, para crear una red privada virtual entre dos o más dispositivos o redes separadas geográficamente. Proporciona una forma segura de acceder a recursos de red internos o intercambiar datos de manera segura a través de una red pública.

Un túnel VPN es la tecnología utilizada para establecer esta conexión segura. Funciona encapsulando y encriptando todos los datos que se envían entre los dispositivos o redes conectadas a través de la VPN. Esto significa que, cuando se transmite información a través del túnel VPN, los datos están protegidos mediante cifrado, lo que garantiza la confidencialidad e integridad de la información durante su tránsito a través de la red pública.

Por ejemplo NordVPN es un provedor de servicios VPN que ofrece tuneles VPN que son el metodo para cifrar y asegurar toda la informacion y datos que circulan por la red

Un bucle de conmutación se produce cuando existen múltiples caminos redundantes entre dos o más dispositivos en una red. Esto significa que hay más de un camino posible para que los paquetes de datos viajen desde un dispositivo a otro. La palabra bucle se refiere a un ciclo o circuito cerrado en el que los paquetes se hacen un lio y se envian continuamente creando un bucle mal. Conmutacion se refiere al proceso de dirigir y transmitir los datos entre estos caminos del bucle mal creado.

STP(Spannsion Tree Protocol o Protocolo de expansion de arbol) es el protocolo que se encarga de eliminar estos bucles de conmutacion y garantizar que no haya problemas en la comunicacion de la red. La palabra tree, arbol, se refiere a la estructura que se crea en el protocolo para establecer una comunicacion limpia y estable.
