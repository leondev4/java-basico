---

markmap:
  initialExpandLevel: 2
---
# Preguntas teóricas – Módulo 1: Fundamentos de Java

## 1. Completar

### Pregunta 1.1
- Todo programa en Java debe tener un método ______ que es el punto de entrada de la aplicación.

### Pregunta 1.2
- La palabra clave ______ se usa para crear una nueva clase en Java.

### Pregunta 1.3
- Para mostrar texto en consola sin salto de línea se usa `System.out.______()`.

### Pregunta 1.4
- El tipo de dato ______ se utiliza para almacenar números decimales en Java.

### Pregunta 1.5
- La sintaxis para declarar una variable de tipo entero llamada `contador` es `______ contador;`.

### Pregunta 1.6
- El tipo primitivo `______` solo puede almacenar `true` o `false`.

### Pregunta 1.7
- Para declarar una constante en Java se usa la palabra clave `final` antes del tipo. Ejemplo: `final double PI = ______;`.

### Pregunta 1.8
- El nombre del archivo fuente en Java debe coincidir con el nombre de la ______ pública.

### Pregunta 1.9
- Las llaves `______` se utilizan para delimitar bloques de código en Java.

### Pregunta 1.10
- El tipo `char` almacena un solo carácter y se escribe entre comillas ______ (simples/dobles).

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Cuál de los siguientes NO es un tipo primitivo en Java?
a) int
b) String
c) double
d) boolean

### Pregunta 2.2
- ¿Qué método se utiliza para mostrar texto con salto de línea?
a) System.out.print()
b) System.out.println()
c) System.out.printf()
d) System.out.write()

### Pregunta 2.3
- ¿Cuál es la salida del siguiente código?
    ```java
    int a = 5;
    int b = 10;
    System.out.println("a + b = " + a + b);
    ```
    a) a + b = 15
    b) a + b = 510
    c) 15
    d) Error

### Pregunta 2.4
- ¿Cuál es la forma correcta de declarar una variable?
a) int edad = 25;
b) int = 25 edad;
c) edad int = 25;
d) int 25 = edad;

### Pregunta 2.5
- ¿Qué palabra clave se usa para crear un objeto?
a) class
b) new
c) create
d) object

### Pregunta 2.6
- ¿Cuál es el valor por defecto de una variable `int` no inicializada en un método?
a) 0
b) null
c) Error de compilación
d) undefined

### Pregunta 2.7
- ¿Qué significa JVM?
a) Java Variable Machine
b) Java Virtual Machine
c) Java Visual Method
d) Java Version Manager

### Pregunta 2.8
- ¿Cuál de los siguientes es un nombre de variable válido?
a) 2variable
b) mi-variable
c) _miVariable
d) mi variable

### Pregunta 2.9
- ¿Qué extensión tienen los archivos fuente de Java?
a) .class
b) .exe
c) .java
d) .jar

### Pregunta 2.10
- ¿Qué comando se usa para compilar un programa Java?
a) java
b) javac
c) compile
d) run

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada tipo primitivo con su tamaño en bits:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. int | A. 1 bit |
    | 2. double | B. 16 bits |
    | 3. char | C. 32 bits |
    | 4. boolean | D. 64 bits |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada palabra clave con su descripción:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. public | A. Acceso desde cualquier lugar |
    | 2. static | B. Valor que no puede cambiar |
    | 3. final | C. Método pertenece a la clase |
    | 4. void | D. Método no devuelve valor |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.3
- Relaciona cada tipo de dato con su ejemplo:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. int | A. 'A' |
    | 2. double | B. true |
    | 3. char | C. 3.1416 |
    | 4. boolean | D. 100 |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) En Java, el nombre de la clase debe ser igual al nombre del archivo .java

### Pregunta 4.2
- (V) (F) El método `main` debe ser `public static void main(String[] args)`

### Pregunta 4.3
- (V) (F) Java es un lenguaje de programación compilado e interpretado

### Pregunta 4.4
- (V) (F) El tipo `String` es un tipo primitivo en Java

### Pregunta 4.5
- (V) (F) Las variables en Java deben declararse antes de usarse

### Pregunta 4.6
- (V) (F) `System.out.println()` automáticamente agrega un salto de línea al final

### Pregunta 4.7
- (V) (F) Los comentarios en Java de una línea se hacen con `/* comentario */`

### Pregunta 4.8
- (V) (F) La palabra clave `final` hace que una variable sea constante

### Pregunta 4.9
- (V) (F) Java es un lenguaje débilmente tipado

### Pregunta 4.10
- (V) (F) Las llaves `{}` en Java son opcionales para bloques de una sola línea

---

## 📋 Respuestas

### Respuestas de completar:
-    1.1: `main`
    1.2: `class`
    1.3: `print`
    1.4: `double`
    1.5: `int`
    1.6: `boolean`
    1.7: `3.1416` (o cualquier número)
    1.8: `clase`
    1.9: `{}`
    1.10: `simples`

### Respuestas de opción múltiple:
-    2.1: b
    2.2: b
    2.3: b
    2.4: a
    2.5: b
    2.6: c (las variables locales deben inicializarse antes de usarse, da error de compilación)
    2.7: b
    2.8: c
    2.9: c
    2.10: b

### Respuestas de relacionar:
-    3.1: 1-C, 2-D, 3-B, 4-A
    3.2: 1-A, 2-C, 3-B, 4-D
    3.3: 1-D, 2-C, 3-A, 4-B

### Respuestas de verdadero/falso:
-    4.1: V
    4.2: V
    4.3: V
    4.4: F (String es una clase)
    4.5: V
    4.6: V
    4.7: F (Los comentarios de una línea son `//`)
    4.8: V
    4.9: F (Java es fuertemente tipado)
    4.10: F (Son necesarias para bloques de más de una línea, pero se recomiendan siempre)

# Preguntas teóricas – Módulo 2: Entrada de datos y operadores

## 1. Completar

### Pregunta 1.1
- Para usar la clase Scanner se debe importar con `import java.______.Scanner;`.

### Pregunta 1.2
- Para crear un objeto Scanner que lea del teclado se usa: `Scanner sc = new Scanner(System.______);`.

### Pregunta 1.3
- El método `sc.nextInt()` se usa para leer un número ______.

