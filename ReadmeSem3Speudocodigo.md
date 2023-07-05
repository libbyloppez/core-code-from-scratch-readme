# Tarea 1
# CALCULADORA SIMPLE

```
 Algoritmo calculadoraSimple
	Imprimir "***Calculadora Simple***"
	Imprimir "ingrese primer numero"
	leer n1
	Imprimir "ingrese segundo numero"
	leer n2
	Imprimir "ingrese una operacion: +.-,*,/"
	leer operacion
	Si operacion == "+" | operacion == "-" | operacion == "*" | operacion == "/" Entonces
		Imprimir "Procesando: " + ConvertirATexto(n1) + " " + operacion + " " + ConvertirATexto(n2) 
			si operacion == "+" Entonces
			Imprimir "resultado: " + ConvertirATexto(n1 + n2)
		sino 
			si operacion == "-" Entonces
				Imprimir "resultado: " + convertirATexto(n1-n2)
			sino 
				si operacion == "*" Entonces
					Imprimir "resultado: " + convertirATexto(n1 * n2)
					SiNo
						Imprimir  "resultado: " + convertirATexto(n1 / n2)
					FinSi
			FinSi
		FinSi
		
	Sino 
		Imprimir " Operación no válida" 
	finsi
	
	
FinAlgoritmo
```

# Tarea 2
# NÚMERO ESPECIAL.

```
Algoritmo NumeroEspecial
	Leer num
	si num == 100 Entonces
		Escribir "Este es un numero especial. "
	SiNo
		si num < 1000 & num % 10 == 0 Entonces
			Escribir "Este es un numero casi especial. "
		sino 
			Escribir "Este es un numero regular. "
		FinSi
	FinSi
	
FinAlgoritmo
```

# Tarea 3
# CALCULADORA SIMPLE CON SWICH.

```
Algoritmo calculadoraSimple  
	Escribir "¿que operacion quiere realizar? (suma/resta/multiplicacion/division)"
	Leer operacion
	
	Escribir "Ingrese primer numero"
	leer n1
	
	Escribir "Ingrese segundo numero"
	leer n2
	
	segun operacion Hacer
		
		Caso, "suma" :
			Escribir "Sumando: ", n1, "+" n2 "="
			Escribir "operando: ", n1, "+" , n2
		
		caso, "resta" :
			Escribir  "Restando: ", n1, "-" n2 "="
			Escribir n1 - n2
			
        caso "multiplicacion":
			Escribir "Multiplicando: ", n1 "*" n2 "="
			Escribir n1 * n2  
			
		caso "division" :
			Escribir "Dividiendo: ", n1 "/" n2 "=" 
			Escribir n1 / n2	
			
	FinSegun
FinAlgoritmo
```

# Tarea 4
# PROGRAMA MULTIOPCION.
```
Algoritmo MultiOpcion
	Escribir "PROGRAMA MULTIOPCION"
	Escribir "Elija cualquiera de las 3 opciones: "
	Escribir "-> Opción 1- Suma de dos números."
	Escribir "-> Opción 2- Longitud de un texto."
	Escribir "-> Opción 3- Día de la semana."
	Escribir "INGRESE UNA OPCION: "
	leer a
	
	Segun a Hacer
	
		1: Escribir "Ingrese primer número."
			Leer b
			Escribir "Ingrese segundo número."
			Leer c
			suma<-b+c
			Escribir "Sumando los números = ", suma
			
		2: Escribir "Ingrese un texto"
			leer d 
			largo<-longitud (d)
			Escribir "La Longitud del texto es: ", largo
			
		3:
			
			Definir día Como Entero
			Escribir "Día de la semana, ingrese un número del 1 al 7"
			Leer día 
	
	Si día ==1 Entonces
		Escribir "Lunes"
		Sino
	FinSi
	
	Si día ==2 Entonces
		Escribir "Martes"
		Sino
					FinSi
		
			Si día ==3 Entonces
				Escribir "Miércoles"
				Sino
			FinSi
			
			Si día ==4 Entonces
				Escribir "Jueves"
				Sino
			FinSi
			
			Si día ==5 Entonces
				Escribir "Viernes"
				Sino
			Finsi
			
			Si día ==6 Entonces
				Escribir "Sábado"
				Sino
			FinSi
			
			Si día ==7 Entonces
				Escribir "Domingo"
			sino
			
			Finsi
		De Otro Modo:
			Escribir "no es opcion"
			
			
	FinSegun
	
			
			
			
	FinAlgoritmo
```

# Tarea 5
# TABLA DE MULTIPLICAR.
```
Algoritmo TablasDeMultiplicar
	Definir a,resultado,b Como Entero
	Escribir "INGRESE CUALQUIER NÚMERO PARA MULTIPLICAR: "
	Leer b
	
	a = 1
	Mientras a <= 10 Hacer
		resultado = b*a
		Escribir b, " * ", a, " = ", resultado
		a = a + 1
	FinMientras
	
FinAlgoritmo
```

# Tarea 6
# CALCULADORA CON DO WHILE
```
Algoritmo calculadoraSimple
	Repetir
	Imprimir "ingrese primer numero"
	leer n1
	Imprimir "ingrese segundo numero"
	leer n2
	Imprimir "ingrese una operacion: +.-,*,/"
	leer operacion
	Si operacion == "+" | operacion == "-" | operacion == "*" | operacion == "/" Entonces
		Imprimir "Procesando: " + ConvertirATexto(n1) + " " + operacion + " " + ConvertirATexto(n2) 
		si operacion == "+" Entonces
			Imprimir "resultado: " + ConvertirATexto(n1 + n2)
		sino 
			si operacion == "-" Entonces
				Imprimir "resultado: " + convertirATexto(n1-n2)
			sino 
				si operacion == "*" Entonces
					Imprimir "resultado: " + convertirATexto(n1 * n2)
				SiNo
					Imprimir  "resultado: " + convertirATexto(n1 / n2)
				FinSi
			FinSi
		FinSi
		
	Sino 
		Imprimir " Operación no válida" 
	finsi
	
	Imprimir "Desea continuar? SI / NO"
	Leer continuar
   Hasta Que continuar == "NO" O continuar == "no"
	
FinAlgoritmo
```

# Tarea 7
# TABLA DE MULTIPLICAR CON BUCLE FOR.
```
Algoritmo TablaMultiplicarBucleFor
	Escribir "Ingrese el número a multiplicar: ";
	Leer tabla;
	Escribir "Ingrese hasta que número: "
	Leer numero;
	Para i <- 1 Hasta numero Hacer
		resultado<-1 * tabla;
		Escribir tabla, " * " , i, " = ", resultado;
	FinPara
	
	
FinAlgoritmo
```

