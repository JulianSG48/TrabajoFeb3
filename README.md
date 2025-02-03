# TrabajoFeb3

#Trabajo Programación Febrero 3

#-------------------------------------------------------
#Ejercicio 1: Lista con elementos no repetidos
#-------------------------------------------------------

def elementos(lista):

    return len(lista) == len(set(lista))


ejemplolista = [1,2,3,4,5,6]

if elementos(ejemplolista):

    print("En la lista no hay elementos repetidos")

else:

    print("En la lista hay elementos repetidos")

Salida en terminal:

![image](https://github.com/user-attachments/assets/331e3e7a-01dd-40e7-8672-26e94c8cac3d)

#-------------------------------------------------------
#Ejercicio 2: Determinar si un elemento de una lista es una cadena palíndrome 
#-------------------------------------------------------

def palindrome(p):

   return p == p[::-1]

def encontrar_palindrome(strings):

    for p in strings:
    
        if palindrome(p):
        
            return p
            
    return "No existe"

lista = ["hola", "oso", "mundo"]

print(encontrar_palindrome(lista))

Salida en terminal:

![image](https://github.com/user-attachments/assets/ec6b7bed-f741-42f0-aff2-3d2a81944c45)

#-------------------------------------------------------
#Ejercicio 3: Cadena de caracteres con dos o más vocales
#-------------------------------------------------------

def vocales(v):

    vocal = {'a', 'e', 'i', 'o', 'u', 'A', 'E', 'I', 'O', 'U'}
    
    conteo = sum(1 for char in v if char in vocal)
    
    return conteo >= 2

def encontrar_vocales(strings):

    encontrado = False  
    
    for v in strings:
    
        if vocales(v):
        
            print(v)
            
            encontrado = True  
    
    if not encontrado:
    
        print("No existe")

lista = ["gato", "zxcvb", "hola", "xyz"]

encontrar_vocales(lista)

Salida en terminal:

![image](https://github.com/user-attachments/assets/d9b57168-ba8b-4612-acda-fcee980c1204)

#-------------------------------------------------------
#Ejercicio 4: Determinar si una cadena es palíndrome 
#-------------------------------------------------------

def palindrome(pal):

    return pal == pal[::-1]

lista = ["aerea"]

if palindrome(lista):

    print("La cadena es palíndrome")
    
else:

    print("La cadena no es palíndrome")

Salida en terminal:

![image](https://github.com/user-attachments/assets/82e289b1-d9e9-4f26-9990-c0a5a9923c4d)

#-------------------------------------------------------
#Ejercicio 5: Cadena de caracteres con dos o más MAYÚSCULAS
#-------------------------------------------------------

def buscar_mayusculas(lista):

    encontrado = False  
    
    for cadena in lista:
    
        mayusculas = sum(1 for m in cadena if m.isupper())
        
        if mayusculas >= 2:
        
            print(cadena)
            
            encontrado = True
    
    if not encontrado:
    
        print("No existe")

lista = ["hola", "Hola Mundo", "abcDEF", "uNaL", "ejemplo", ""]

buscar_mayusculas(lista)

Salida en terminal:

![image](https://github.com/user-attachments/assets/d8748209-c8b3-4acf-abe9-5f9330f46e19)


#-------------------------------------------------------
#Ejercicio 6: Cadena de caracteres con dos o más numeros
#-------------------------------------------------------

def buscar_numeros(lista):

    encontrado = False  
    
    for cadena in lista:
    
        numeros = sum(1 for n in cadena if n.isdigit())

        if numeros >= 2:
        
            print(cadena)
            
            encontrado = True 
    
    if not encontrado:
    
        print("No existe")

lista = ["abc123", "numeros", "abc12", "prueba345", "abc1", "12345"]

buscar_numeros(lista)

Salida en terminal:

![image](https://github.com/user-attachments/assets/7dc104f2-5fc2-42dd-8df8-2667b8e7e51d)

#-------------------------------------------------------
#Ejericicio 7: Determina la cantidad de palíndromos existentes en una cadena
#-------------------------------------------------------

def es_palindromo(cadena):

    cadena = cadena.lower()
    
    return cadena == cadena[::-1]

def encontrar_palindromos(lista):

    palindromos = []
    
    for s in lista:
    
        if es_palindromo(s):
        
            palindromos.append(s)  
    
    if palindromos:
    
        for pal in palindromos:
        
            print(pal)  
            
        print(f"Total de palíndromos encontrados: {len(palindromos)}")
        
    else:
    
        print("No existe")

lista = ["madam", "hello", "racecar", "abcba", "world"]

encontrar_palindromos(lista)

Salida en terminal:

![image](https://github.com/user-attachments/assets/c02a11a7-67b0-4dab-8906-6300c91425aa)

#-------------------------------------------------------
#Ejericicio 8: Determina si una cadena cuenta con más de 5 caracteres
#-------------------------------------------------------

def palabra_larga(cadena):

    palabras = cadena.split()
    
    for palabra in palabras:
    
        if len(palabra) > 5:
        
            return True
            
    return False

def encontrar_palabras(lista):

    encontrado = False
    
    for s in lista:
    
        if palabra_larga(s):
        
            print(s)  
            
            encontrado = True
    
    if not encontrado:
    
        print("No existen cadenas con palabras de más de 5 caracteres")

lista = ["Hola Mundo", "Universidad Nacional", "Julian Santana", "abc def"]

encontrar_palabras(lista)

Salida en terminal:

![image](https://github.com/user-attachments/assets/4e1fc349-de13-4827-a2a7-956d5a6fa71c)
