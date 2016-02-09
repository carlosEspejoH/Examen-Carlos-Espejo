Ciclo ágil,prioridades,historias, estimaciones y definiciones de "Hecho".


	Prioridad	Historia	Estimación	Hecho
	   1     	NºsNaturales        3           Comprueba que de lo que le entra solo acepta los numeros naturales (digito positivo y entero).Historia utilities.
	   2     	Suma 		    2     	Comprueba que suma correctamente dos numeros. Se usa la funcionalidad de comprobar que son naturales.Historia 1.
	   3 		Multiplicación	    2     	Comprueba que multiplica correctamente dos numeros. Se usa la funcionalidad de comprobar que son naturales.Historia 2.
	   4   		Resta 		    2    	Comprueba que resta correctamente dos numeros. Se usa la funcionalidad de comprobar que son naturales.Historia 3.
	   5 		ErrorResta          3           Comprueba que el resultado de la resta es natural y muestra un error si no se puede realizar la resta.Historia 4.
  	   6   		nºsRomanos 	    4   	Comprueba que pasa un número romano a natural y con ello puede ser usado en las demás aplicaciones. Historia 5.

Notas: Supongo que tengo recursos ilimitados, en mi caso necesito 3 trabajadores, ya que una vez terminada la funcion de detectar que los numeros son 
naturales ( que es bloqueante a la suma, resta y multiplicación) las 3 funciones se trabajan en paralelo. 

Una vez acabada la resta, se trabaja la funcion ErrorResta, ya que la resta es bloqueante para esta función

La función numeros romanos solo pasa de numeros romanos a naturales para ser usados por las demas funciones. No es bloqueada por ninguna pero al ser 
opcional y la menos prioritaria según el cliente (el enunciado) se deja para hacerla en paralelo con ErrorResta.

La prioridad la marca el cliente (el enunciado) según lo indicado por el product owner (Víctor) al equipo de trabajo.

Se aplica la metodología TDD por lo que se definen unos requisitos que deben cumplir las funciones y unas pruebas para comprobar que se cumplen antes de 
escribir el código de las funciones.

Las funciones bloqueantes son (por si no ha quedado claro):
Función números naturales para la suma multiplicación y la resta
Función resta para la función ErrorResta.

EXPLICACIÓN DEL GIT:

Commit Inicial: README y gitignore aunque no se use el gitignore de momento es útil que este en los proyectos por si en algún punto se necesita.

Requisitos y pruebas TDD: Requisitos que deben cumplir la funcion Nºs naturales. Que sea un digito, que sea positivo, que sea entero.

Código que comprueba que son naturales: 

Prueba naturales: Compruebo con Red-Green-Refactor

Creo las ramas Hist1Suma, Hist2Multiplicación, Hist3Resta

Requisitos y test de la ( Suma, Multiplicación, Resta,):Planear test y pruebas para cada función, por ejemplo:
Que 1 + 3 =4 para la suma, que 5-2=3 para la resta y que 3*7=21 para la multiplicación.

Código de la (Suma, Multiplicación, Resta): Llamada a la función previamente programada que comprueba que son naturales y
código en el lenguaje que sea que haga la función indicada.

Pruebas de la (Suma, Multiplicación, Resta): Pruebas de que correctamente el código hace que 1 + 3 =4 para la suma, 
que 5-2=3 para la resta y que 3*7=21 para la multiplicación. Compruebo con método Red-Green-Refactor.

Merge (Suma, Multiplicación, Resta) con master (rama ppal). Solapa suma con master ya que master no aporta cambios.

Creo las ramas Hist4ErroresResta y Hist5Romanos

Requisitos y test de la ( Hist4ErroresResta, Hist5Romanos):Planear test y pruebas para cada función, por ejemplo:
 2 - 12 =-10 muestra "error" para Hist4ErroresResta  y  VI=6 para Hist5Romanos

Código de la Hist4ErroresResta:Comprueba que el resultado de la función previamente rehalizada Resta es un número natural y se puede realizar la resta,
sino manda mensaje. Después, código en el lenguaje que sea que haga la función indicada.

Código de la Hist5Romanos: código en el lenguaje que sea que haga la función indicada.

Pruebas de la (Suma, Multiplicación, Resta): Pruebas de que correctamente el código hace que  2 - 12 =-10 muestra "error" para Hist4ErroresResta  y  VI=6 para Hist5Romanos

Merge Hist4ErroresResta y Hist5Romanos con master (rama ppal). Solapa Hist4ErroresResta con master ya que master no aporta cambios.