### Pregunta 1.4
- El operador `%` se llama operador ______ y devuelve el resto de una división.

### Pregunta 1.5
- El operador `______` se usa para evaluar "mayor o igual que".

### Pregunta 1.6
- El operador lógico `&&` significa ______ (Y lógico).

### Pregunta 1.7
- El operador `!` es el operador de ______ lógica.

### Pregunta 1.8
- Para leer una línea completa de texto (incluyendo espacios) se usa `sc.______()`.

### Pregunta 1.9
- El resultado de una expresión relacional es siempre un valor ______ (true/false).

### Pregunta 1.10
- Para convertir un `double` a `int` se usa el ______ explícito: `(int) variable`.

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Qué método de Scanner se usa para leer un número decimal?
a) nextInt()
b) nextDouble()
c) nextLine()
d) nextDecimal()

### Pregunta 2.2
- ¿Cuál es el resultado de `15 / 4` si ambas variables son `int`?
a) 3.75
b) 3
c) 4
d) 3.0

### Pregunta 2.3
- ¿Qué operador lógico devuelve `true` solo si ambas condiciones son `true`?
a) ||
b) !
c) &&
d) &|

### Pregunta 2.4
- ¿Cuál es el resultado de `(5 > 3) || (4 > 10)`?
a) true
b) false
c) Error
d) null

### Pregunta 2.5
- ¿Qué problema puede ocurrir al usar `nextLine()` después de `nextInt()`?
a) Error de compilación
b) El programa se congela
c) `nextLine()` consume el salto de línea pendiente y lee un String vacío
d) No hay problema

### Pregunta 2.6
- ¿Cuál es el resultado de `17 % 5`?
a) 3
b) 2
c) 3.4
d) 5

### Pregunta 2.7
- ¿Cuál es la precedencia correcta de estos operadores (de mayor a menor)?
a) () > * > + > == > &&
b) * > () > + > && > ==
c) () > * > + > && > ==
d) && > == > + > * > ()

### Pregunta 2.8
- ¿Qué valor tiene `resultado` después de `boolean resultado = !(10 > 5);`?
a) true
b) false
c) 10
d) 5

### Pregunta 2.9
- ¿Cuál es el resultado de `(2 + 3 * 4)`?
a) 20
b) 14
c) 24
d) 9

### Pregunta 2.10
- ¿Qué hace el operador `+=` en `a += 5;`?
a) a = a + 5
b) a + 5
c) a = 5
d) a > 5

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada operador con su descripción:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. == | A. Asignación |
    | 2. = | B. Diferente de |
    | 3. != | C. Igualdad |
    | 4. === | D. No existe en Java |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada método de Scanner con su función:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. next() | A. Lee una línea completa |
    | 2. nextLine() | B. Lee un número entero |
    | 3. nextInt() | C. Lee una palabra |
    | 4. nextDouble() | D. Lee un número decimal |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.3
- Relaciona cada expresión con su resultado (a=10, b=3):

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. a > b | A. 1 |
    | 2. a % b | B. 13 |
    | 3. a + b | C. false |
    | 4. a == b | D. true |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) El operador `=` se usa para comparar igualdad en Java.

### Pregunta 4.2
- (V) (F) `Scanner` pertenece al paquete `java.util`.

### Pregunta 4.3
- (V) (F) El operador `||` devuelve `true` solo si ambas condiciones son `true`.

### Pregunta 4.4
- (V) (F) `5 / 2` en Java con enteros da como resultado `2.5`.

### Pregunta 4.5
- (V) (F) El operador `%` solo funciona con números enteros.

### Pregunta 4.6
- (V) (F) Los operadores aritméticos tienen mayor precedencia que los relacionales.

### Pregunta 4.7
- (V) (F) `nextLine()` lee solo hasta el primer espacio en blanco.

### Pregunta 4.8
- (V) (F) Es recomendable cerrar el objeto `Scanner` con `sc.close()`.

### Pregunta 4.9
- (V) (F) `!(a > b)` es equivalente a `a <= b`.

### Pregunta 4.10
- (V) (F) El operador `++` incrementa el valor de una variable en 2.

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `util`
1.2: `in`
1.3: `entero`
1.4: `módulo` (o `resto`)
1.5: `>=`
1.6: `Y`
1.7: `negación` (o `NOT`)
1.8: `nextLine`
1.9: `booleano`
1.10: `casting`

### Respuestas de opción múltiple:
- 2.1: b
2.2: b
2.3: c
2.4: a
2.5: c
2.6: b (17 % 5 = 2)
2.7: c
2.8: b
2.9: b (2 + 12 = 14)
2.10: a

### Respuestas de relacionar:
-   3.1: 1-C, 2-A, 3-B, 4-D
    3.2: 1-C, 2-A, 3-B, 4-D
    3.3: 1-D, 2-A, 3-B, 4-C

### Respuestas de verdadero/falso:
-   4.1: F (es asignación, la igualdad es `==`)
    4.2: V
    4.3: F (es `&&` el que requiere ambas verdaderas)
    4.4: F (da 2, división entera)
    4.5: F (también funciona con números decimales)
    4.6: V
    4.7: F (lee toda la línea)
    4.8: V
    4.9: V
    4.10: F (incrementa en 1)

# Preguntas teóricas – Módulo 3: Estructuras condicionales

## 1. Completar

### Pregunta 1.1
- La estructura `if (condición) { }` ejecuta el bloque solo si la condición es ______.

### Pregunta 1.2
- La palabra clave ______ se usa en `switch` para evitar la caída a los siguientes casos.

### Pregunta 1.3
- El bloque `______` en un `switch` se ejecuta cuando ningún `case` coincide.

### Pregunta 1.4
- El operador ternario tiene la sintaxis: `variable = (condición) ? ______ : ______;`.

### Pregunta 1.5
- Para evaluar múltiples condiciones excluyentes después de un `if` se usa `else ______`.

### Pregunta 1.6
- En un `switch`, la variable puede ser de tipo `int`, `char`, `String` o ______.

### Pregunta 1.7
- El siguiente código es un ejemplo de estructura ______: `if (x > 0) { } else { }`.

### Pregunta 1.8
- La estructura `if-else if-else` se evalúa en ______ (orden/desorden).

### Pregunta 1.9
- Para comparar igualdad en Java se usa el operador ______ (dos signos igual).

