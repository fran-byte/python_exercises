:page_with_curl: [README](../README.md) :books: [Material didáctico](/documentation/indicedocu.md) :pencil: [Ejercicios](/tests/indicetests.md)


# 1 - Comenzando (print / input)
## _print_
#### Ejercicio 1:


Escribe un programa que muestre por pantalla el texto **Hello Word!**

````python
print("Hello Word!")
````

## _print, input, Tipos de Variables_
#### Ejercicio 2:


Escribe un programa que pida al usuario introducir una cadena, la almacene en una variable y luego muestre por pantalla
el contenido de la variable.

````python
cadena = input("Introduce una cadena de texto: ")
print(cadena)
````

## _print, input, Tipos de Variables, Operadores_
#### Ejercicio 3:


Escribe un programa que pida al usuario introducir 2 números y los multiplique entre si mostrando el resultado por pantalla.

````python
numero1 = float(input("Número 1: "))
numero2 = float(input("Número 2: "))
print(numero1*numero2)
````

## _print, input, Tipos de Variables, Operadores_
#### Ejercicio 4:


Escribe un programa que calcule el volumen de una balón, pidiendo por teclado al usuario los datos necesarios.
Puedes buscar la formula aquí: [volumen ](https://es.wikipedia.org/wiki/Esfera) 

````python
radio = float(input("Radio: "))
PI = 3.14159265359
print("El volumen es : ",(4*PI*radio**3)/3)
````
