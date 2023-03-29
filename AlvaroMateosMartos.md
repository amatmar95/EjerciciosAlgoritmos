## Primeros 3 ejercicios



### Ejercicio 1



*Calcular la letra del DNI Español*



**Paso 1**: Definir el problema: A partir de un número de DNI hemos de calcular la letra.

 ¿Cómo se calcula la letra del DNI?

- Número del DNI debe tener 8 dígitos, este DNI hay que dividirlo entre 23 y el resto será el ``resultadoResto``.

El ``resultadoResto`` lo compararemos con la lista de códigos de la siguiente tabla de letras ``tablaLetrasDNI``.



| ```resultadoResto``` | Letra |
| -------------------- | ----- |
| 0                    | T     |
| 1                    | R     |
| 2                    | W     |
| 3                    | A     |
| 4                    | G     |
| 5                    | M     |
| 6                    | Y     |
| 7                    | F     |
| 8                    | P     |
| 9                    | D     |
| 10                   | X     |
| 11                   | B     |
| 12                   | N     |
| 13                   | J     |
| 14                   | Z     |
| 15                   | S     |
| 16                   | Q     |
| 17                   | V     |
| 18                   | H     |
| 19                   | L     |
| 20                   | C     |
| 21                   | K     |
| 22                   | E     |

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``DNI`` , ``tablaLetrasDNI``, resultado = ""

Proceso: 

- Validar que el ``DNI``  tenga 8 dígitos

  ​      · Si es errónea asignar a la variable ``resultado`` "DNI Inválido"

- Dividimos ``DNI`` en 23 y el resto lo asignamos a ``resultadoResto``

- Comparar el ``resultadoResto`` con los valores de la tabla y asignar a ``resultado`` el valor equivalente en la tabla.

Salida:

- Escribir ``resultado``

**Paso 3**: Escribir el pseudocódigo



```

Algoritmo CalculoDNI

  # Entrada
  DNI<-leer()
  tablaLetrasDNI<-"TRWAGMYFPDXBNJZSQVHLCKE"
  resultado<-""
  
  # Proceso
  Si DNI es válido Entonces
  		resultadoResto<-DNI mod 23 #mod es el resto de dividir
  		resultado<-recuperarLetra(resultadoResto,tablaLetrasDNI)
  sino
  		resultado<-"DNI Invalido"
  Fin si
  
  # Salida

Fin Algoritmo

```





### Ejercicio 2

*Calcular el salario de un empleado*

**Paso 1**: Definir el problema:

El salario en España se calcula a partir del salario bruto anual, que incluye todas las percepciones económicas que recibe un trabajador durante el año, incluyendo salario base, paga extras, complementos y otros conceptos retributivos.



**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``salario base``,  ``pagas extras``, ``complementos``, ``otrosConceptosRetributivos``.

``IRPF``, ``Seguridad Social``.

Proceso: 

- Sumar ``salarioBase``,  ``pagasExtras``, ``complementos``, ``otrosConceptosRetributivos`` y lo asigno a ```salarioBruto```.
- Sumar ``IRPF``, ``Seguridad Social``y lo asigno a ``deducciones``.
- ``salarioNeto`` asigna ``salarioBruto``  - ``deducciones``



Salida:

Escribir (````salarioBruto`` , ``salarioNeto``)

**Paso 3**: Escribir el pseudocódigo



```

Algoritmo 

  # Entrada
salarioBase<-Leer()
pagasExtras<-Leer()
complementos<-Leer()
otrosConceptosRetributivos<-Leer()
IRPF<-Leer()
Seguridad Social<-Leer()
  # Proceso
salarioBruto<-salarioBase+pagasExtras+complementos+otrosConceptosRetributivos
deducciones<-IRPF+Seguridad Social
salarioNeto<-salarioBruto-deducciones
  # Salida
Escribir(salarioBruto, salarioNeto)
Fin Algoritmo

```





### Ejercicio 3

*Determinar la ruta para llegar a una ciudad por avión.*

**Paso 1**: Definir el problema.

Necesitamos calcular el trayecto que realizara un avión para llegar de una ciudad a otra

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``avion``,  ``ciudadOrigen``, ``ciudadDestino``

Proceso: 

- .
- .
- .

Salida:

Escribir (``ruta``)

**Paso 3**: Escribir el pseudocódigo



