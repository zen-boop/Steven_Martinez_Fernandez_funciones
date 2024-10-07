#Practicando funciones
#En Python una funcion es definida usando la palabra def como palabra clave 

def my_function():
    print("Hello from a function")


#Para llamar a una funcion, use la funcion nombrada y seguida de parentesis:
def my_function():
    print("Hello from a function")





#El siguiente ejemplo tiene una función con un argumento (fname). Cuando se llama a la función, pasamos un nombre, que se usa dentro de la función para imprimir el nombre completo:

def my_function(fname):
    print(fname + " Refsnes")

my_function("Emil")
my_function("Tobias")
my_function("Linus")



#De forma predeterminada, se debe llamar a una función con la cantidad correcta de argumentos. Lo que significa que si su función espera 2 argumentos, debe llamar a la función con 2 argumentos, ni más ni menos.

#Ejemplo

#Esta función espera 2 argumentos y obtiene 2 argumentos:

def my_function(fname, lname):

    print(fname + " " + lname)

my_function("Emil", "Refsnes")


#Esta función espera 2 argumentos, pero solo obtiene 1:
def my_function(fname, lname):
    print(fname + " " + lname)

my_function("Emil","refuses")




#Si no sabe cuántos argumentos se pasarán a su función, agregue un * antes del nombre del parámetro en la definición de la función.

#De esta manera, la función recibirá una tupla de argumentos y podrá acceder a los elementos en consecuencia:

#Si se desconoce el número de argumentos, agregue un * antes del nombre del parámetro:

def my_function(*kids):
    print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus")



#También puede enviar argumentos con la sintaxis clave = valor.

#De esta forma no importa el orden de los argumentos.
def my_function(child3, child2, child1):
    print("The youngest child is " + child3)

my_function(child1 = "Emil", child2 = "Tobias", child3 = "Linus")


#Argumentos arbitrarios de palabras clave, **kwargs
#Si no sabe cuántos argumentos de palabras clave se pasarán a su función, agregue dos asteriscos: ** antes del nombre del parámetro en la definición de la función.

#De esta manera, la función recibirá un diccionario de argumentos y podrá acceder a los elementos en consecuencia:
#Si se desconoce el número de argumentos de palabras clave, agregue un doble ** antes del nombre del parámetro:

#Ícono de validado por la comunidad





def my_function(**kid):
    print("His last name is " + kid["lname"])

my_function(fname = "Tobias", lname = "Refsnes")



#Valor de parámetro predeterminado
#El siguiente ejemplo muestra cómo utilizar un valor de parámetro predeterminado.

#Si llamamos a la función sin argumento, usa el valor predeterminado:
def my_function(country = "Norway"):
    print("I am from " + country)

my_function("Sweden")
my_function("India")
my_function()
my_function("Brazil")

#Pasar una lista como argumento
#Puede enviar cualquier tipo de argumento de datos a una función (cadena, número, lista, diccionario, etc.) y será tratado como el mismo tipo de datos dentro de la función.

#P.ej. Si envía una Lista como argumento, seguirá siendo una Lista cuando llegue a la función:

def my_function(food):
    for x in food:
        print(x)

fruits = ["apple", "banana", "cherry"]

my_function(fruits)
print("");print("pruebas");print("")
def p(c):
  if(c > 0):
    r = c + p(c - 1)
    print(r)
  else:
    r = 0
  return r


p(10)
![image](https://github.com/user-attachments/assets/545a60dd-37ae-48a5-861a-95da593b6fb7)
