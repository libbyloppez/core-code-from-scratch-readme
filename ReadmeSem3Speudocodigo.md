### Tarea
# Calculadora Simple

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

