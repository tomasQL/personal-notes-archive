
Componentes de una red.
	*PC - Conectado a la red y participe de la misma = hosts.
	Hosts - Dispositivos finales = "clientes"*
En redes, un host es el dispositivo de la red que se le asigna un nº para la comunicación.
Así, identificamos a este host dentro de una red determinada.
	*IP: Internet Protocol, número que identifica al host y la red en la que 
	se encuentra.*
Esquema base de una comunicación en la red: 
Cliente - Internet - Servidor

*Redes peer to peer:* 
	Software client y server client, normalmente van separados. En el esquema peer to peer ambos actores pueden ejercer el mismo rol.
		Ventajas:
		- Fácil de instalar
		- Menos complejidad del sistema
		- Menores costos
		Desventajas:
		- Adminsitración no centralizada
		- Menos segura
		- No es escalable
		- Dependiendo de algunos factores, bajo rendimiento

**End Devices** (PC, Iphone, Laptop, Printers, Tablet, etc).
Cada end device en una red tiene una dirección. Cuando un end device envía un mensaje a otro, este deber saber la dirección final a donde se 
entregará el mensaje.

**Intermediary Devices.**
Conectan los end devices a la red. Incorporan múltiples redes individuales para formar una red interna. Estos son: Routers, LAN Switch, Wireless Router, Multilayer Switch, Firewall Appliance.

**Network Media.**
Medios por los que se transmiten los datos del mensaje.
Cobre, Fibra óptica, Coaxial, hilos metálicos. LAN, Wireless, WAN.
Business Internet Connections.
The Converging Network.
Home and Small Office Internet Connections.


## Direccionamiento IPv4
Las direcciones IP se componen de 32 bits divididos en octetetos, esto quiere decir en 4 grupos de 8 bits.
El valor de un bit puede ser de 0 o 1. 
000000000.11111111.01010101.10111010
0-255 . 0-255 . 0-255 . 0-255
El número mínimo que podemos escribir en bits es el 0000000 que corresponde al 0.
El número máximo que podemos escribir en bits es el 11111111 que corresponde al 255.
Entre los 4 octetos de la IP siempre hay uno que identifica la "porción de red" y los demás la "porción de host".

**Clases de direcciones IP**
Clase A, B, C.

Clase A: Por norma siempre el primer bit componente es 0.
0xxxxxxx.xxxxxxxx.xxxxxxxx.xxxxxxxx
El rango válido de la clase A es el 01111110 = 126.
El valor máximo de la clase A es el 01111111.xxxxxxxx.xxxxxxxx.xxxxxxxx pero este no se utiliza ya que está reservado para el loopback o localhost.
*La máscara de subred predeterminada para la clase A es 255.0.0.0.
255 significa la red y 0 significa el host.*

Grupo 1.
	ip PC1: 100.0.0.19
	ip PC2: 101.0.0.20
La máscara de subred, representada por el primer octeto, es diferente en ambos end devices, por lo que nunca llegarían a comunicarse.

Grupo 2.
	ip PC1: 100.0.0.19
	ip PC2: 100.0.0.20
La porción de dirección de red es correcta en ambos dispositivos.

Clase B: Por norma siempre los dos primeros bits del primer componente son 1 0 .
10xxxxxx.xxxxxxxx.xxxxxxxx.xxxxxxxx
El rango mínimo válido parte desde 10000000 = 128.
El rango máximo válido es 10111111 = 191
La máscara predeterminada para la clase B es 255.255.0.0 

Grupo 1.
	ip PC1: 130.40.0.19
	ip PC2: 130.0.0.20
	Primer y segundo octeto son diferentes.
Grupo 2.
	ip PC1: 100.0.0.19
	ip PC2: 100.0.89.20
	

Clase C: Por norma, siempre los primeros 3 bits del primer componente es 110xxxxx.xxxxxxx.xxxxxxxx.xxxxxxxx.
El rango mínimo válido parte desde 11000000 = 192
El rango máximo válido es 11011111 = 223
La máscara de subred predeterminada para la clase C es 255.255.255.0

Sobre las direcciones IPv4.
La máscara detemina cuantos de los 4 componentes corresponden a 
una porción de red y de host (osea, que identifica al host dentro de la red).
En una red pura (sin subredes) la máscara tendrá solo dos valores:
255 - porción de red
0 - porción de host
ip: 192.168.90.10
	r.r.r.h
mask: 255.255.255.0
La máscara me dice entonces, que los tres primeros octetos corresponden a a la red.

