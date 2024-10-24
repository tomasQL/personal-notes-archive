
<hr>

### Ingeniería de Requerimientos

Bibliografía consultada.
Systems and software engineering — Life cycle processes — Requirements engineering.
ISO - IEC - IEEE
https://ieeexplore-ieee-org.ezproxy.dnb-inacap.cl/stamp/stamp.jsp?tp=&arnumber=8559686

Engineering and Managing Software Requirements - Aybüke Aurum & Claes Wohlin - Springer.
https://repository.dinus.ac.id/docs/ajar/%5BAyb%C3%BCke_Aurum_(Editor),_Claes_Wohlin_(Editor)%5D_En(BookFi.org)_.pdf

<hr>

# Ingeniería de Requerimientos

1. Requerimientos: tipos, técninas y dificultades para su obtención.
2. Importancia de la ingeniería de requerimientos.
3. Roles y responsabilidades.
4. Costos y planificación.
5. Actividades de la ingeniería de requerimientos.

### 1. Requerimientos.

¿Qué es un requerimiento?
IEEE:
	1. A condition or capability needed by a user to solve a problem or achieve an objective.
	2. A condition or capability that must be met or possessed by a system or system 
		component to satisfy a contract, standard, specification, or other formally imposed
		documents.  
	(A documented representation of a codition or capability as in 1 or 2).

Sommerville: Un requerimiento es una declaración abstracta de alto nivel de un servicio
que debe proporcionar el sistema o una restricción de este.
Los requerimientos reflejan las necesidades del cliente por un sistema que atienda cierto propósito, como controlar un dispositivo, buscar información o colocar un pedido.
Al proceso de descubrir, analizar, documentar y verificar estos servicios y restricciones se le llama Ingeniería de Requerimientos.

Normalmente se apunta a que el requerimiento debe describir *lo que el sistema debe hacer* y 
no el *cómo lo debe hacer* aunque esta línea sea algo difícil de persona a persona y difiera 
en su práctica.

En el documento Systems and Software Engineering (ISO/IEC/IEE) se hace enfasis en lo que 
"deberá (shall)" hacer el sistema. 
Pero también, capturan las restricciones (*constraints*). Restricciones propias del dominio, o
del sistema.

Ejemplos: 
	- Cuando la señal x es recibida [CONDICIÓN], el sistema [SUJETO] debe colocar [ACCIÓN] el bit de la señal x recibida con dos segundos [RESTRICCIÓN].
	- El sistema de facturas [SUJETO], debe mostrar las facturas pendientes de los clientes [ACCIÓN], en orden ascendiente o por fecha de la factura [RESTRICCIÓN].

Según la guía SWEBOK:
	"*Software requierements express the needs and constraints placed o a software product that contribute to the solution of some real-world problem"


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

Existen requerimientos volátiles y duraderos.
Unos podrán cambiar a lo largo del desarrollo del sistema y también del proceso de análisis (o en la elicitación) y los otros perduran
a lo largo del sistema.


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

## Unidad 1. Ingeniería de requerimientos.

Objetivo: elaborar una especificación de requerimientos de software para un
proyecto.
Ingeniería de Software - Sommerville / pp. 83-114

85 - derivacion de req a partir de otros

30/08/2024
Clase 2.

Identificar y documentar falencias en un sistema:

Aspectos a analizar:
* Performance
* Seguridad
* Usabilidad
* Escalabilidad

Proponer al menos 3 requerimientos para mejorar el sistema, o crear
uno nuevo que aborde las falencias.
Documentar dichas falencias.

Seguridad: Quienes tienen acceso al historial del paciente? Cuales son
los permisos que tiene el personal del Hospital sobre la información
sensible de un paciente? 

Usabilidad: Gestión de Citas, quien las programa? el hospital o la clínica
dispone de horarios? lo agenda el paciente o el personal del hospital?

Escalabilidad: HME, disponer de un modelo que permita al sistema 
integrarse con otros sistemas, afp, cajas de compensación, isapres,
etc.

Seguridad: gestion de citas, para la consulta puede ser semi-restringida, para los casos de pacientes con problemas mentales.

<hr>


