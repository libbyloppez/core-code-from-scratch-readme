# tarea 1
# Calculadora Simple

```Algoritmo calculadoraSimple
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
# Número especial
```Algoritmo NumeroEspecial
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
# Calculadora Simple con swuitch

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