```

Algoritmo 

  # Entrada
	avion <-Leer()
	ciudadOrigen<-Leer()
	ciudadDestino<-Leer()	
  # Proceso

  # Salida
	Escribir (ruta)
Fin Algoritmo

```







### Ejercicio 4

*Calcula el área y perímetro de un círculo dado su radio*

**Paso 1**: Definir el problema:

Dado el radio de un círculo, debemos calcular el área y el perímetro del mismo.

El área de un circulo se calcula con la fórmula: A= R^2 x Pi

El perímetro de un circulo se calcula con la fórmula: P= R X 2 x Pi

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``radioCirculo``

Proceso: 

- Multiplicar el ``radioCirculo`` elevado al cuadrado x el numero Pi.
- Asignar el resultado a la variable ``areaCirculo``.
- Multiplicar el ``radioCirculo`` x 2 y x el número Pi.
- Asignar dicho resultado a la variable ``perimetroCirculo``.



Salida:

Escribir (``areaCirculo , perimetroCirculo``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
radioCirculo<-Leer()
  # Proceso
areaCirculo <- (radioCirculo)^2 x Pi
perimetroCirculo <- radioCirculo x 2 x Pi
  # Salida
Escribir(areaCirculo, perimetroCirculo)
Fin Algoritmo

```







### Ejercicio 5

*Dada una lista de números enteros, determina cuál es el mayor y cuál es el menor*

**Paso 1**: Definir el problema:

Teniendo una lista de números enteros, debemos determinar cual es el número mayor y el número menor de dicha lista

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``listaNumeros``

Proceso: 

- Determinar un numero de la ``listaNumeros`` como el mayor y asignarlo a la variable ``numeroMayor``, e ir comparando con los siguientes números de la ``listaNumeros``.
- Si el número con el que comparamos es mayor que el que tenemos asignado, se reasignara el valor de la variable y dicho número pasara a ser ``numeroMayor``, si no, el ``numeroMayor`` sigue siendo el que teníamos asignado.
- Determinar un numero de la ``listaNumeros`` como el menor y asignarlo a la variable ``numeroMenor``, e ir comparando con los siguientes números de la ``listaNumeros``.
- Si el número con el que comparamos es menor que el que tenemos asignado, se reasignara el valor de la variable y dicho número pasara a ser ``numeroMenor``, si no, el ``numeroMenor`` sigue siendo el que teníamos asignado.



Salida:

Escribir (``numeroMayor , numeroMenor``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
listaNumeros<-Leer()
  # Proceso
numeroMayor <- num1>num2
numeroMenor <- num1<num2
  # Salida
Escribir(numeroMayor, numeroMenor)
Fin Algoritmo

```



### Ejercicio 6

*Crea un algoritmo que convierta grados Celsius a Fahrenheit.*

**Paso 1**: Definir el problema:

Teniendo una entrada en la que  escribimos un número que corresponderá a la temperatura en grados Celsius, deberemos transformar dicha temperatura a Fahrenheit.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``gradosCelsius``

Proceso: 

- Multiplicar ``gradosCelsius`` x 1,8.
- A ese resultado le sumamos 32.
- El resultado total que obtengamos los asignamos a la variable ``fahrenheit``.

Salida:

Escribir (``fahrenheit``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
gradosCelsius<-Leer()
  # Proceso
fahrenheit <- (gradosCelsius x 1.8) + 32
  # Salida
Escribir(fahrenheit)
Fin Algoritmo

```







### Ejercicio 7

*Dado un número entero, crea un algoritmo que determine si es par o impar*

**Paso 1**: Definir el problema:

Teniendo un número entero dado, debemos determinar si dicho número es par o impar.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``numero``

Proceso: 

- Dividir ``numero`` entre 2.
- Si el resto de esa división es 0, el número es par y la variable ``esPar`` es true. Entonces escribimos la variable ``esPar``.
- Si por el contrario el resto es diferente de 0, el número es impar y la variable ``esImpar`` es true. Entonces escribimos la variable ``esImpar``.

Salida:

Escribir (``esPar``,``esImpar``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
numero<-Leer()
  # Proceso
esPar <- numero mod 2 == 0
esImpar <- numero mod 2 != 0
  # Salida
Escribir(esPar, esImpar)
Fin Algoritmo

```







### Ejercicio 8

*Crea un algoritmo que determine si un año es bisiesto o no*

**Paso 1**: Definir el problema:

Dado un año, debemos determinar si dicho año es bisiesto o no.

Un año es bisiesto si es:

- Divisible entre 4.
- No divisible entre 100.
- Divisible entre 400. (2000 y 2400 son bisiestos pues aún siendo divisibles entre 100 lo son también entre 400. Pero los años 1900, 2100, 2200 y 2300 no lo son porque solo son divisibles entre 100).

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``año``

Proceso: 

- Dividir ``año`` entre 4.
- Dividir ``año``entre 100
- Dividir ``año`` entre 400
- Si el resto de dividir  ``año`` entre 4 es igual a 0, y el resto de dividir ``año`` entre 100 es diferente de 0, o el resto de dividir entre 400 es igual a 0, el año es bisiesto y la variable ``esBisiesto`` es true y escribimos dicha variable
- En caso contrario, ``año`` no es bisiesto y la variable ``esBisiesto`` es false. Entonces escribimos la variable como false y decimos que no es bisiesto

Salida:

Escribir (``esBisiesto``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
año<-Leer()
  # Proceso
esBisiesto <- (año mod 4 == 0) && (año mod 100 != 0) || (año mod 400 == 0 )
  # Salida
Escribir(esBisiesto)
Fin Algoritmo

```





### Ejercicio 9

*Crea un algoritmo que determine si una cadena de texto es un palíndromo o no.*

**Paso 1**: Definir el problema:

Dada una cadena de texto debemos determinar si dicha cadena es un palíndromo o no

Un palíndromo es una palabra o expresión que es igual si se lee de izquierda a derecha que de derecha a izquierda.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``cadenaTexto``

Proceso: 

- Escribir ``cadenaTexto`` empezando por el final y asignarlo a la variable ``cadenaTextoInversa``.
- Comprobar si ``cadenaTexto`` y ``cadenaTextoInversa`` son iguales.
- Si son iguales, la variable ``esPalindromo`` es true. En caso contrario, la variable ``esPalindromo`` será false.
- Escribimos la variable ``esPalindromo``.

Salida:

Escribir (``esPalindromo``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
cadenaTexto<-Leer()
  # Proceso
cadenaTextoInversa<- Escribir cadenaTexto empezando por el final
cadenaTexto = cadenaTextoInversa <- esPalindromo = true
cadenaTexto != cadenaTextoInversa <- esPalindromo = false
  # Salida
Escribir(esPalindromo)
Fin Algoritmo

```







### Ejercicio 10

*Dada una lista de nombres, crea un algoritmo que ordene la lista alfabéticamente.*

**Paso 1**: Definir el problema:

Dada una lista de nombres, ordenar dichos nombres por orden alfabético.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``listaNombres``

Proceso: 

- Determinar un nombre  de la ``listaNombres`` como el primero de la nueva ``listaOrdenada``.
- Después, debemos ir comparando con los siguientes nombres de la ``listaNombres``.
- Si el nombre es posterior alfabéticamente, lo asignamos después del nombre que teníamos como el primero en ``listaOrdenada``, en caso contrario, lo asignamos antes del nombre que teníamos como primero, que pasa a ser el segundo  de ``listaOrdenada`` momentáneamente.

Salida:

Escribir (``listaOrdenada``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
listaNombres<-Leer()
  # Proceso
listNombres <- nombre1 < nombre2
listaOrdenada <- nombre1
  # Salida
Escribir(listaOrdenada)
Fin Algoritmo

```





### Ejercicio 11

*Crea un algoritmo que calcule el factorial de un número entero.*

**Paso 1**: Definir el problema:

Dado un número entero, calcular el factorial del mismo.

El factorial de un número es igual al producto de todos los números enteros positivos desde 1 hasta dicho número.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``numero``

Proceso: 

- Multiplicar todos los números enteros positivos hasta llegar al número dado, incluido el mismo.
- El resultado de dichas multiplicaciones lo asignamos a la variable ``factorial``.

Salida:

Escribir (``factorial``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
numero<-Leer()
  # Proceso
factorial <- 1x2x3x...x numero
  # Salida
Escribir(factorial)
Fin Algoritmo

```





### Ejercicio 12

*Dado un número entero, crea un algoritmo que determine si es primo o no.*

**Paso 1**: Definir el problema:

Dado un número entero, debemos determinar si dicho número es primo o no.

Un número es primo si solo es divisible entre 1 y entre sí mismo.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``numero``

Proceso: 

- Dividir ``numero`` entre cada número desde 1 hasta el propio ``numero``
- Si solamente el resto de dividir ``numero`` entre 1 y ``numero`` entre el propio ``numero`` es igual a 0, y los restos de dividir ``numero`` entre el resto de números entre 1 y el propio ``numero`` son diferentes de 0, el ``numero`` es primo y la variable ``esPrimo``será true. En caso contrario, la variable ``esPrimo`` será false.
- Escribimos la variable ``esPrimo``.

Salida:

Escribir (``esPrimo``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
numero<-Leer()
  # Proceso
esPrimo <- (numero mod 1 == 0) && (numero mod numero == 0) && (numero mod restodenumeros != 0) = true
  # Salida
Escribir(esPrimo)
Fin Algoritmo

```





### Ejercicio 13

*Crea un algoritmo que calcule el área y volumen de un cubo dado su lado.*

**Paso 1**: Definir el problema:

Dado un lado de un cubo, debemos calcular el área y el volumen del mismo.

El área de un cubo se calcula con la fórmula: A= (Lado x Lado) x 6

El volumen de un cubo se calcula con la fórmula: V = Lado^3



**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``ladoCubo``

Proceso: 

- Multiplicar el ``ladoCubo`` x ``ladoCubo`` para obtener el área de una de las caras del cubo. Es resultado lo multiplicamos x 6, que corresponde a las 6 caras del cubo. El resultado obtenido de dicha fórmula lo asignamos a la variable ``areaCubo``.
- Realizar la fórmula de ``ladoCubo`` elevado a 3. El resultado obtenido o asignamos a la variable ``volumenCubo``.



Salida:

Escribir (``areaCubo , volumenCubo``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
ladoCubo<-Leer()
  # Proceso
areaCubo <- (ladoCubo x ladoCubo) x 6
volumenCubo <- ladoCubo^3
  # Salida
Escribir(areaCubo, volumenCubo)
Fin Algoritmo

```





### Ejercicio 14

*Dada una lista de números enteros, crea un algoritmo que calcule la suma de todos los números pares de la lista.*

**Paso 1**: Definir el problema:

Dado una lista de números, debemos calcular la suma de todos los números pares.

Para saber si un número es par, el resto de dividir dicho número entre 2 debe ser 0.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``listaNumeros``

Proceso: 

- Dividir cada número de la lista entre 2. Si el resto es 0, asignamos dicho número a la ``listaPares``.
- Posteriormente, una vez hayamos terminado de dividir todos los números de la ``listaNumeros`` y tengamos terminada la ``listaPares``, sumamos todos los números de la ``listaPares``, y el resultado lo asignamos a la variable ``sumaPares``



Salida:

Escribir (``sumaPares``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
listaNumeros<-Leer()
  # Proceso
listaNumeros <- num1 mod 2 == 0 
listaPares <- num1
sumaPares <- num1(listaPares) + num2(listaPares) + ...
  # Salida
Escribir(sumaPares)
Fin Algoritmo

```





### Ejercicio 15

*Crea un algoritmo que determine si un número es positivo, negativo o cero.*

**Paso 1**: Definir el problema:

Dado un número, debemos determinar si dicho número es positivo, negativo, o cero.

El número será positivo si es mayor que 0, y negativo si es menor que 0.

Para saber si un número es par, el resto de dividir dicho número entre 2 debe ser 0.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``numero``

Proceso: 

- Comprobar si el ``numero`` es mayor, menor, o igual a 0.
- Si el ``numero`` es mayor que 0, la variable ``esPositivo`` será true, y las variables ``esNegativo`` y ``esCero`` serán false.
- Si el ``numero`` es menor que 0, la variable ``esNegativo`` será true, y las variables ``esPositivo`` y ``esCero`` serán false.
- Si el ``numero`` es igual a 0,  la variable ``esCero`` será true, y las variables ``esPositivo`` y ``esNegativo`` serán false.



Salida:

Escribir (``esPositivo, esNegativo, esCero``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
numero<-Leer()
  # Proceso
esPositivo <- numero > 0
esNegativo <- nnumero < 0
esCero <- numero == 0
  # Salida
Escribir(esPositivo, esNegativo, esCero)
Fin Algoritmo

```





### Ejercicio 16

*Dada una lista de números enteros, crea un algoritmo que calcule la media de la lista.*

**Paso 1**: Definir el problema:

Dado una lista de números, debemos calcular una media de todos los números de dicha lista.

Para calcular la media, deberemos sumar todos los números de la lista, y después dividir la suma entre la cantidad de números que tiene la lista.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``listaNumeros``

Proceso: 

- Sumar todos los números de ``listaNumeros`` y asignar el resultado a la variable ``suma``
- Dividir la variable ``suma`` entre la cantidad de números que hemos sumado, que son los que tiene la ``listaNumeros``.
- Asignamos el resultado de la división a la variable ``media``
- Escribimos ``media``



Salida:

Escribir (``media``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
listaNumeros<-Leer()
  # Proceso
suma <- num1 + num2 + ...
media <- suma / cantidad de números sumados
  # Salida
Escribir(media)
Fin Algoritmo

```







### Ejercicio 17

*Crea un algoritmo que genere un número aleatorio entre 1 y 100, y le pida al usuario adivinarlo. El algoritmo deberá indicar si el número introducido es mayor o menor que el número aleatorio, hasta que el usuario adivine el número correcto.*

**Paso 1**: Definir el problema:

Debemos crear un algoritmo que genere un número aleatorio del 1 al 100. El usuario debe intentar adivinarlo, y el algoritmo irá diciéndole al usuario si el número introducido es mayor o menor que el generado para que vaya acercándose.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``numeroUsuario``

Proceso: 

- Generar ``numeroAleatorio`` del 1 al 100
- Pedir al usuario que introduzca un ``numeroUsuario`` para intentar adivinarlo
- El programa dirá al usuario si ``numeroUsuario`` es mayor o menor que ``numeroAleatorio``
- El programa pedirá al usuario otro ``numeroUsuario``
- Se repetirá el mismo proceso hasta que ``numeroUsuario`` sea igual que ``numeroAleatorio``.



Salida:

Escribir (``numeroALeatorio``, ``numeroUsuario``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
numeroUsuario<-Leer()
  # Proceso
numeroAleatorio
numeroUsuario <- numeroUsuario == numeroAleatorio
numeroUsuario <- numeroUsuario <> numeroAleatorio
numeroUsuario
  # Salida
Escribir(numeroUsuario, numeroAleatorio)
Fin Algoritmo

```







### Ejercicio 19

*Dada una lista de números enteros, crea un algoritmo que elimine los números duplicados de la lista*

**Paso 1**: Definir el problema:

Teniendo una lista dada de números enteros, debemos crear un algoritmo que elimine los números duplicados de la misma.

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``listaNumeros``

Proceso: 

- Recorrer la ``listaNumeros`` desde el primero de ellos.
- Comparar el primer número con el resto de la ``listaNumeros``.
- Si encuentra otro número igual, eliminar uno de ellos, y guardar uno en la variable ``listaCorregida``
- Después, realizar el mismo proceso con el segundo número de la ``listaNumeros``, y lo haremos sucesivamente con todos los números.

Salida:

Escribir (``listaCorregida``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
listaNumeros<-Leer()
  # Proceso
listaNumeros <- num1 != num2 != num3 ...
listaCorregida <- num1...
  # Salida
Escribir(listaCorregida)
Fin Algoritmo

```







### Ejercicio 20

*Crea un algoritmo que determine si un número es capicúa o no*

**Paso 1**: Definir el problema:

Dado un número, debemos determinar si dicho número es capicúa o no.

Un número será capicúa si se lee igual tanto de izquierda a derecha como de derecha a izquierda

**Paso 2**: Poner la entrada, el proceso y la salida

Entrada: ``numero``

Proceso: 

- Escribir ``numero`` empezando por el final y asignarlo a la variable ``numeroInverso``.
- Comprobar si ``numero`` y ``numeroInverso`` son iguales.
- Si son iguales, la variable ``esCapicua`` es true. En caso contrario, la variable ``esCapicua`` será false.
- Escribimos la variable ``esCapicua``.

Salida:

Escribir (``esCapicua``)

**Paso 3**: Escribir el pseudocódigo



```
Algoritmo 

  # Entrada
numero<-Leer()
  # Proceso
numeroInverso<- Escribir numero empezando por el final
numero = numeroInverso <- esCapicua = true
numero != numeroInverso <- esCapicua = false
  # Salida
Escribir(esCapicua)
Fin Algoritmo

```