04/09/2024 -  Clase día miércoles.

Actividad en clases. 12:17
Requerimientos principales basados en el contexto:
- Necesidades de operatividad de los equipos en los laboratorios (disponibilidad, resiliencia).
- Organizar la demanda (reserva y uso) de los laboratorios.
El sistema debe permitir CONOCER los equipos defectuosos y GESTIONAR
las reparaciones.

Preguntas.
¿De cuanto tiempo se dipone para el desarrollo e implementación de la solución?
	3 meses.
¿Con cuanta recurrencia se utilizan los laboratorios diariamente?
		8 clases + alumnos que puedan usarlos en tiempos libres
¿Cual es el presupuesto del centro para desarrollar una solución?
	 poco presupuesto, se solicita una cotización o factibilidad.
 ¿Existen restricciones sobre la operatividad de los equipos (eléctrica por ejemplo)?
	los lab estan conectados a una LAN de la empresa en una red, seccionados por laboratorio identificado cada computador por lab, apagado después de inactividad de tiempo mediante la plataforma automatizado. Se apagan y encienden de manera arbitraria por uso. Cada pc tiene un perfil de usuario para los usuarios de centro, con restricciones de privilegios.

* Monitoreo de RAM, CPU, ALMACENAMIENTO en RT, detección de fallas de software y hardware.
	Gestion mediante plataforma web el uso, y la reserva, en demanda y calendarizado hasta la hora actual.

	Roles: los pc ya están loggeados, hay perfil de admin en cada laboratorio. 

	Apps necesarias vienen preinstaladas, tampoco se requiere gestion de otros reglamentos del SO en los equipos.

	Cuando se generen alertas que lleguen a soporte, pero que también tengan otro alcance si se necesita, en casos de mantenimiento.
	Pic de uso, notificaciones de errores.
	Y que el computador en su monitorización se habilite o deshabilite cuando detecte estas fallas, y que esto se generen a mantención.

	Pantallazos azules, scripts maliciosos.
	Soporte se retira y se apagan los equipos.
	
	Laboratorios Existentes: 4

Dual Boot, Windows, Linux.
Calendarizazión semestral.


<hr>
# Ejercicios basados en proyectos

Criterios: Considerar falencias del sistema.
Clasificar requerimientos en funcionales y no funcionales.

1. Identificar los principales requerimientos de negocio establecidos del caso.
2. Identificar requerimientos de usuario.
3. Clasificar a los usuarios según tipo (func y no func)
4. Establecer falencias de los requerimientos.

La Cadena Hotelera desea automatizar servicios.
SI por cada hotel.
Muchas actividaes son registradas en papel. Actividades sobre las estadísticas consumen tiempo y recursos.
Quieren Centralizar y Unificación el sistema de reservas de sus hoteles.
No se realiza overbooking (Sobreventas o exceso de reservas de un servicio que está por sobre la capacidad real de la empresa)
Es para anticiparse a las cancelaciones de ultimo momento. Y garantizar la ocupación 
del 100%. 
En cambio al overbooking se desea sugerir a los clientes otros hoteles de las cadenas cuando no hay disponibilidad (Prioritario) (Requerimiento no funcional).

Los clientes de la empresa deben poder realizar sus actividades por internet (Requerimiento funcional).
Las estaciones de trabajo en los hoteles, operarán con la misma interfaz (Requerimiento funcional).
Por lo que debe simplificarse el uso del sistema
Proveer que las agencias de viajes puedan interoperar con el sistema mediante el uso de web services.
Hay necesidades de rendimiento para el check in & check out
Se debe poder usar un sistema de validación existente.
Los empleados suelen trabajar en un solo hotel, pero estos pueden ser rotados a hoteles de otra región.

Necesidad de info estadística. Sobre hoteles que abren o cierran donde la empresa está instalada. La información se recoje periodicamente y es utilizada por economistas de la empresa.
Los servicios de cada hotel varían, todos cubren una amplia gamma de servicios a la habitación.

Servicio a la habitación. Paquetes turísticos. Afiliación a sistemas de millas entre otros.
Estos servicios se van agregando y removiendo del sistema en producción incluso.
El sistema debe ser capaz de incorporar y remover nuevos modulos y subsistemas 
Servicios extras varían en el tiempo.


