
**PCEP™ – Certified Entry-Level Python Programmer** certification (Exam PCEP-30-0x) is a professional credential that measures the candidate's ability to accomplish coding tasks related to the essentials of programming in the Python language. A test candidate should demonstrate sufficient knowledge of the universal concepts of computer programming, the syntax and semantics of the Python language, as well as the skills in resolving typical implementation challenges with the help of the Python Standard Library.  
  
The PCEP™ certification shows that the individual is familiar with the following concepts: fundamental **terms and definitions** (e.g. compilation vs. interpretation), Python's **logic and structure** (e.g. keywords, instructions, indentation), **literals**, **variables**, and **numeral systems**, **operators** and **data types**, **I/O operations**, **control flow** mechanisms (conditional blocks and loops), **data collections** (lists, tuples, dictionaries, strings), **functions** (decomposition, built-in and user-defined functions, organizing interaction between functions and their environment, generators, recursion), **exceptions** (exception handling, hierarchies), as well as the essentials of Python programming language **syntax**, **semantics**, and **the runtime environment**.
https://pythoninstitute.org/pcep
https://pythoninstitute.org/pcep-exam-syllabus



<hr>

Las computadoras pueden realizar tareas muy complejas pero no es algo innato de ellas.
Una computadora ejecuta operaciones muy simples. Pero la computadora no puede 
comprender el valor de una función matemática complicada por sí misma. 
Las computadoras pueden evaluar resultados de operaciones fundamentales, como sumar, 
dividir, entre otras de manera muy rápida y prácticamente cualquier cantidad de veces.

Un conjunto de comandos conocidos se llama lista de instrucciones.
Las computadoras entienden solamente el lenguaje máquina.

Las partes que componene un lenguaje son:

1. Un alfabeto: conjunto de símbolos utilizados para formar palabras de un determinado
   lenguaje.
2. Un léxico: conjunto de palabras que el lenguaje ofrece a sus usuarios.
3. Una sintáxis: conjunto de relgas formales o informales utilizadas para precisar si una 
   determinada cadena de palabras forma una oración válida (i.e "Soy una serpiente" a "Yo serpiente soy una").
4. Una semántica: conjunto de reglas que determinan si una frase tiene sentido (i.e "Me comí una dona" frente a "Una dona me comió").

Los lenguajes de programación de alto nivel son el puente entre los lenguajes máquina y el 
lenguaje natural. 
Un programa escrito en un lenguaje de programación de alto nivel se llama código fuente.

#### Compilación versus Interpretación.

Un programa no es más que una secuencia de instrucciones con la cuál se causará un efecto
deseado, la obtención de un objetivo. 
Tal composición debe ser correcta alfabética, lexica, sintáctica y semánticamente.

Luego, dicho programa escrito en un lenguaje debe ser traducido al lenguaje máquina para ser
ejecutado.
Existen dos formas de transformar un programa de un lenguaje de programación de alto nivel 
al de máquina:

**Compilación**
	El programa fuente se traduce una vez (esto se repite cada vez que se modifica el código 
	fuente), obtieniendo un archivo que contiene el código máquina. El programa encargado de 
	la traducción se llama compilador.

**Interpretación**
	El programa se puede traducir cada vez que se ejecuta. El programa que realiza esta 
	transformación se conoce como intérprete.

Python es un lenguaje interpretado.
Python alias CPython.
Además de las versiones de Python 2 y 3 , existen sus "implementaciones".
Python es mantenido por la Python Software Foundation. 
Originalmente Guido van Rossum utilizó el lenguaje de programación C para implementar la 
primera versión de su lenguaje. Gracias a que los Python's provenientes de la PSF está escritos
en C esto abre muchas puertas. La migración y portabilidad es más facil debido a que muchas 
plataformas tienen la capacidad de compilar y ejecutar programas en el lenguaje C.



<hr>
# Literals - Literales en Python

#literals

Utilizamos literales para codificar datos y colocarlos en el código.

    print("2")
    print(2)
	print(c)

Las primeras dos funciones imprimen una salida similar, pero no son iguales.
"2" es una cadena de caracteres y 2 es un literal de tipo entero. Por otra parte c no 
es nada por el momento.
Python posee a grandes rasgos tipos de números enteros y de coma flotante: *int* y *float*.

	print(1000)
	print(1_000)
Son iguales representaciones del número 1.000

	print(0o123) Octal
	print(0x123) Hexadecimal

Números flotantes: 

	print(7.2)
	print(.5)
	print(2.)
Estas son formas de escribir números de tipo flotante en Python.

Notación científica:
Se utiliza la letra *e*. Los textos utilizan la abreviación 3x10⁽⁸⁾
La base del primer número puede ser entero o flotante.

	print(3E8)
	print(3e8)

Python puede elegir una notación diferente en los outputs, por ejemplo:

	print(0.0000000000000000000001)
	output $ 1e-22
Python siempre elige la representación más corta.

Cadenas de caracteres:

	print("I'm your father")
	print('I\'m your father')
El backslash con la comilla simple es conocido como un caracter de escape.

Las cadenas pueden estar vacías. Aún así una cadena de caracteres vacía sigue siendo una 
cadena.

	print("")
	print('')

Literales booleanos:
Se utilizan para evaluar la veracidad.

	print(True < False)
	print(True > False)


Finalmente exite un literal especial en Python llamado None. Objeto de NoneType.
Se utiliza para representar la ausencia de un valor.

