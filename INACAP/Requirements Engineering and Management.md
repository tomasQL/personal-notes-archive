
<hr>

### Ingeniería de Requerimientos - Asignatura

Bibliografía consultada.
Systems and software engineering — Life cycle processes — Requirements engineering.
ISO - IEC - IEEE
https://ieeexplore-ieee-org.ezproxy.dnb-inacap.cl/stamp/stamp.jsp?tp=&arnumber=8559686

Engineering and Managing Software Requirements - Aybüke Aurum & Claes Wohlin - Springer.
https://repository.dinus.ac.id/docs/ajar/%5BAyb%C3%BCke_Aurum_(Editor),_Claes_Wohlin_(Editor)%5D_En(BookFi.org)_.pdf

<hr>

# Ingeniería de Requerimientos
(Guía de aprendizaje)

1. Requerimientos: tipos, técninas y dificultades para su obtención.
2. Importancia de la ingeniería de requerimientos.
3. Roles y responsabilidades.
4. Costos y planificación.
5. Actividades de la ingeniería de requerimientos.

### 1. Requerimientos.

¿Qué es un requerimiento?
IEE:
	1. A condition or capability needed by a user to solve a problem or achieve an objective.
	2. A condition or capability that must be mer or possessed by a system or system 
		component to satisfy a contract, standard, specification, or other formally imposed
		documents 
	(A documented representation of a codition or capability as in 1 or 2).

Sommerville: Un requerimiento es una declaración abstracta de alto nivel de un servicio
que debe proporcionar el sistema o una restricción de este.

Normalmente se apunta a que el requerimiento debe describir *lo que el sistema debe hacer* y 
no el *cómo lo debe hacer* aunque esta línea sea algo difícil de persona a persona y difiera 
en su práctica.

En el documento Systems and Software Engineering (ISO/IEC/IEE) se hace enfasis en lo que 
"deberá (shall)" hacer el sistema. 
Pero también, capturan las restricciones (*constraints*). Restricciones propias del dominio, o
del sistema.

Las principales características de un requerimiento son:

* Completo: no necesita detalles en su redacción; se porporciona la información suficiente
	para su comprensión.
* Conciso: Simple y clara, debe ser comprensible.
* No ambiguo: Debe existir una sola interpretación, sin generar confusiones.
* Consistente: No debe contradecir otro(s) requerimiento(s).
* Probar y verificar: si no se puede comprobar un requerimiento, ¿Cómo sabemos que 
	se cumplió con él o no?.


#### Tipos de requerimientos.

Se pueden dividir en dos grandes categorías: Funcionales y no funcionales.
* Functional Requirements: What the system will do.
* Non-functional Requirements: Constraints on the types of solutions that will meet the 
	functional requeriments. i.e accuracy, performance, security, etc.

Los requerimientos funcionales describen las funciones que el sistema será capaz de realizar.
Describen transformaciones del sistema, sobre entradas para producir salidas (el cómo, que 
bajo la perspectiva de sistemas sería el proceso se da en su desarrollo y considerando los 
requerimientos no funcionales).
Los requerimientos no funcionales se relacionan con las características del sistema y que lo 
limitan, enmarcando sus fronteras y restricciones.


#### Clasificación de los Requerimientos.

Recordemos que este proceso es importantísimo para la especificación y documentación de 
las necesidades de los clientes o usuarios en su dominio a la hora de implementar una solución
de software (o tecnológica en general).

El análisis completo de las necesidades del usuario
	+
Acuerdos entre el desarrollador y el cliente 
	= Resultan en una Especificación de Requerimientos de alta calidad.

Los requerimientos no obstante son parte de un proceso de ingeniería que no es inherente
al desarrollo de Software, mas bién, a diversas disciplinas al momento de solucionar problemas
empresariales, organizacionales, de usuarios o clientes.

Se pueden clasificar en:

* Requerimientos de procesos: Condiciones básicas para la aplicación de metodologías 
	de trabajo asegurando fluides y riesgos en el desarrollo a modo de ejercer control (Proceso).
* Requerimientos de usuario: Actividad central conociendo las necesidades del usuario para 
	cumplir con sus expectativas del producto como del proceso (costo y tiempo).
* Requerimientos de análisis y negociación: Para lograr una especificación de alta calidad debe existir un análisis completo y exhaustivo logrando acuerdos entre desarrollador y cliente, 
	manifestando la conformidad del resultado.