Apuntes.
https://registro.sernatur.cl/wp-content/uploads/biblioteca/calidad/NCh02760-2013-046.pdf
norma de clasificación de establecimientos turísticos denominados hotel ...
establece la clasificación en categorías de estrellas para los hoteles.
Esta clasificación norma el cumplimiento de requesitos generales, arquitectónicos, de equipamiento y de servicios bien definidos para la clasificación.

Existen requisitos generales, arquitectónicos y de equipamiento definidos 
deben cumplir en base a esta clasificación.

Norma chilena para Alojamiento Turístico N.Ch 2912.

<hr>


<hr>


Contexto de la problemática.

Una cadena hotelera desea automatizar varios de sus servicios y procesos empresariales
mediante el uso de los Sistemas de Información Tecnológicos ya sea actualizando o creando 
nuevos recurso que apoyen la toma de decisiones de su directiva para la eficiencia en costos de tiempo y dinero respecto a las actividades en las áreas operacionales, ejecutivas y gerenciales.

Cada hotel posee ya un sistema de información el cual debe actualizarsae en base a las siguientes 
necesidades o problemáticas:

Muchas actividades de los hoteles son registradas en el papel, y al momento de querer hacer 
las estadísticas de la empresa aumenta el consumo de tiempo y recursos de sus trabajadores 
para cumplir con esta tarea.

Para responder a lo anterior la directiva a establecido que:

* Centralización y unificación del sistema de reserva de sus hoteles.
	El sistema de reservas debe evitar el Overbooking (práctica común en el domino de negocio Hotelero).
	En cambio a esta práctica, desean sugerir a los clientes, otros hoteles de la cadena cuando no 
	exista disponibilidad siendo esta parte del sistema un aspecto prioritario.

* Las estaciones de trabajo en los hoteles deberán operar con la misma interfaz tanto para los usuarios trabajadores como para los usuarios clientes del hotel. Esto con el fin de simplificar el
  uso o interacciones con el sistema.

* La cadena necesita proveer a las agencias de viajes interoperatividad con el sistema hotelero y 
  sus servicios mediante el uso de servicios web (Web Services).

* El sistema de check in & check out debe responder con un alto rendimiento.
* La cadena hotelera posee un sistema de facturación que debe mantenerse
* Acerca de los empleados: estos suelen trabajar en un solo hotel, pero estos mismos pueden ser
	rotados a otros hoteles de la cadena en distintas regiones.

* Especialistas en economía de la empresa, presentan la necesidad e información estadística sobre
  los hoteles que abren o cierran en los lugares en donde la empresa está instalada.
  Esta información debe ser recogida periódicamente.
  
  * Cada hotel varía en los servicios que ofrecen a sus clientes, cubriendo una amplia
	gamma de servicios a la habitación, paquetes turísticos, afiliación a sistemas de millas, entre
	otros.
	Estos servicios se van agregando y removiendo en el tiempo, por lo que el sistema debe permitir
	estos cambios con el sistema en producción.

* El sistema debe ser capaz de incorporar y remover nuevos módulos y subsistemas.

<hr>

Análisis de requerimientos.

Módulo de fichas de pacientes - Forma o "flujo" general del tratamiento de la
información de un paciente.

¿De que forma quieren registrar la ficha del paciente cuando este ingresa al centro de rehabilitación?
	Desde cualquier dispositivo. 
Formulario.
¿Cómo les gustaría ver el historial del paciente en rehabilitación?
ver los pacientes, antecedentes, controles o consultas. Comentarios o notas.

¿Cómo se quiere identificar a los pacientes?
Resumen, ultimo procedimiento, luego por interaccion del usuario aparece el historial completo. 

¿Cómo se presenta el acceso a la información del paciente? (Por área del centro, por especies, por contenedor)
Clasificacion 
Por contendor
Por especie
Por tipo de animal
Por motivo de llegada
Por fecha

Clasificación de los procedimientos de hospitalización

(BPMN)proceso de negocio respecto a la manipulación de fichas.

Consultas a distintos centros de fauna silvestre.**


