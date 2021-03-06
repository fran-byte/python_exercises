:page_with_curl: [README](../README.md) :books: [Material didáctico](/documentation/indicedocu.md) :pencil: [Ejercicios](/tests/indicetests.md)

# 36. PAQUETES

Crear un módulo en Python es tan sencillo como crear un script, sólo tenemos que añadir alguna función a un fichero con la extensión .py, 

por ejemplo **saludos.py** :

````python
def saludar():
    print("Hola, te estoy saludando desde la función saludar() " \
            "del módulo saludos")
````

Luego ya podremos utilizarlo desde otro script,

por ejemplo **script.py**, en el mismo directorio haciendo un import y el nombre del módulo:

````python
import saludos
saludos.saludar()
````

También podemos importar funciones directamente, de esta forma ahorraríamos memoria. Podemos hacerlo utilizando la sintaxis from import:

````python
from saludos import saludar
saludar()
````

Para importar todas las funciones con la sintaxis from import debemos poner un asterisco:

````python
from saludos import *
saludar()
````

Dicho esto, a parte de funciones también podemos reutilizar clases:

````python
class Saludo():
    def __init__(self):
        print("Hola, te estoy saludando desde el __init__ " \
                "de la clase Saludo")
````

Igual que antes, tendremos que llamar primero al módulo para referirnos a la clase:

````python
import saludos

s = saludos.Saludo()
````

O cargar solo una clase con el from import:

````python
from saludos import Saludo

s = Saludo()
````

El problema ocurre cuando queremos utilizar nuestro módulo desde un directorio distinto por ejemplo test/script.py.

