# Tarea 1
# VENTAS POR COMISION
```
Algoritmo VentasPorComision
	Definir total, cantidad, i, valr, comisionVentas Como Entero
	Definir comision como real
	i<-1
	comision<-0
	Escribir "Ventas realizadas en el mes:"
	Leer  cantidad
	Mientras (i<=cantidad) Hacer
		Escribir "Ingrese la venta ", i ":"
		Leer valr
		total<-total+valr
		i<-i+1
	FinMientras
	Si (total>3000) Entonces
		comision<-total*0.10
		comisionVentas<-total+comision
		Escribir "La comisión fue: ",comision
		Escribir "El total con comisión es: ",comisionVentas
	FinSi
	Escribir "El total en ventas es: ",total
FinAlgoritmo
```
(revisar codigo ya que solo permite numeros enteros)

#  Tarea 2
# NUMERO PAR IMPAR
```
Algoritmo numeroParImpar
	Repetir
		Escribir 'Pon un número entre 0 y 50.'
		leer n
		SI  n < 0  y n > 50 Entonces
			Imprimir "Veamos pares: "
			Imprimir 'Número inválido.'
		FinSi
	Mientras Que n < 0  y n > 50
	
	par =  n % 2 = 0
	
	Para i=1 Hasta n Con Paso 1 Hacer
		SI i % 2 = 0 & par Entonces
			Imprimir i
		FinSi
		SI i % 2 = 1 & ~(par) Entonces
			Imprimir i
		FinSi
	FinPara
	
FinAlgoritmo
```

# Tarea 3
# NOMBRE COMPLETO
```
Algoritmo nombreCompleto
	Definir nombre Como Caracter
	Definir n,x,c Como Entero
	Escribir "Escribe tu nombre: "
	Leer nombre 
	n = longitud(nombre)
	c = 0
	para x = 1 Hasta n Con Paso 1 Hacer
		si  x == 1 Entonces
			Escribir Mayusculas(Subcadena(nombre,x,x)) Sin Saltar
		SiNo
			si Subcadena(nombre,x,x) == " " Entonces
				c = 1
			SiNo
				si c == 1 Entonces
					Escribir " ",Mayusculas(Subcadena(nombre,x,x)) Sin Saltar
					c = 0
				SiNo
					Escribir Subcadena(nombre,x,x) Sin Saltar
					
					
				FinSi
				
			FinSi
		FinSi
	FinPara
	
	Escribir " "
FinAlgoritmo

```

# Tarea 4
# DADOS
```
Funcion resultado<-Tirada()
	Definir  resultado,i Como Entero
	i=0;
	resultado=azar(6)+1+azar(6)+1;
	Escribir "Pulsa cualquier tecla para tirar los dados.";
	Esperar Tecla;
	Escribir "Tirando los dados"
	Para i<-0 Hasta 20 Con Paso 1 Hacer
		Escribir "*" Sin Saltar;
		Esperar 100 Milisegundos;
		
	FinPara
	Escribir " ";
	Escribir resultado;
FinFuncion

Algoritmo  Craps1
	Definir i,resultado Como Entero;
	i=0;
	Para i<-0 Hasta 20 Con Paso 1 Hacer
		resultado=Tirada();
		
	FinPara
```

# Tarea 5
# DISTACIA A CERO
```
Algoritmo DistanciaACero
	definir cant, cantTrunc Como Real
	Escribir "Escriba un numero"
	leer cant
	cantTrunc = Trunc(cant)
	Dimension nums[cant]

	Para i<-1 Hasta 5 Con Paso 1 Hacer
		Escribir "Escribir un numero"
		Leer nums[i]
		
		Escribir abs(i)
		Escribir Trunc(-i)
		Escribir redon(i)
		
	FinPara

	mayr<-nums[i]
	
	si (nums[i]>mayr) Entonces
		mayr<-nums[i]
	FinSi
	si (nums[i]>menr) Entonces
		menr<-nums[i]
	
	FinSi
Escribir "Este es el mas lejano a cero."

FinAlgoritmo
```
(codigo incompleto)	

# Tarea 6
# LANZAR MONEDAS
```
Algoritmo LanzarMoneda
    Definir nombrePrimerJugador, nombreSegundoJugador como Cadena
    Definir cantidadPrimerJugador, cantidadSegundoJugador como Entero
	
    Imprimir "Ingrese el nombre del primer jugador"     // Pide al usuario que ingrese el nombre del primer jugador
    Leer nombrePrimerJugador                           // Lee el nombre del primer jugador ingresado por el usuario
    Imprimir "Escriba la cantidad para jugar"          // Solicita al usuario que ingrese la cantidad con la que desea jugar
    Leer cantidadPrimerJugador                         // Lee la cantidad ingresada por el primer jugador
	
    Imprimir "Ingrese el nombre del segundo jugador"    // Pide al usuario que ingrese el nombre del segundo jugador
    Leer nombreSegundoJugador                           // Lee el nombre del segundo jugador ingresado por el usuario
    Imprimir "Escriba la cantidad para jugar"           // Solicita al usuario que ingrese la cantidad con la que desea jugar
    Leer cantidadSegundoJugador                         // Lee la cantidad ingresada por el segundo jugador
	
    Si cantidadPrimerJugador <= 0 y cantidadSegundoJugador <= 0 Entonces
        Imprimir "Juego Cancelado"                      // Si ambas cantidades son menores o iguales a cero, imprime "Juego Cancelado"
    Sino
        Si cantidadPrimerJugador <= 0 Entonces
            Imprimir "Gana: ", nombreSegundoJugador     // Si la cantidad del primer jugador es menor o igual a cero, imprime "Gana: " seguido del nombre del segundo jugador
        Sino Si cantidadSegundoJugador <= 0 Entonces
				Imprimir "Gana: ", nombrePrimerJugador   // Si la cantidad del segundo jugador es menor o igual a cero, imprime "Gana: " seguido del nombre del primer jugador
			Sino
				Definir ganadorAleatorio como Entero      // Si ninguna cantidad es menor o igual a cero, define la variable "ganadorAleatorio" como entero
				ganadorAleatorio = Aleatorio(1, 2)         // Genera un número aleatorio (1 o 2) para simular el lanzamiento de la moneda
				Si ganadorAleatorio = 1 Entonces
					Imprimir "Jugador ganador: ", nombrePrimerJugador, ", cantidad que gana: ", cantidadPrimerJugador     // Si el número aleatorio es 1, imprime el nombre del primer jugador como ganador junto con la cantidad que gana
				Sino
					Imprimir "Jugador ganador: ", nombreSegundoJugador, ", cantidad que gana: ", cantidadSegundoJugador   // Si el número aleatorio es 2, imprime el nombre del segundo jugador como ganador junto con la cantidad que gana
				FinSi
			FinSi
		FinSi
	FinSi
FinAlgoritmo

# Tarea 7
#
	

	
	