* Requerimientos para la gestión: el proyecto, al cumplir con ciertas condiciones, debe asegurar el control de las actividades y del desarrollo de cada requierimiento.


Según Aybüke Aurum & Claes Wohlin en Engineering and Managing Software Requirements.
Requirements Classification:
* Functional & Non-functional requirements
* Goal level requirements - related to business goals
* Domain level requirements - related to problema area
* Product level requirements - related to the product
* Design level requirements - what to build
* Primary requirements - elicited (*obtenido o producido*) from stakeholders
* Derived requirements - derived from primary requirements
Others classifications:
* Business requirements versus technical requirements
* Product requirements versus process requirements - Business needs vs how people will
	interact with the system
* Role based requirements - Customer R, User R, IT R, System R and Security R (R-requirements)
Estos requerimientos pueden ser abordados en una clasificación mas general según distintas
miradas y autores.
Por ejemplo se pueden establecer niveles de clasificación como:
* Requirements at organizational level
* Requirements at product level
* Requirements at project level
Donde los alcances de estos niveles se relaciónan con la gestión Estratégica (Strategic Management), Táctica (Tactical Management) y Operacional (Operational Management).

Con estos antecedentes, cabe preguntarnos ¿Cómo los obtenemos?


#### Técnicas para obtener Requerimientos.

Necesitamos obtener información para definir y desarrollar los requerimientos de software.
No existe una única técnica o herramienta para su obtención, por lo que esto dependerá de 
las características del cliente o usuario, del entorno y complejidad del problema a resolver.

Entre las más comunes:
* Entrevistas y cuestionarios: para reunir información proveniente de grupos o personas.
* Sistemas existentes: analizar sistemas existentes o analizar un "estado del arte".
* Lluvia de ideas: modelo para generar una gran cantidad de ideas posibles para el sistema.
* Prototipos: simulaciones del posible producto, que es probado por el usuario final.
* Casos de uso: para especificar el comportamiento de un sistema.
* Entre otras más.


Según Zowghi & Coulin - Requirements Elicitation: A Survey of Techniques, Approaches, and 
Tools (from Engineering and Managing Software Requirements).

*Requirements elicitation is concerned with learning and understanding the needs of users and project sponsors (or stakerholders) with the ultimate aim of communicating these needs to the
system developers. A substantial part of elicitation is dedicated to uncovering, extracting, and 
surfacing the wants of the stakeholders.*

Typical activities of the requirements elicitation process can be divided into five fundamental
types: 
1. Understanding the Application Domain.
2. Identifying the Sources of Requirements.
3. Analyzing the Stakeholders.
4. Selecting the Techniques, Approaches and Tools to use.
5. Eliciting the Requirements from Stakeholders and Other Sources.

Es importante destacar que la obtención de requerimientos no ocurre de manera aislada. Este
proceso está fuertemente relacionado al contexto en el que es llevado a cabo y sirve para 
la especificación de las características del proyecto, la organización y su entorno.

Material de profundización - INACAP.

*Educción* - "Actividad dentro de la IR que recupera información relevante acerca del dominio
del problema, y de las necesidades de las partes interesadas (stakeholders) para la
confirmación de los requisitos del producto de software", (redalyc.org).
Esto se puede traducir fácilmente, también, como el proceso de levantamiento y análisis de
requerimientos, para su posterior modelamiento.

Conceptualización de requisitos.
Esto es muy similar a lo que ya hemos establecido; aún así no es irrelevante volver a abordarlo.

* Análisis de requerimientos: aprender, entender e identificar el problema, las necesidades y los usuarios para comprender las restricciones de la solución.
En la obtención / levantamiento / educción de requisistos se obtiene un discurso.
Discurso que es entregado por los interesados en el desarrollo de una solución de software.
A partir de este discurso, obtenemos un modelo conceptual.

Informalidad: **¿Para qué toda esta parafernalia de conceptos y metodologías?**
	Lo que debemos entender al desarrollar sistemas y software, es que existe la "crisis del software" y otros antecedentes, que aún atentan contra la calidad de una solución tecnológica.
	Este gap o "brecha", es debido principalmente, por la dificultad en los procesos de comunicación entre las partes, tanto desarrolladores como usuarios o clientes. Generando el 
	riesgo de llegar a una solución de software de baja calidad. 
	*Recordar Sommerville y todo el resto de weones que leiste acerca de porqué fallan los
	proyectos de software, tomasQL.*

