# PRIMEROS PASOS EN JAVASCRIPT

## [Aprendiendo javascript con "MentoringJS Pretraining Step 2"](http://mentoringjs.com/)


El lenguaje en javascript fué creado en 1995 por Brendan Einch. ECMAScript es el nombre de la normal oficial, siendo JavaScript la más conocida de las implementaciones.

INCLUIR SCRIPTS EN PÁGINAS Y ARCHIVOS .JS

Hay al menos tres maneras de incluir código JavaScript en las páginas web.
	+ Escribir en el propio documento HTML mediante etiquetas <script type="text/javascript"></script>.
	+ En un archivo externo de tipo JavaScript(.js) que los documentos HTML enlazan mediante la etiqueta <script src="nombre_archivo.js"></script>
	+ Incluir javascript dentro de las propias etiquetas. Es la menos utilizada y tiene la desventaja que ensucia mucho el código.


SINTAXIS DE LENGUAJE.

	+ Es case sensitive, es decir, distingue entre mayúsculas y minúsculas. 
	+ Cada sentencia acaba con el carácter (;).
	+ Se pueden añadir comentarios. Estos pueden ser de una sola línea (//….) o de un bloque (/*....*/).

VARIABLES

Las vasrtiables en JavaScipt se utilizan mediante la palabra reservada 'var'. La parabra 'var' solamente se indica al definir por primera vez la variable, y a eso lo llamamos 'declarar' una variable.
					
					var num1 = 2;
					var num2 = 6;
					var res = num1 + num2;

El nombre de una variable también se le conoce como identificador y debe cumplir la siguiente normativa:
	+ El identificador únicamente puede estar formado por números,
	letras, y los símbolos '$' y '_' a lo sumo.
	+ El primer carácter del identificador no debe ser un número.

TIPOS DE DATOS

	+ NUMÉRICOS
		Se usan para contener valores numéricos enteros (llamados integer) o decimales (llamados float).

	+ CADENAS DE TEXTO
		Se usan para contener caracteres, palabras y/o frases de texto. Para darle el valor a la variable, se encierran los valores entre comillas dobles o simples, que delimitan el inicio y el final de la frase.


	+ ARRAYS
		También llamados vectores o matrices. Un array es una colección de variables. Los arrays sirven para guardar colecciones de valores, de manera que serviría para agrupar diferentes variables.

	+ BOOLEANOS
		Las variables de tipo booleano también son llamadas o denominadas con el nombre de variables de tipo lógico. Estas variables suelen servir para condiciones o para la programación lógica. Una variable este tipo solo puede almacenar dos valores: true (verdadero) o false (falso).

	+ OPERADORES
		Los operadores manipulas los valores de las variables, realizan cálculos matemáticos y comparan los valores de diferentes variables.


	+ ASIGNACIÓN
		Este operador es el principal y el más sencillo. Sirve para asignar un valor a una variable.

					var num1 = 3;

	
	+ INCREMENTO Y DECREMENTO
		Ambos operadores sirven para decrementar o incrementar el valor de una variable.

					var num = 5;
					++num;
					--num;
					num++; 
					num--;

		Cuando el operador ++ está como prefijo -> Su valor se incrementa antes de la operación.
		Cuando el operador ++ está como sufijo -> Su valor se incrementa después de la operación.

	
	+ NEGACIÓN
		El operador de negación se utiliza para dar el valor contrario a una variable. En el caso de una variable que tenga el valor de un booleano, se le asignará el valor contrario tras usarse el operador de negación.
		El operador de negación también se puede usar cuando el valor de la variable es un texto o un número. Si

	
	+ AND
		Este operador sirve para combinar los valores de dos variables, usando lógica matemática y solo dando true si ambos valores son true. En otro caso el valor final es false. El operador se define mediante el símbolo '&&'.
	

	+ OR
		Este operador sirve para combinar los valores de dos variables, usando lógica matemática y solo dando true si alguno de los valores es true.
		En otro caso el valor final es false. El operador se define mediante el símbolo '||'.
	

	+ MATEMÁTICOS
		Los operadores declarados son: suma (+), resta (-), multiplicación (*) y división (/).

	
	+ RELACIONALES
		Los relacionales: mayor que (>), menor que (<), mayor o igual (>=), menor o igual (<=), igual que (==) y distinto de (!=). El resultado de ellos siempre es un valor de booleano.


Para realizar este trabajo he consultado los apuntes del curso impartido por la fundación telefónica de Desarrollo web en PHP. Además de consultar también este libro [Speaking Javascript](http://speakingjs.com/es5/index.html), concretamente este capítulo [I. JavaScript Quick Start](http://speakingjs.com/es5/pt01.html).


Un saludo!!