### Pregunta 1.10
- Si en un `switch` se omite el `break`, ocurre una ______ hacia el siguiente `case`.

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Qué imprime el siguiente código?
    ```java
    int x = 5;
    if (x = 10) {
        System.out.println("Hola");
    }
    ```
    a) Hola
    b) Nada
    c) Error de compilación
    d) 10

### Pregunta 2.2
-  ¿Qué valor toma `resultado`?
    ```java
    int resultado = (8 > 3) ? 100 : 200;
    ```
    a) 8
    b) 3
    c) 100
    d) 200

### Pregunta 2.3
- ¿Qué imprime este código si `dia = 2`?
    ```java
    switch(dia) {
        case 1: System.out.print("A");
        case 2: System.out.print("B");
        case 3: System.out.print("C");
        default: System.out.print("D");
    }
    ```
    a) B
    b) BCD
    c) BC
    d) ABCD

### Pregunta 2.4
- ¿Cuál es la salida si `nota = 75`?
    ```java
    if (nota >= 90) System.out.println("A");
    else if (nota >= 80) System.out.println("B");
    else if (nota >= 70) System.out.println("C");
    else System.out.println("D");
    ```
    a) A
    b) B
    c) C
    d) D

### Pregunta 2.5
- ¿Qué tipo de datos NO se puede usar en un `switch`?
a) `int`
b) `char`
c) `String`
d) `double`

### Pregunta 2.6
- ¿Cuál es la forma correcta de escribir un `if` de una línea?
a) `if (x > 0) System.out.println("Positivo");`
b) `if x > 0 then System.out.println("Positivo");`
c) `if (x > 0) then println("Positivo");`
d) `if x > 0 { println("Positivo"); }`

### Pregunta 2.7
- ¿Qué hace el operador ternario en `int m = (a > b) ? a : b;`?
a) Asigna a `m` el valor de `a` si `a > b`, sino asigna `b`
b) Compara `a` y `b`
c) Suma `a` y `b`
d) Resta `b` de `a`

### Pregunta 2.8
- ¿Cuál es la salida?
    ```java
    int a = 10, b = 20;
    if (a > b) 
        System.out.println("A");
        System.out.println("B");
    ```
    a) A
    b) B
    c) A y B en líneas separadas
    d) Error

### Pregunta 2.9
- ¿Qué condición es equivalente a `!(a > b)`?
a) a < b
b) a <= b
c) a >= b
d) a == b

### Pregunta 2.10
- ¿Cuál es la salida si `edad = 17`?
    ```java
    String mensaje = (edad >= 18) ? "Mayor" : "Menor";
    System.out.println(mensaje);
    ```
    a) Mayor
    b) Menor
    c) true
    d) false

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada estructura con su caso de uso:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. if-else | A. Asignación condicional simple |
    | 2. switch | B. Dos opciones excluyentes |
    | 3. Operador ternario | C. Múltiples opciones con valores fijos |
    | 4. else if | D. Múltiples opciones con rangos |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada expresión con su valor (a=10, b=5):

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. a > b && b > 0 | A. true |
    | 2. a < b || b == 5 | B. false |
    | 3. !(a == b) | C. true |
    | 4. a == b && b > 0 | D. false |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.3
