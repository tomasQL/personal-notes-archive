  
**1. Introducción a la virtualización.**
**2. El hipervisor.**
**3. El centro de Datos.**
**4. El centro de Datos Virtual.**
**5. La nube.**
**6. Soluciones de VMware.**
**7. Conclusiones.**

**Nota personal**
	*Para entender el contenido y las fronteras de la virtualización, debemos comenzar enteniendo sobre que base trabajamos (hardware, software, abstracciónes de "sistema" computacional ), y como transformamos dicho objeto a la idea de la virtualización.*
	
<hr>

# 1. Introducción a la virtualización



**Hardware:** es lo tangible, las herramientas sobre las que utilizamos día a día.
Es un conjunto de componentes físicos que forman un sistema informático.

CPU: Computer Processing Unit. Compuesta por circuitos integrados, principalmente transistores de silicio en una pieza comúnmente llamada chip.

RAM: Random Access Memory. Un equipo tiene dos tipos de memoria, la no volátil (read-only) y la memoria volátil.

ROM: Read Only Memory.

Motherboard: Printed Circuit Board. Contiene los puertos del procesador, RAM, ROM, red, y E/S.

Chipset: Conjunto de microchips en una placa base que administra funciones específicas, como la transmisión de datos al procesador, a la RAM, etc.

Almacenamiento: Dispositivos de almacenamiento de datos.

**Software:** interfaz (el/los medios) mediante la que utilizamos las funciones de los dispositivos. Diferentes tipos de software para controlar diferentes tipos de acciones informáticas que nos otorgan los sistemas de hardware.

Software del sistema: Es la parte que controla las funciones más básicas. Comúnmente es el BIOS, el firmware (software almacenado normalmente en la ROM).
El "primer" tipo de software de sistema es el sistema operativo.

OS: Operative System. Se ejecuta en segundo plano y se encarga de controlar el hardware ya que está conectado directamente a él.

Software de aplicación: se ejecuta sobre el sistema operativo.

<hr>

¿Qué es una máquina virtual?
VM: virtual machine.
Es un programa que interactúa directamente con el hardware.