**Investigación de dominio: Consulta a centros de rehabilitación.** PENDIENTE
Centro de rehabilitación CONCON.

- Sobre el ingreso de fichas:
    - ¿Qué información específica debe contener una ficha de paciente al momento de su creación? (esto lo responde la foto, sin embargo es bueno escuchar que diría el cliente o que espera)
    - ¿Existen campos obligatorios y opcionales? ¿Cuáles son?
    - ¿Como registran los casos de propietarios de fauna silvestre o exóticos autorizados?NUEVOOO

- Modificación de fichas:
    - ¿Qué tipos de modificaciones son las más comunes en las fichas de pacientes?
    - ¿Existe algún sistema de control de versiones o historial de cambios en las fichas?
    
- Listado y visualización de fichas:
    - ¿Qué criterios de búsqueda y filtrado son necesarios para el listado de fichas?
    - ¿Qué información debe mostrarse en la vista resumida de las fichas activas?

- Archivado de fichas:
    - ¿Cuáles son los criterios para archivar una ficha de paciente? ¿Se recibe información sobre el SAG cuando los animales
    - son reinsertados al habitat?IMPORTANTE
    - ¿Cómo se diferencia una ficha archivada de una activa en términos de acceso y modificación?SOLICITUDES Y PERMISOS.

- Procedimientos y hospitalización:
    - ¿Qué información detallada se requiere al añadir un procedimiento?
    - En la ficha de hospitalización, ¿qué datos específicos se necesitan registrar?NETAMENTE TÉRMINOLOGÍA??

- Adjuntos y exámenes:
    - ¿Qué tipos de archivos se deben poder adjuntar a las fichas?
    - ¿Existe un límite de tamaño o cantidad para los archivos adjuntos?OJO A LA MAL UTILIZACIÓN DEL SISTEMA CASO
    - VETIAPP CAMILA
    - DETECCIÓN DE CAMPOS (CUANDO "CHANTAN" TEXTO EN LOS COMENTARIOS).
    
- Responsables y fechas:
    - ¿Cómo el registro del tiempo es crucial para el sistema e información del paciente (ingreso, procedimientos, alta)?

- Búsqueda de fichas históricas:
    - ¿Qué criterios de búsqueda son importantes para localizar fichas históricas?

- Roles y permisos:
    - ¿Qué acciones específicas puede realizar un voluntario-residente que un administrador no pueda, y viceversa?
    - ¿Existen otros roles que no estén representados en el sistema? EXTERNOS O VIATOR3.0 API DATA

- Eliminación de fichas:
    - ¿Bajo qué circunstancias se eliminaría una ficha de paciente?
    - ¿Existe algún proceso de respaldo o recuperación para fichas eliminadas?AUTH DIRECCIÓN O RESIDENTES

- Usabilidad y acceso:
    - ¿Desde qué tipos de dispositivos se accederá al sistema (computadoras de escritorio, tablets, smartphones)?
    - ¿Hay alguna consideración especial de usabilidad para el entorno de una clínica veterinaria (por ejemplo, uso con guantes, pantallas táctiles, entre otros)

### 1. **Requerimientos funcionales**

- ¿Quiénes son los responsables de actualizar o modificar las fichas (residentes, voluntarios, veterinarios)?
- ¿Hay diferencias en el seguimiento de los procedimientos rutinarios versus los veterinarios?
- ¿Cómo se maneja la ficha si se necesita adjuntar documentos aparte? OPORTUNIDAD CAMBIAR EXÁMENES POR DOCs.
* ¿Existen necesidades sobre el almacenamiento de imágenes en el sistema? OPORTUNIDAD ADJUNTAR ESTADO DEL PACIENTE FOTO???
- ¿Cuándo se decide que una ficha debe ser enviada a la carpeta de activos?

### 2. **Requerimientos no funcionales**

- ¿Existen restricciones de seguridad de la información?¿Cómo se asegura la confidencialidad de la información de los miembros de la organización?
- ¿Hay alguna necesidad de integración con otros sistemas (por ejemplo, para los exámenes clínicos o de laboratorio)? ejemplo equipos que ya se encuentran conectados a tecnologías veterinarias como radiografías, ecografías, entre otros.
- ¿Qué mecanismos de respaldo o recuperación existen para las fichas en caso de pérdida de información?
- Necesidades gráficas de interfaz de usuario y experiencia de usuario (identidad de la organización, colores, gráficas).
* Horarios de uso del sistema.