- Relaciona cada tipo de `case` con su sintaxis correcta:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. case 1: | A. case "rojo": |
    | 2. case 'A': | B. case 1: |
    | 3. case "rojo": | C. case 'A': |

    **Respuesta:** `1-___, 2-___, 3-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) El `else` es obligatorio después de un `if`.

### Pregunta 4.2
- (V) (F) El `switch` puede trabajar con rangos de valores.

### Pregunta 4.3
- (V) (F) Si se omite `break` en un `switch`, el programa continúa ejecutando los siguientes `case`.

### Pregunta 4.4
- (V) (F) El operador ternario puede reemplazar cualquier estructura `if-else`.

### Pregunta 4.5
- (V) (F) En un `if-else if`, se ejecuta más de un bloque si varias condiciones son verdaderas.

### Pregunta 4.6
- (V) (F) `switch` es más legible que `if-else` cuando hay muchas opciones con valores fijos.

### Pregunta 4.7
- (V) (F) El bloque `default` en un `switch` es obligatorio.

### Pregunta 4.8
- (V) (F) `else if` es una palabra clave separada en Java.

### Pregunta 4.9
- (V) (F) Las llaves `{}` son obligatorias en el `if` cuando el bloque tiene más de una línea.

### Pregunta 4.10
- (V) (F) El operador ternario puede anidarse: `(a>b)?(a>c?a:c):(b>c?b:c)`

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `true` (o `verdadera`)
1.2: `break`
1.3: `default`
1.4: `valorTrue`, `valorFalse`
1.5: `if`
1.6: `enum`
1.7: `if-else` (o `binaria`)
1.8: `orden`
1.9: `==`
1.10: `caída` (o `fall through`)

### Respuestas de opción múltiple:
- 2.1: c
2.2: c
2.3: b
2.4: c
2.5: d
2.6: a
2.7: a
2.8: b (solo la primera línea está dentro del if)
2.9: b
2.10: b

### Respuestas de relacionar:
- 3.1: 1-B, 2-C, 3-A, 4-D
3.2: 1-A, 2-C, 3-A, 4-D
3.3: 1-B, 2-C, 3-A

### Respuestas de verdadero/falso:
- 4.1: F (es opcional)
4.2: F (solo valores concretos)
4.3: V
4.4: F (solo para asignaciones simples)
4.5: F (solo el primero)
4.6: V
4.7: F (es opcional)
4.8: F (es `else` seguido de `if`)
4.9: V
4.10: V

# Preguntas teóricas – Módulo 4: Bucles

## 1. Completar

### Pregunta 1.1
- El bucle `for` tiene tres partes: ______, ______ e ______.

### Pregunta 1.2
- El bucle `while` evalúa la condición al ______ (inicio/final) del bloque.

### Pregunta 1.3
- El bucle `do-while` garantiza que el bloque se ejecute al ______ una vez.

### Pregunta 1.4
- La sentencia ______ termina inmediatamente la ejecución de un bucle.

### Pregunta 1.5
- La sentencia ______ salta a la siguiente iteración del bucle sin ejecutar el resto del bloque.

### Pregunta 1.6
- Un bucle que nunca termina se llama bucle ______.

### Pregunta 1.7
- En un bucle `for (int i = 0; i < 10; i++)`, la variable `i` se incrementa en ______ cada iteración.

### Pregunta 1.8
- El bucle `for-each` se usa para recorrer ______ y colecciones.

### Pregunta 1.9
- Para salir de un bucle `while` se puede usar la condición que se vuelva ______ o usar `break`.

### Pregunta 1.10
- En un bucle anidado, el bucle ______ se ejecuta completamente por cada iteración del bucle externo.

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Cuántas veces se ejecuta el siguiente bucle?
    ```java
    for (int i = 0; i < 5; i++) {
        System.out.println(i);
    }
    ```
    a) 4
    b) 5
    c) 6
    d) 0

### Pregunta 2.2
- ¿Qué imprime este código?
    ```java
    int i = 0;
    while (i < 3) {
        System.out.print(i);
        i++;
    }
    ```
    a) 012
    b) 123
    c) 0123
    d) 0

### Pregunta 2.3
- ¿Qué imprime este código?
    ```java
    int i = 0;
    do {
        System.out.print(i);
        i++;
    } while (i < 0);
    ```
    a) Nada
    b) 0
    c) 0 (bucle infinito)
    d) Error

### Pregunta 2.4
- ¿Qué hace `break` dentro de un bucle?
a) Termina el programa
b) Sale del bucle actual
c) Salta a la siguiente iteración
d) Reinicia el bucle

### Pregunta 2.5
- ¿Cuál es la salida?
    ```java
    for (int i = 0; i < 5; i++) {
        if (i == 2) continue;
        System.out.print(i);
    }
    ```
    a) 01234
    b) 0134
    c) 0123
    d) 034

### Pregunta 2.6
- ¿Qué condición hace que este bucle sea infinito?
    ```java
    int i = 0;
    while (i < 10) {
        System.out.println(i);
    }
    ```
    a) Falta incrementar `i`
    b) La condición es `i < 10`
    c) `i` se inicializa en 0
    d) No imprime nada

### Pregunta 2.7
- ¿Cuál es el resultado de `for (int i = 5; i > 0; i--)`?
a) Itera de 5 a 1
b) Itera de 5 a 0
c) Itera de 0 a 5
d) Bucle infinito

### Pregunta 2.8
- ¿Qué imprime este código?
    ```java
    for (int i = 1; i <= 3; i++) {
        for (int j = 1; j <= 2; j++) {
            System.out.print(i + "" + j + " ");
        }
    }
    ```
    a) 11 12 21 22 31 32
    b) 11 12 13 21 22 23
    c) 11 21 31 12 22 32
    d) 11 12 21 22 31 33

### Pregunta 2.9
- ¿Cuál es la sintaxis correcta del `for-each`?
a) `for (int i : array) { }`
b) `for (int i = 0 : array) { }`
c) `foreach (int i in array) { }`
d) `for (int i; array) { }`

### Pregunta 2.10
- ¿Qué imprime este código?
    ```java
    int i = 0;
    while (i < 3) {
        System.out.print(i);
        i++;
        if (i == 2) break;
    }
    ```
    a) 01
    b) 012
    c) 0
    d) 01 (bucle termina en i=2)

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada bucle con su caso de uso:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. for | A. Se ejecuta al menos una vez |
    | 2. while | B. Número fijo de iteraciones |
    | 3. do-while | C. Condición al inicio |
    | 4. for-each | D. Recorrer arrays sin índice |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada sentencia con su efecto:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. break | A. Salta a la siguiente iteración |
    | 2. continue | B. Sale del bucle |
    | 3. return | C. Sale del método |

    **Respuesta:** `1-___, 2-___, 3-___`

### Pregunta 3.3
- Relaciona cada código con su salida:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. `for (int i=0; i<3; i++) { System.out.print(i); }` | A. 012 |
    | 2. `for (int i=3; i>0; i--) { System.out.print(i); }` | B. 0 |
    | 3. `int i=0; while (i<1) { System.out.print(i); i++; }` | C. 321 |

    **Respuesta:** `1-___, 2-___, 3-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) El bucle `for` siempre ejecuta el bloque al menos una vez.

### Pregunta 4.2
- (V) (F) `break` puede usarse dentro de `if` para salir del bucle que lo contiene.

### Pregunta 4.3
- (V) (F) `continue` hace que el bucle termine inmediatamente.

### Pregunta 4.4
- (V) (F) El bucle `do-while` es adecuado cuando se necesita ejecutar el bloque al menos una vez.

### Pregunta 4.5
- (V) (F) En un `for`, la inicialización solo se ejecuta una vez.

### Pregunta 4.6
- (V) (F) Se puede usar `break` para salir de un `if`.

### Pregunta 4.7
- - (V) (F) El `for-each` permite modificar los elementos del array.

### Pregunta 4.8
- (V) (F) Un bucle infinito ocurre cuando la condición nunca se vuelve `false`.

### Pregunta 4.9
- (V) (F) `for (int i = 10; i >= 0; i--)` itera 11 veces.

### Pregunta 4.10
- (V) (F) `while(true)` es un bucle infinito.

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `inicialización`, `condición`, `incremento`
1.2: `inicio`
1.3: `menos`
1.4: `break`
1.5: `continue`
1.6: `infinito`
1.7: `1` (uno)
1.8: `arrays`
1.9: `false`
1.10: `interno`

### Respuestas de opción múltiple:
- 2.1: b (0,1,2,3,4 = 5 veces)
2.2: a (0,1,2)
2.3: b (0)
2.4: b
2.5: b (0,1,3,4)
2.6: a
2.7: a
2.8: a
2.9: a
2.10: a (0,1)

### Respuestas de relacionar:
- 3.1: 1-B, 2-C, 3-A, 4-D
3.2: 1-B, 2-A, 3-C
3.3: 1-A, 2-C, 3-B

### Respuestas de verdadero/falso:
- 4.1: F (puede no ejecutarse)
4.2: V
4.3: F (solo salta la iteración actual)
4.4: V
4.5: V
4.6: F (solo funciona en bucles o switch)
4.7: F (solo lectura)
4.8: V
4.9: V (10 a 0 son 11 valores)
4.10: V

