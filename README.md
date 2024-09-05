# parcial1
parcial #1 Daniel Reyes
Proyecto de Parcial 1

Este proyecto contiene varios programas desarrollados para el primer parcial de la asignatura de Lenguajes de Programación. Cada punto del parcial aborda un problema específico y su solución correspondiente.
Puntos del Parcial
# 1. Autómata Finito Determinista (AFD) en Python

Implementa un programa en Python que acepta las siguientes expresiones regulares:

    +
    ++
    [0-9]+
    ([0-9]+)”.”([0-9])+

Para cada expresión regular, el programa debe devolver el token correspondiente. El programa recibe una expresión regular como parámetro y devuelve su token.

Ejemplo de uso:

    python3 AFD.py 

los elementos a probar son:235, 15.65, +, ++
Salida: 
    
    Expresión: 235 -> Token: ENTERO
    Expresión: 15.65 -> Token: REAL
    Expresión: + -> Token: SUMA
    Expresión: ++ -> Token: INCR


# 2. Gramática Regular para Función Lambda en LEX

Escribe una gramática regular en LEX para comprender el funcionamiento de la función lambda en Python. El programa debe recibir un archivo de texto como parámetro y devolver si la expresión es aceptada o no.

Ejemplo de archivo de entrada (prueba.txt):

    square = lambda x: x ** 2
    print(square(3))

Ejemplo de uso:

    ./verificar_lambda prueba.txt

Salida: ACEPTA o NO ACEPTA

# 3. Programa en C para Contar Coincidencias de una Palabra Clave

Escribe un programa en C que reciba dos parámetros: un archivo de texto y una palabra clave. El programa debe retornar la cantidad de coincidencias de la palabra clave en el texto.
la prueba es:

    hola mundo
    hola buenas tardes, probemos si funciona
    hola a todos
    este es un ejemplo de hola
    por eso es bueno decir hola
    Ejemplo de uso:

se ejecuta:

    ./contador prueba.txt hola
    
 Salida: 
     
     hola se repite 5 veces en el texto.

# 4. Programa en AWK para Identificar Números Primos

Realiza un programa en AWK que analice un archivo de texto con 1000 números enteros aleatorios del 1 al 1000 y determine cuáles son números primos.

los numeros primos se definen de forma aleatoria por un programa en python que genera un archivo llamado numeros.txt

Ejemplo de uso:

    awk -f primos.awk numeros.txt

# 5. Programa en ANTLR para Calcular Funciones Trigonométricas

Escribe un programa en ANTLR que pueda calcular las siguientes funciones trigonométricas:

    Sin(x)
    Cos(x)
    Tan(x)

El programa debe leer las expresiones desde un archivo de texto e imprimir el resultado en radianes.

Ejemplo de archivo de entrada (expr.in):

    Sin(90)
    Cos(0)
    Cos(180)
    Sin(45)

Se ejecuta:

    java TrigCalc expr.in
Salida:

    1.0
    1.0
    -1.0
    0.7071067811865475