Cuando existen dificultades a la hora de obtener requerimientos que se manifiestan en el 
proceso de educción, entra en juego la conceptualización de los requisitos gracias al 
discurso del cliente o usuario.
Con todo esto, aumentamos nuestra comprensión del problema, reducimos la complejidad o 
brecha (gap) del problema y su solución, contribuyendo a la obtención de conceptos y por 
lo tanto requerimientos de mayor calidad.

Entonces:
	1. Discurso del usuario en un lenguaje natural.
	2. Proceso de conceptualización de requisitos.
		2.1 Análisis orientado al **problema**.
		2.2 Análisis orientado al **producto**. 
	3. Representaciones (modelos) intermedias de los requisitos del usuario.
		Estos modelos suelen representar lo que se llama Escenario de usuario.
En el punto 3, identificamos:
(Esto es parecido pero no igual a los casos de uso y herramientas usadas en el UML)
* Actores, Atributos, Relaciones, Acciones, Funcionalidades e Interacciones.

Así, comienza la articulación del espacio del problema con elementos de la realidad, y el 
espacio del producto con las funcionalidades que debe realizar el software.

#### Dificultades para obtener requerimientos.

Todo suena muy bonito, pero en "el mundo real" cuando tenemos que ejecutar con las
metodologías y herramientas, se presentan problemas, como no.
Esto pone en riesgo la correcta definición de todo este proceso e ingeniería, que impactará
negativamente en el proyecto de software.

* Los requerimientos no son obvios y provienen de muchas fuentes
* Son difíciles de expresar en palabras (el lenguaje se torna ambiguo)
* La cantidad de requerimientos es difícil de manejar
* Un requerimiento puede cambiar a lo largo del ciclo de desarrollo
* El usuario no puede explicar lo que hace
* Tiende a recordar lo excepcional y olvidar lo rutinario
* Hablan de lo que no funciona
* Los usuarios tienen distinto vocabulario que los desarrolladores

No profundizaré (personalmente) en estas dificultades ya que son claras y recuerda, 
si te crees profesional debes actuar como uno. El resto son factores externos manejables.

### 2. Importancia de la ingenería de requerimientos.

Aquí, la guía hace un énfasis, que a mi gusto, es simplemente darle la vuelta a las 
anteriores perspectivas, metodologías y necesidades establecidas como posibles problemas
para enfatizar la importancia de la IR. Sin embargo, como recordatorio o forma de reconocer
nuevos "dolores de cabeza" y sobre todo *administrar bien nuestros dos recursos más valiosos*, el tiempo y el dinero es que le damos cuerda a este tema. Informalidad (no es que lo desprecie,
o crea que ya lo se todo, simplemente creo entender y tener bien grabado los aspectos de la
profesionalidad en la gestión y administración siempre pensando en su impacto y resultado en  blablablabla, puras weas).

Parafraseando a Arias (2007):
"Los requerimientos serán la pieza fundamental del desarrollo de software (como no xd), ya 
que son la forma de planear el tiempo y costo así como la definición de recursos para el control."
Recordar que antes de querer administrar, hay que definir que es lo que hay que administrar, 
por muy obvio que parezca, por eso usamos métodos y herramientas.

El desarrollo de un producto de software nunca debe ser lo que el desarrollador quiere, sino
lo que el cliente necesita, y esto puede verse "trastocado" por ser nosotros, los intérpretes de
esta obra que se pretende llevar a cabo, con todos los recursos y costos que significa su 
realización.

Las metodologías y herramientas (básicamente ser profesional...)
permite:
* Evitar rechazo de usuarios finales
* Gestionar las necesidades del proyecto de forma estructurada
* Mejorar la capacidad de predecir cronogramas y resultados
* Disminuir costos y restrasos del proyecto
* Mejorar la calidad del software
* Mejorar la comunicación entre equipos


Aybüke Aurum & Claes Wohlin.
*Requirements engineering is accepted as one of the most crucial stages in software design 
and development as it addresses the critical problem of designing the right software for the
customer.*
...
*Software requirements are critical determinants of software quality...*
El capítulo 1 aporta datos precisos de revisiones en otros estudios empíricos sobre la tasa
de fallos y sus motivos, así como porcentajes de fallos sobre proyectos de software.

**DOMAIN KNOWLEDGE!!!** (no es el único, ni principal motivo)
Esa parte la tienes que tener clarísima.


### 3. Roles y responsabilidades.









<hr>