# Preguntas teóricas – Módulo 5: Arrays y cadenas

## 1. Completar

### Pregunta 1.1
- Para obtener la longitud de un array se usa la propiedad `array.______`.

### Pregunta 1.2
- Para obtener la longitud de un `String` se usa el método `texto.______()`.

### Pregunta 1.3
- El primer índice de un array es ______.

### Pregunta 1.4
- Si un array tiene tamaño 5, el último índice válido es ______.

### Pregunta 1.5
- Para declarar un array de enteros se usa: `int[] numeros = new int[______];`.

### Pregunta 1.6
- El método `charAt(posición)` devuelve el ______ en esa posición.

### Pregunta 1.7
- El método `substring(inicio, fin)` devuelve los caracteres desde `inicio` hasta `fin-______`.

### Pregunta 1.8
- Para comparar dos Strings por contenido se usa el método `______()`.

### Pregunta 1.9
- El método `toUpperCase()` convierte un String a ______.

### Pregunta 1.10
- El método `trim()` elimina los espacios en ______ y al final del String.

---

## 2. Opción múltiple

### Pregunta 2.1
-  ¿Cómo se declara un array de 10 enteros?
a) `int[10] numeros;`
b) `int[] numeros = new int[10];`
c) `int numeros = new int[10];`
d) `array int numeros[10];`

### Pregunta 2.2
- ¿Cuál es la salida?
    ```java
    int[] nums = {1, 2, 3};
    System.out.println(nums.length);
    ```
    a) 2
    b) 3
    c) 4
    d) Error

### Pregunta 2.3
- ¿Qué método se usa para obtener un carácter en una posición específica de un String?
a) `getChar()`
b) `charAt()`
c) `getCharacter()`
d) `characterAt()`

### Pregunta 2.4
- ¿Cuál es la salida?
    ```java
    String texto = "Hola";
    System.out.println(texto.length());
    ```
    a) 3
    b) 4
    c) 5
    d) Error

### Pregunta 2.5
- ¿Cómo se compara correctamente dos Strings?
a) `if (s1 == s2)`
b) `if (s1.equals(s2))`
c) `if (s1.compare(s2))`
d) `if (s1 = s2)`

### Pregunta 2.6
- ¿Qué imprime este código?
    ```java
    String s = "Programación";
    System.out.println(s.substring(0, 4));
    ```
    a) Prog
    b) Progr
    c) Progra
    d) Program

### Pregunta 2.7
- ¿Cuál es el valor de `miArray[2]`?
    ```java
    int[] miArray = {10, 20, 30, 40};
    ```
    a) 10
    b) 20
    c) 30
    d) 40

### Pregunta 2.8
- ¿Qué ocurre al acceder a `nums[5]` si `int[] nums = new int[5];`?
a) Devuelve 0
b) Error en tiempo de compilación
c) Error en tiempo de ejecución (ArrayIndexOutOfBoundsException)
d) Devuelve null

### Pregunta 2.9
- ¿Cuál es la sintaxis correcta del for-each para un array de Strings?
a) `for (String s : array)`
b) `for (String s in array)`
c) `foreach (String s in array)`
d) `for (String s = 0; s < array.length; s++)`

### Pregunta 2.10
- ¿Qué método convierte un String a minúsculas?
a) `toLowerCase()`
b) `toLower()`
c) `lowerCase()`
d) `toLow()`

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada método de String con su función:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. length() | A. Extrae parte del String |
    | 2. charAt() | B. Longitud del String |
    | 3. substring() | C. Compara contenido |
    | 4. equals() | D. Obtiene carácter por índice |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada operación con su resultado (`String s = "Java"`):

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. s.length() | A. "J" |
    | 2. s.charAt(0) | B. 4 |
    | 3. s.substring(1,3) | C. "av" |
    | 4. s.equals("JAVA") | D. false |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.3
