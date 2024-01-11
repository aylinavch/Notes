# POO

Hay distintos **enfoques o paradigmas de programación**, es decir, diversos puntos de vistas teórico-práctico que hace posible encontrar soluciones a problemas complejos partiendo del análisis y apoyándose en la planificación del código.

Uno de los enfoques para resolver un problema de programación es mediante la creación de *****objetos*****, llamado ***Programación Orientada a Objetos (POO)***

> 🐍 Todo en Python es un OBJETO


Un OBJETO tiene dos propiedades:

1. ATRIBUTOS —> Características --> _Variables_
    
2. MÉTODOS —> Comportamientos --> _Funciones_

<span style="color:orange"> **Por ejemplo:** </span>

<span style="color:orange"> Un *perro* puede ser el objeto y tiene las siguiente propiedades:</span>

<span style="color:orange">`nombre, edad, color` —> *atributos*</span>

<span style="color:orange"> `ladrar, caminar` —> *métodos*</span>

## Clases - Instancias - Objetos 

Para crear objetos en Python se utiliza el comando `class`

Las clases son moldes que sirven para crear objetos. Entonces podemos pensar a la clase como un boceto (****prototipo****) que contiene todos los detalles y basándonos en estas descripciones construimos el objeto.

```python
class Nombre_Objeto:
```

Un **objeto**, también llamado instancias, es creado a partir de una clase (molde, boceto); y el proceso de creación de este objeto se llama **instanciación**.

```python
class Nombre_Objeto:
	def __init__(self, atributo1, atributo2):
		self.atributo1 = atributo1
		self.atributo2 = atributo2
```

El constructor `__init__` es aquel método para inicializar algunos atributos (características de un objeto). Se ejecuta instantáneamente después de crear el objeto a partir de una clase.

El parámetro *`self`* sirve para trabajar con un objeto futuro dentro de una clase (que será creado posteriormente en el código), permitiendo agregar y leer atributos y métodos desde la definición misma de la clase

## Constructores

`__new__` Crear una nueva instancia de la clase (**************************no es necesario declararlo**************************)

`__init__` Inicializar atributos; se llama una vez creado el objeto

`__del__` Se llama cuando la clase está a punto de ser destruida

`__bytes__` Representación de bytes-string de un objeto

`__format__` Producir una representación de string "formateada" de un objeto

`__str__` Representación en cadena de texto del objeto (informal, *user*)

`__repr__` Representación en cadena de texto del objeto (formal, *programmer*)

- Diferencia entre `__str__` y `__repr__`
    
    ```python
    >>> import datetime
    >>> today = datetime.datetime.now()
    
    >>> today #__repr__
    datetime.datetime(2023, 2, 18, 18, 40, 2, 160890)
    
    >>> print(today) #__str__
    2023-02-18 18:40:02.160890
    
    # Para ver qué el constructor se puede correr today.__repr__() o today.__str__()
    # Para más info ver https://realpython.com/python-repr-vs-str/
    ```
    

`__add__` Qué hace el comando “`+`" en este objeto

`__lt__` Qué hace el comando “`<`"

`__le__` Qué hace el comando “`<=`"

`__eq__` Qué hace el comando “`==`"

`__ne__` Qué hace el comando “`!=`"

`__gt__` Qué hace el comando “`>`"

`__ge__` Qué hace el comando “`>=`"

`__bool__` Llamado para implementar pruebas de valor de verdad y la operación `bool()`

`__len__` Para implementar la función `len()`

`__get__` Llamado para obtener el atributo de la clase propietaria (acceso al atributo de clase) o de una instancia de esa clase (acceso al atributo de instancia).

`__set__`

# (this is not up2date, in [this link](https://gorgeous-sky-34f.notion.site/POO-46d011c5761344d781c7419f8869bef2?pvs=4) you could see updates and more info)