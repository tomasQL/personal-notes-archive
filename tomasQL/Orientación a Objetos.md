
¿Que es un objeto?
Es una representación de una entidad del mundo real. Sea esto algo físico, conceptual, incluso un mismo elemento de software.
* Entidad física: un vehículo, una casa, productos de aseo.
* Entidades conceptuales: procesos químicos, transacciones bancarias.
* Entidades de sofware: interfaz gráfica, una lista enlazada.
  
Según James Rumbaugh
	*"un objeto es un concepto, abstracción o cosa con un significado y límites claros en el problema en cuestión, un objeto conceptual puede ser "un auto".*

Según Grady Booch: un objeto posee 3 elementos, un estado (características), comportamiento (las acciones que puede realizar) y una identidad (la forma en que lleva a cabo el comportamiento).

**Estado:**
Lo que el objeto sabe, normalmente puede cambiar en el tiempo, y es implementado por un conjunto de propiedades (atributos), ademas de las conexiones que puede tener con otros objetos. Por ejemplo un estado "edad" puede ir cambiando a lo largo del tiempo.
El estado de un objeto lo implementamos en un programa como los atributos que tiene un objeto, estas son sus características.

**Comportamiento:**
Lo que el objetopuede hacer o acciones que puede llevar a cabo. Si un objeto no tiene implementado un comportamiento, este no puede reaccionar frente a la interacción con otros objetos.
Un pato por ejemplo tiene ciertas capacidades, funciones, acciones o comportamientos, como caminar, dormir, comer, hacer caca, tomar decisiones.
Los comportamientos también se componen de otros comportamientos, por ejemplo ver un objeto, consta también de un ojo que tiene la capacidad de recibir fotones y procesarlos para enviarlos al cerebro, esto es un comportamiento a una entrada que tiene permitido hacer basado en ciertas reglas.
Esto lo llamamos métodos en programación. 
Es modelado por un conjunto de mensajes a los que el objeto puede responder (esto serían las acciones que este puede realizar).

**Identidad:**
Cada objeto tiene una identidad única, incluso si su estado es idéntico al de otro objeto. Por ejemplo tener tres vehículos iguales. Aunque estos sean