- Relaciona cada declaración con su inicialización:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. int[] a = new int[3]; | A. `{10, 20, 30}` |
    | 2. int[] b = {10, 20, 30}; | B. `[0, 0, 0]` |
    | 3. int[] c = new int[]{10, 20, 30}; | C. `{10, 20, 30}` |

    **Respuesta:** `1-___, 2-___, 3-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) El primer índice de un array es 1.

### Pregunta 4.2
- (V) (F) La propiedad `length` de un array es un método.

### Pregunta 4.3
- (V) (F) Los Strings en Java son mutables (se pueden modificar).

### Pregunta 4.4
- (V) (F) `substring(2, 5)` devuelve caracteres desde el índice 2 hasta el 5 inclusive.

### Pregunta 4.5
- (V) (F) `String` es una clase en Java.

### Pregunta 4.6
- (V) (F) Se puede usar `==` para comparar contenido de Strings si se tiene cuidado.

### Pregunta 4.7
- (V) (F) Un array puede contener diferentes tipos de datos.

### Pregunta 4.8
- (V) (F) `equalsIgnoreCase()` compara Strings ignorando mayúsculas/minúsculas.

### Pregunta 4.9
- (V) (F) El bucle for-each permite modificar el array original.

### Pregunta 4.10
- (V) (F) `trim()` elimina todos los espacios de un String.

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `length`
1.2: `length`
1.3: `0`
1.4: `4`
1.5: `tamaño` (cualquier número)
1.6: `carácter`
1.7: `1`
1.8: `equals`
1.9: `mayúsculas`
1.10: `inicio`

### Respuestas de opción múltiple:
- 2.1: b
2.2: b
2.3: b
2.4: b
2.5: b
2.6: a ("Prog")
2.7: c
2.8: c
2.9: a
2.10: a

### Respuestas de relacionar:
- 3.1: 1-B, 2-D, 3-A, 4-C
3.2: 1-B, 2-A, 3-C, 4-D
3.3: 1-B, 2-A, 3-C

### Respuestas de verdadero/falso:
- 4.1: F (es 0)
4.2: F (es una propiedad)
4.3: F (son inmutables)
4.4: F (hasta 4, el 5 no se incluye)
4.5: V
4.6: F (no es recomendable)
4.7: F (todos los elementos deben ser del mismo tipo)
4.8: V
4.9: F (solo lectura)
4.10: F (solo espacios al inicio y final)

# Preguntas teóricas – Módulo 6: Métodos

## 1. Completar

### Pregunta 1.1
- La palabra clave ______ se usa cuando un método no devuelve ningún valor.

### Pregunta 1.2
- Para devolver un valor desde un método se usa la palabra clave ______.

### Pregunta 1.3
- Los valores que recibe un método se llaman ______.

### Pregunta 1.4
- Un método puede tener el mismo nombre que otro pero diferente lista de ______. Esto se llama sobrecarga.

### Pregunta 1.5
- Las variables declaradas dentro de un método se llaman variables ______.

### Pregunta 1.6
- El modificador ______ permite que un método pertenezca a la clase y no a los objetos.

### Pregunta 1.7
- La firma de un método incluye el nombre y la lista de ______.

### Pregunta 1.8
- Para llamar a un método estático desde el mismo `main` se usa el nombre del ______ o directamente el nombre del método.

### Pregunta 1.9
- Un método puede llamar a otros ______ dentro de su bloque de código.

### Pregunta 1.10
- La sobrecarga de métodos se basa en el número, tipo u ______ de los parámetros.

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Cuál es la firma del método?
    ```java
    public static int sumar(int a, int b)
    ```
    a) `sumar(int a, int b)`
    b) `public static int`
    c) `sumar`
    d) `int sumar`

### Pregunta 2.2
- ¿Qué palabra clave se usa para devolver un valor?
a) `return`
b) `void`
c) `output`
d) `give`

### Pregunta 2.3
- ¿Cuál es la salida?
    ```java
    public static void main(String[] args) {
        System.out.println(sumar(3, 4));
    }
    public static int sumar(int a, int b) {
        return a + b;
    }
    ```
    a) 3
    b) 4
    c) 7
    d) Error

### Pregunta 2.4
- ¿Cuál de estos métodos es válido como sobrecarga de `sumar(int a, int b)`?
a) `sumar(int a, int b, int c)`
b) `sumar(double a, double b)`
c) `sumar(int x, int y)`
d) `int sumar(int a, int b)`

### Pregunta 2.5
- ¿Qué imprime este código?
    ```java
    public static void cambiar(int x) {
        x = 10;
    }
    public static void main(String[] args) {
        int a = 5;
        cambiar(a);
        System.out.println(a);
    }
    ```
    a) 5
    b) 10
    c) Error
    d) null

### Pregunta 2.6
- ¿Cuál es el ámbito de una variable declarada dentro de un método?
a) Toda la clase
b) Solo dentro del método
c) Todo el programa
d) Solo dentro del main

### Pregunta 2.7
- ¿Qué método tiene retorno?
a) `public static void saludar()`
b) `public static int sumar()`
c) `public static void main()`
d) `public static void mostrar()`

### Pregunta 2.8
- ¿Cuál es la sintaxis correcta para llamar al método `calcular()` desde `main`?
a) `calcular();`
b) `calcular;`
c) `call calcular();`
d) `ejecutar calcular();`

### Pregunta 2.9
- ¿Cuántos parámetros puede tener un método?
a) Máximo 5
b) Máximo 10
c) Máximo 255
d) Los que sean necesarios

### Pregunta 2.10
- ¿Qué es la sobrecarga de métodos?
a) Varios métodos con el mismo nombre y diferentes parámetros
b) Un método que se llama a sí mismo
c) Un método que llama a otro
d) Varios métodos con diferentes nombres y mismos parámetros

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada parte de la firma con su función:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. public | A. Tipo de dato que devuelve |
    | 2. static | B. Nombre del método |
    | 3. int | C. Acceso público |
    | 4. sumar | D. Pertenece a la clase |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada tipo de método con su característica:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. void | A. Devuelve un valor |
    | 2. int | B. No devuelve valor |
    | 3. String | C. Devuelve texto |

    **Respuesta:** `1-___, 2-___, 3-___`

### Pregunta 3.3
- Relaciona cada código con su tipo de paso de parámetros (Java es siempre paso por valor):

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. `int a; metodo(a);` | A. Paso por valor |
    | 2. `int[] arr; metodo(arr);` | B. Paso por referencia de la referencia |

    **Respuesta:** `1-___, 2-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) Un método puede tener múltiples sentencias `return`.

### Pregunta 4.2
- (V) (F) El tipo de retorno puede ser cualquier tipo de datos.

### Pregunta 4.3
- (V) (F) Los parámetros son opcionales en un método.

### Pregunta 4.4
- (V) (F) Un método `void` puede usar `return;` para salir antes.

### Pregunta 4.5
- (V) (F) Java permite pasar métodos como parámetros a otros métodos.

### Pregunta 4.6
- (V) (F) La sobrecarga solo se basa en el tipo de retorno.

### Pregunta 4.7
- (V) (F) Las variables locales existen hasta que el programa termina.

### Pregunta 4.8
- (V) (F) Un método puede llamarse a sí mismo (recursión).

### Pregunta 4.9
- (V) (F) `public static void` es la firma completa del método.

### Pregunta 4.10
- (V) (F) Los métodos ayudan a reutilizar código y hacerlo más legible.

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `void`
1.2: `return`
1.3: `parámetros` (o `argumentos`)
1.4: `parámetros`
1.5: `locales`
1.6: `static`
1.7: `parámetros`
1.8: `método`
1.9: `métodos`
1.10: `orden`

### Respuestas de opción múltiple:
- 2.1: a
2.2: a
2.3: c
2.4: a y b (c y d son iguales, sobrecarga requiere diferencia en parámetros)
2.5: a (los primitivos se pasan por valor)
2.6: b
2.7: b
2.8: a
2.9: d
2.10: a

### Respuestas de relacionar:
- 3.1: 1-C, 2-D, 3-A, 4-B
3.2: 1-B, 2-A, 3-C
3.3: 1-A, 2-B

### Respuestas de verdadero/falso:
- 4.1: V (con condicionales)
4.2: V
4.3: V
4.4: V
4.5: F (usando lambdas sí, pero básico no)
4.6: F (solo en parámetros)
4.7: F (solo duran mientras el método se ejecuta)
4.8: V
4.9: F (es el encabezado, la firma es `nombre(parámetros)`)
4.10: V


**Guardar como:** `teoria_modulo7.md`


# Preguntas teóricas – Módulo 7: Programación Orientada a Objetos

## 1. Completar

