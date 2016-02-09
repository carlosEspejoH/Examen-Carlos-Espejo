Ciclo �gil,prioridades,historias, estimaciones y definiciones de "Hecho".


	Prioridad	Historia	Estimaci�n	Hecho
	   1     	N�sNaturales        3           Comprueba que de lo que le entra solo acepta los numeros naturales (digito positivo y entero).Historia utilities.
	   2     	Suma 		    2     	Comprueba que suma correctamente dos numeros. Se usa la funcionalidad de comprobar que son naturales.Historia 1.
	   3 		Multiplicaci�n	    2     	Comprueba que multiplica correctamente dos numeros. Se usa la funcionalidad de comprobar que son naturales.Historia 2.
	   4   		Resta 		    2    	Comprueba que resta correctamente dos numeros. Se usa la funcionalidad de comprobar que son naturales.Historia 3.
	   5 		ErrorResta          3           Comprueba que el resultado de la resta es natural y muestra un error si no se puede realizar la resta.Historia 4.
  	   6   		n�sRomanos 	    4   	Comprueba que pasa un n�mero romano a natural y con ello puede ser usado en las dem�s aplicaciones. Historia 5.

Notas: Supongo que tengo recursos ilimitados, en mi caso necesito 3 trabajadores, ya que una vez terminada la funcion de detectar que los numeros son 
naturales ( que es bloqueante a la suma, resta y multiplicaci�n) las 3 funciones se trabajan en paralelo. 

Una vez acabada la resta, se trabaja la funcion ErrorResta, ya que la resta es bloqueante para esta funci�n

La funci�n numeros romanos solo pasa de numeros romanos a naturales para ser usados por las demas funciones. No es bloqueada por ninguna pero al ser 
opcional y la menos prioritaria seg�n el cliente (el enunciado) se deja para hacerla en paralelo con ErrorResta.

La prioridad la marca el cliente (el enunciado) seg�n lo indicado por el product owner (V�ctor) al equipo de trabajo.

Se aplica la metodolog�a TDD por lo que se definen unos requisitos que deben cumplir las funciones y unas pruebas para comprobar que se cumplen antes de 
escribir el c�digo de las funciones.

Las funciones bloqueantes son (por si no ha quedado claro):
Funci�n n�meros naturales para la suma multiplicaci�n y la resta
Funci�n resta para la funci�n ErrorResta.

EXPLICACI�N DEL GIT:

Commit Inicial: README y gitignore aunque no se use el gitignore de momento es �til que este en los proyectos por si en alg�n punto se necesita.

Requisitos y pruebas TDD: Requisitos que deben cumplir la funcion N�s naturales. Que sea un digito, que sea positivo, que sea entero.

C�digo que comprueba que son naturales: 

Prueba naturales: Compruebo con Red-Green-Refactor

Creo las ramas Hist1Suma, Hist2Multiplicaci�n, Hist3Resta

Requisitos y test de la ( Suma, Multiplicaci�n, Resta,):Planear test y pruebas para cada funci�n, por ejemplo:
Que 1 + 3 =4 para la suma, que 5-2=3 para la resta y que 3*7=21 para la multiplicaci�n.

C�digo de la (Suma, Multiplicaci�n, Resta): Llamada a la funci�n previamente programada que comprueba que son naturales y
c�digo en el lenguaje que sea que haga la funci�n indicada.

Pruebas de la (Suma, Multiplicaci�n, Resta): Pruebas de que correctamente el c�digo hace que 1 + 3 =4 para la suma, 
que 5-2=3 para la resta y que 3*7=21 para la multiplicaci�n. Compruebo con m�todo Red-Green-Refactor.

Merge (Suma, Multiplicaci�n, Resta) con master (rama ppal). Solapa suma con master ya que master no aporta cambios.

Creo las ramas Hist4ErroresResta y Hist5Romanos

Requisitos y test de la ( Hist4ErroresResta, Hist5Romanos):Planear test y pruebas para cada funci�n, por ejemplo:
 2 - 12 =-10 muestra "error" para Hist4ErroresResta  y  VI=6 para Hist5Romanos

C�digo de la Hist4ErroresResta:Comprueba que el resultado de la funci�n previamente rehalizada Resta es un n�mero natural y se puede realizar la resta,
sino manda mensaje. Despu�s, c�digo en el lenguaje que sea que haga la funci�n indicada.

C�digo de la Hist5Romanos: c�digo en el lenguaje que sea que haga la funci�n indicada.

Pruebas de la (Suma, Multiplicaci�n, Resta): Pruebas de que correctamente el c�digo hace que  2 - 12 =-10 muestra "error" para Hist4ErroresResta  y  VI=6 para Hist5Romanos

Merge Hist4ErroresResta y Hist5Romanos con master (rama ppal). Solapa Hist4ErroresResta con master ya que master no aporta cambios.