### 3. **Flujo de trabajo**

* ¿Qué pasos son manuales y cuáles podrían automatizarse?
- ¿Existen situaciones donde se deba realizar más de un procedimiento al mismo tiempo? Si es así, ¿cómo se refleja esto en el sistema?

### 4. **Registros y trazabilidad**

- ¿Qué información debe registrarse para identificar al responsable de un procedimiento?  (Lo entrega la organización
  en su docuemtación)
- ¿Cómo se lleva el control de los procedimientos veterinarios realizados y los que están pendientes?¿Se espera un servicio del sistema en este caso?

### 5. **Ocurrencias**

* ¿Existen validaciones o alertas que se esperan del sistema? Por ejemplo: ¿Qué ocurre si se intenta adjuntar un documento no válido a la ficha? Con la inactividad de una ficha activa?

COSTOS DE DESARROLLO.


- **NWRA e IWRC**: Las organizaciones _National Wildlife Rehabilitators Association_ (NWRA) y _International Wildlife Rehabilitation Council_ (IWRC) proporcionan guías importantes sobre el manejo médico y ético de la fauna silvestre. Estos incluyen estándares para el tratamiento y la liberación de animales con un enfoque en la salud y el bienestar, alineados con las _Cinco Libertades_ y los _Cinco Dominios_ del bienestar animal, los cuales son marcos clave para medir el bienestar durante la rehabilitación​
    
    [Vet Knowledge Hub](https://vetbooks.ir/minimum-standards-for-wildlife-rehabilitation-4th-edition/)
    
    ​
    
    [MDPI](https://www.mdpi.com/2076-2615/13/11/1836)
    
    .
    
- **Standards for Wildlife Rehabilitation**: La cuarta edición de este estándar internacionalmente reconocido proporciona directrices para la rehabilitación de animales silvestres, incluyendo procedimientos médicos, y es aplicable para tu sistema. Detalla los requisitos de registros médicos, manejo de la salud y el bienestar, y criterios de liberación o eutanasia cuando la reintroducción al hábitat no es viable​
    
    [Vet Knowledge Hub](https://vetbooks.ir/minimum-standards-for-wildlife-rehabilitation-4th-edition/)
    
    ​
    
    [Professionals](https://www.rcvs.org.uk/document-library/bvzs-good-practice-guidelines-for-wildlife-rehabilitation/bvzs-good-practice-guidelines-for-wildlife-centres-011016-.pdf)
    
    .
    
- **Principios y Consideraciones Legales**: En Reino Unido, la _Royal College of Veterinary Surgeons_ (RCVS) emite guías para el manejo de centros de rehabilitación que también pueden ser útiles. Estas guías hacen énfasis en que los centros deben tener instalaciones y conocimiento adecuado de cada especie, y se enfocan en el objetivo de liberar a los animales






django automatización de generacion de apis.



# Trazabilidad de los Requerimientos.

### Matriz de trazabilidad de Requerimientos:


Ejemplos de relaciones entre los "objetos" o "artefactos" entregados
o generados en el proceso de desarrollo.

Customer Requirements -> System Requirements
	Principales fuentes de información sobre las necesidades del
	negocio y las restricciones o funciones del sistema.
	
Software Requirements -> Software Architechture
	Una vez se establece la función del sistema, se derivan requerimientos de software (Diagramas UML, modelos y descripciones). Identificación previa de patrónes de diseño de 
	software.
	
Software Detailed Desing -> Implementation (code)
Implementation -> Unit Tests
	Puede estar en el alcance de un documento de especificación
	la referencia a la validación de las implementaciones durante
	el proceso de desarrollo. De este derivan las pruebas de
	integración, unitarias, funcionales (nuevamente linkea Customer Requirements), aceptación, rendimiento.


Estas relaciones deben representar las dependencias y orígenes 
de los requerimientos.