### Pregunta 1.1
- Una ______ es una plantilla para crear objetos.

### Pregunta 1.2
- Un ______ es una instancia concreta de una clase.

### Pregunta 1.3
- Los atributos de una clase representan el ______ del objeto.

### Pregunta 1.4
- Los ______ definen el comportamiento de un objeto.

### Pregunta 1.5
- La palabra clave ______ se usa para crear un objeto.

### Pregunta 1.6
- El ______ es un método especial que se ejecuta al crear un objeto.

### Pregunta 1.7
- El modificador de acceso ______ hace que un atributo no sea accesible desde fuera de la clase.

### Pregunta 1.8
- Los métodos ______ permiten acceder a atributos privados.

### Pregunta 1.9
- Los métodos ______ permiten modificar atributos privados.

### Pregunta 1.10
- La palabra clave ______ se usa dentro de la clase para referirse al objeto actual.

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Cuál es la diferencia entre clase y objeto?
a) La clase es concreta, el objeto es abstracto
b) La clase es la plantilla, el objeto es la instancia
c) La clase tiene comportamiento, el objeto tiene estado
d) No hay diferencia

### Pregunta 2.2
- ¿Qué palabra clave se usa para crear un objeto?
a) `class`
b) `object`
c) `new`
d) `create`

### Pregunta 2.3
- ¿Cuál es el propósito del constructor?
a) Destruir el objeto
b) Inicializar los atributos
c) Mostrar información
d) Modificar atributos privados

### Pregunta 2.4
- ¿Qué modificador de acceso permite el acceso solo dentro de la misma clase?
a) `public`
b) `protected`
c) `private`
d) `package`

### Pregunta 2.5
- ¿Para qué sirve el encapsulamiento?
a) Hacer el código más rápido
b) Proteger los datos de modificaciones incorrectas
c) Crear más objetos
d) Eliminar métodos

### Pregunta 2.6
- ¿Qué es un getter?
a) Método que modifica un atributo
b) Método que devuelve el valor de un atributo
c) Método que elimina un atributo
d) Método que crea un objeto

### Pregunta 2.7
- ¿Qué imprime este código?
    ```java
    Persona p1 = new Persona("Ana");
    Persona p2 = new Persona("Ana");
    System.out.println(p1 == p2);
    ```
    a) true
    b) false
    c) Error
    d) null

### Pregunta 2.8
- ¿Qué palabra clave se usa para referirse al objeto actual?
a) `self`
b) `this`
c) `current`
d) `object`

### Pregunta 2.9
- ¿Cuál es la sintaxis correcta para crear un objeto `Perro`?
a) `Perro p = new Perro();`
b) `Perro p = new Perro;`
c) `Perro p = Perro();`
d) `new Perro p = Perro();`

### Pregunta 2.10
- ¿Qué beneficio NO proporciona el encapsulamiento?
a) Validación de datos
b) Ocultamiento de implementación
c) Mayor velocidad de ejecución
d) Mantenibilidad

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada concepto con su descripción:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. Clase | A. Instancia concreta |
    | 2. Objeto | B. Plantilla para crear objetos |
    | 3. Atributo | C. Comportamiento del objeto |
    | 4. Método | D. Estado del objeto |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada modificador con su nivel de acceso:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. public | A. Solo dentro de la clase |
    | 2. private | B. Desde cualquier lugar |
    | 3. (sin modificador) | C. Solo dentro del paquete |

    **Respuesta:** `1-___, 2-___, 3-___`

### Pregunta 3.3
- Relaciona cada constructor con su tipo:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. `public Persona() { }` | A. Constructor con parámetros |
    | 2. `public Persona(String n) { }` | B. Constructor por defecto |
    | 3. No escribir constructor | C. Constructor vacío implícito |

    **Respuesta:** `1-___, 2-___, 3-___`

---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) Una clase puede tener múltiples constructores.

### Pregunta 4.2
- (V) (F) Los atributos deberían ser siempre `public`.

### Pregunta 4.3
- (V) (F) El constructor tiene el mismo nombre que la clase.

### Pregunta 4.4
- (V) (F) Los getters siempre deben devolver el atributo sin modificar.

### Pregunta 4.5
- (V) (F) Los setters pueden incluir validaciones.

### Pregunta 4.6
- (V) (F) `this` se usa para diferenciar entre atributo y parámetro.

### Pregunta 4.7
- (V) (F) Un objeto puede crearse sin usar `new`.

### Pregunta 4.8
- (V) (F) Los métodos estáticos pertenecen a la clase, no a los objetos.

### Pregunta 4.9
- (V) (F) El encapsulamiento es opcional en Java.

### Pregunta 4.10
- (V) (F) Dos objetos creados con `new` son iguales si tienen los mismos atributos.

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `clase`
1.2: `objeto`
1.3: `estado`
1.4: `métodos`
1.5: `new`
1.6: `constructor`
1.7: `private`
1.8: `getters`
1.9: `setters`
1.10: `this`

### Respuestas de opción múltiple:
- 2.1: b
2.2: c
2.3: b
2.4: c
2.5: b
2.6: b
2.7: b (son dos objetos diferentes en memoria)
2.8: b
2.9: a
2.10: c

### Respuestas de relacionar:
- 3.1: 1-B, 2-A, 3-D, 4-C
3.2: 1-B, 2-A, 3-C
3.3: 1-B, 2-A, 3-C

### Respuestas de verdadero/falso:
- 4.1: V
4.2: F (deberían ser private)
4.3: V
4.4: V
4.5: V
4.6: V
4.7: F (siempre se necesita new)
4.8: V
4.9: F (es fundamental en POO)
4.10: F (son diferentes objetos en memoria)

# Preguntas teóricas – Módulo 8: Proyecto integrador

## 1. Completar

### Pregunta 1.1
- En el proyecto final, la clase que representa a los estudiantes se llama ______.

### Pregunta 1.2
- Para almacenar múltiples estudiantes se puede usar un array o un ______.

### Pregunta 1.3
- El menú del proyecto se implementa típicamente con un bucle ______ y una estructura ______.

### Pregunta 1.4
- Para buscar un estudiante por nombre se usa el método `equals______()` para ignorar mayúsculas/minúsculas.

### Pregunta 1.5
- El promedio de calificaciones se calcula sumando todas las calificaciones y dividiendo por la ______ de estudiantes.

### Pregunta 1.6
- Si no hay estudiantes registrados, al calcular el promedio se debe mostrar un mensaje de ______.

### Pregunta 1.7
- En la clase `Estudiante`, la edad debe ser ______ (positiva/mayor que cero).

### Pregunta 1.8
- En la clase `Estudiante`, la calificación debe estar entre ______ y ______.

### Pregunta 1.9
- El método `mostrarInfo()` muestra los ______ del estudiante.

### Pregunta 1.10
- Para salir del programa, la opción de menú debe romper el bucle ______.

---

## 2. Opción múltiple

### Pregunta 2.1
- ¿Qué estructura de control se usa para mostrar el menú repetidamente?
a) `if-else`
b) `switch`
c) `do-while` o `while`
d) `for`

### Pregunta 2.2
- ¿Qué tipo de estructura se usa para evaluar la opción del menú?
a) `if-else`
b) `switch`
c) Ambas son válidas
d) `for`

### Pregunta 2.3
- ¿Qué método se recomienda para buscar un estudiante por nombre ignorando mayúsculas?
a) `equals()`
b) `compareTo()`
c) `equalsIgnoreCase()`
d) `compareToIgnoreCase()`

### Pregunta 2.4
- Si el array tiene capacidad para 100 estudiantes, ¿qué variable se usa para saber cuántos hay actualmente?
a) `array.length`
b) `contador`
c) `capacidad`
d) `tamaño`

### Pregunta 2.5
- ¿Qué se debe hacer antes de calcular el promedio?
a) Verificar que hay al menos un estudiante
b) Ordenar los estudiantes
c) Mostrar la lista completa
d) Guardar en un archivo

### Pregunta 2.6
- ¿Qué mensaje se muestra si no hay estudiantes al listar?
a) "Lista vacía"
b) "No hay estudiantes registrados"
c) "Error"
d) "Listando..."

### Pregunta 2.7
- ¿Qué ventaja tiene usar `ArrayList` sobre un array fijo?
a) Es más rápido
b) No tiene límite fijo de tamaño
c) Es más fácil de declarar
d) No necesita importaciones

### Pregunta 2.8
- ¿Cómo se agrega un elemento a un `ArrayList<Estudiante>`?
a) `estudiantes.add(estudiante);`
b) `estudiantes[contador] = estudiante;`
c) `estudiantes.push(estudiante);`
d) `estudiantes.insert(estudiante);`

### Pregunta 2.9
- ¿Qué método del proyecto se encarga de mostrar todos los estudiantes?
a) `agregarEstudiante()`
b) `buscarEstudiante()`
c) `listarEstudiantes()`
d) `calcularPromedio()`

### Pregunta 2.10
- ¿Cuál es la opción típica para salir del programa?
a) 0
b) 5 (o la última opción)
c) Salir
d) Cualquier letra

---

## 3. Relacionar

### Pregunta 3.1
- Relaciona cada funcionalidad con su descripción:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. Agregar estudiante | A. Muestra todos los estudiantes |
    | 2. Listar estudiantes | B. Calcula el promedio |
    | 3. Buscar estudiante | C. Crea un nuevo objeto Estudiante |
    | 4. Calcular promedio | D. Encuentra por nombre |

    **Respuesta:** `1-___, 2-___, 3-___, 4-___`

### Pregunta 3.2
- Relaciona cada componente con su responsabilidad:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. Clase Estudiante | A. Lógica principal y menú |
    | 2. Clase SistemaEstudiantes | B. Define atributos y métodos |
    | 3. Método main | C. Punto de entrada |

    **Respuesta:** `1-___, 2-___, 3-___`

### Pregunta 3.3
- Relaciona cada validación con el atributo correspondiente:

    | Columna A | Columna B |
    |-----------|-----------|
    | 1. edad | A. Debe estar entre 0.0 y 10.0 |
    | 2. calificacion | B. Debe ser mayor a 0 |
    | 3. nombre | C. No puede estar vacío |

    **Respuesta:** `1-___, 2-___, 3-___`
---

## 4. Verdadero o Falso

### Pregunta 4.1
- (V) (F) El menú debe mostrarse solo una vez al inicio.

### Pregunta 4.2
- (V) (F) La opción de salir debe terminar el programa.

### Pregunta 4.3
- (V) (F) Es recomendable tener un método separado para cada funcionalidad del menú.

### Pregunta 4.4
- (V) (F) El proyecto no necesita validar la entrada del usuario.

### Pregunta 4.5
- (V) (F) Se puede usar tanto array como ArrayList para almacenar estudiantes.

### Pregunta 4.6
- (V) (F) El promedio debe mostrarse con un solo decimal.

### Pregunta 4.7
- (V) (F) La búsqueda por nombre debe ser exacta (case sensitive).

### Pregunta 4.8
- (V) (F) El método `mostrarInfo()` debe ser público.

### Pregunta 4.9
- (V) (F) El proyecto final integra todos los conceptos del curso.

### Pregunta 4.10
- (V) (F) Es obligatorio usar `ArrayList` en el proyecto.

---

## 📋 Respuestas

### Respuestas de completar:
- 1.1: `Estudiante`
1.2: `ArrayList`
1.3: `do-while` (o while), `switch` (o if-else)
1.4: `IgnoreCase`
1.5: `cantidad` (o número)
1.6: `advertencia` (o "No hay estudiantes")
1.7: `positiva`
1.8: `0`, `10`
1.9: `datos` (o atributos)
1.10: `principal` (o `do-while`)

### Respuestas de opción múltiple:
- 2.1: c
2.2: c
2.3: c
2.4: b
2.5: a
2.6: b
2.7: b
2.8: a
2.9: c
2.10: b

### Respuestas de relacionar:
- 3.1: 1-C, 2-A, 3-D, 4-B
3.2: 1-B, 2-A, 3-C
3.3: 1-B, 2-A, 3-C

### Respuestas de verdadero/falso:
- 4.1: F (debe mostrarse después de cada acción)
4.2: V
4.3: V
4.4: F (las validaciones son importantes)
4.5: V
4.6: F (con dos decimales es mejor, pero no obligatorio)
4.7: F (se recomienda `equalsIgnoreCase`)
4.8: V
4.9: V
4.10: F (no es obligatorio, se puede usar array)
