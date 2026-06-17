---

markmap:
  initialExpandLevel: 2
---
# Ejercicios prácticos – Módulo 1: Fundamentos de Java

## Ejercicio 1.1 – Mi primer programa
- Crea un programa llamado `HolaMundo.java` que muestre por consola "Hola, bienvenido a Java".

## Ejercicio 1.2 – Variables personales
- Declara variables para:
Tu nombre completo (`String`)
Tu edad (`int`)
Tu estatura en metros (`double`)
Tu letra inicial (`char`)
Si te gusta programar (`boolean`)

Muestra cada valor en una línea diferente.

## Ejercicio 1.3 – Datos de un producto
- Crea un programa que declare variables para:
    Nombre del producto
    Precio
    Cantidad en stock
    Disponible (true/false)

    Muestra toda la información formateada como:
    ```
    Producto: [nombre]
    Precio: [precio] $
    Stock: [cantidad] unidades
    Disponible: [true/false]
    ```

## Ejercicio 1.4 – Intercambio de valores
- Declara dos variables `a = 5` y `b = 10`. 
Intercambia sus valores usando una variable 
temporal. Muestra `Antes: a=5, b=10` y `Después: a=10, b=5`.

## Ejercicio 1.5 – Presentación personal
- Crea un programa que almacene tu nombre, edad, ciudad y profesión. Muestra:
    ```
    Hola, me llamo [nombre], tengo [edad] años, vivo en [ciudad] y soy [profesión].
    ```

## Ejercicio 1.6 – Operaciones básicas
- Declara dos números enteros: `num1 = 15` y `num2 = 4`. Calcula y muestra:
    - Suma
    - Resta
    - Multiplicación
    - División (resultado decimal)
    - Resto (módulo)

## Ejercicio 1.7 – Área de un rectángulo
- Declara `base = 8` y `altura = 5`. Calcula el área (base * altura) y
 el perímetro (2 * base + 2 * altura). Muestra los resultados.

## Ejercicio 1.8 – Conversión de tipos
- Declara `double precio = 19.99`. Conviértelo a `int` (casting) y muestra 
el valor entero. Luego declara `int cantidad = 7` y conviértelo a `double`, 
multiplícalo por el precio y muestra el total.

## Ejercicio 1.9 – Concatenación
- Declara `String nombre = "Carlos"`, `int edad = 30`, `String ciudad = "Lima"`. 
Muestra un mensaje que combine todo: "Carlos tiene 30 años y vive en Lima".

## Ejercicio 1.10 – Calculadora de propina
- Declara `double cuenta = 45.50` y `double porcentajePropina = 15`.
 Calcula la propina (cuenta * porcentaje/100) y el total a pagar.
  Muestra:
    ```
    Cuenta: 45.50
    Propina (15%): 6.825
    Total: 52.325
    ```

---




# Ejercicios prácticos – Módulo 2: Entrada de datos y operadores

## Ejercicio 2.1 – Saludo personalizado
- Pide al usuario su nombre y edad. Muestra: `Hola [nombre], tienes [edad] años`.

## Ejercicio 2.2 – Calculadora simple
- Pide dos números al usuario. Muestra:
    - Suma
    - Resta
    - Multiplicación
    - División (con decimales)
    - Módulo (resto)

## Ejercicio 2.3 – Calculadora de IMC
- Pide peso (kg) y altura (m). Calcula el IMC = peso / (altura * altura). 
Muestra el resultado con 2 decimales.

## Ejercicio 2.4 – Conversor de temperaturas
- Pide una temperatura en grados Celsius. Convierte a 
Fahrenheit usando: F = (C * 9/5) + 32. Muestra ambos valores.

## Ejercicio 2.5 – Par o impar
- Pide un número al usuario. Determina si es par o 
impar usando el operador módulo (`%`).

## Ejercicio 2.6 – Comparación de números
- Pide dos números. Muestra:
    Si el primero es mayor que el segundo
    Si son iguales
    Si el primero es menor

## Ejercicio 2.7 – Área de un círculo
- Pide el radio de un círculo. Calcula y muestra:
    $Área = π * r² $(usa Math.PI)
    $Circunferencia = 2 * π * r$

## Ejercicio 2.8 – Calculadora de promedio
- Pide tres calificaciones (decimales). Calcula el promedio y muéstralo.

## Ejercicio 2.9 – Conversor de segundos
- Pide una cantidad de segundos. Calcula y muestra los minutos y segundos 
equivalentes. Ejemplo: 125 segundos → 2 minutos y 5 segundos.

## Ejercicio 2.10 – Precio con descuento
- Pide el precio original y el porcentaje de descuento. Calcula y muestra:
    Descuento aplicado
    Precio final
    Ahorro total

## Ejercicio 2.11 – Mayor de tres números (operadores)
- Pide tres números. Usa operadores lógicos (`&&`) para determinar si el
 primero es el mayor de todos. Muestra `El primero es el mayor` o `El
  primero no es el mayor`.

## Ejercicio 2.12 – Rango de edad
- Pide una edad. Usa operadores lógicos para determinar si está entre 18 y 65 años (inclusive). 
Muestra `Está en edad laboral` o `No está en edad laboral`.


---



# Ejercicios prácticos – Módulo 3: Condicionales

## Ejercicio 3.1 – Día de la semana (switch)
- Pide un número del 1 al 7. Usa `switch` para mostrar el día correspondiente (Lunes a Domingo). 
Si el número está fuera de rango, muestra "Día no válido".

## Ejercicio 3.2 – Calificación en letra (if-else)
- Pide una nota (0-100). Usa `if-else` para mostrar:
    ```
    A: 90-100
    B: 80-89
    C: 70-79
    D: 60-69
    F: 0-59
    ```

## Ejercicio 3.3 – Número positivo, negativo o cero
- Pide un número. Determina si es positivo, negativo o cero.

## Ejercicio 3.4 – Calculadora con menú (switch)
- Muestra un menú:
    1. Sumar
    2. Restar
    3. Multiplicar
    4. Dividir
- Pide dos números y realiza la operación seleccionada usando 
`switch`. Maneja la división entre cero.

## Ejercicio 3.5 – Año bisiesto
- Pide un año. Determina si es bisiesto usando:
Divisible por 4 Y (no divisible por 100 O divisible por 400)

## Ejercicio 3.6 – Máximo de tres números (if-else)
- Pide tres números. Usa `if-else` para encontrar y mostrar el mayor.

## Ejercicio 3.7 – Días del mes (switch)
- Pide el número del mes (1-12). Usa `switch` para mostrar cuántos días
 tiene ese mes. Enero = 31, Febrero = 28, Marzo = 31, Abril = 30, etc.

## Ejercicio 3.8 – Categoría por edad (if-else)
- Pide una edad. Clasifica:
    Bebé: 0-2 años
    Niño: 3-12 años
    Adolescente: 13-17 años
    Adulto: 18-64 años
    Adulto mayor: 65+ años

## Ejercicio 3.9 – Triángulo válido
- Pide tres lados. Usa condicionales para determinar si forman un triángulo válido 
(cada lado debe ser menor que la suma de los otros dos). Muestra "Es un triángulo válido" o
 "No es un triángulo válido".

## Ejercicio 3.10 – Calculadora de impuestos (operador ternario)
- Pide el salario de una persona. Usa el operador ternario para calcular:
Si salario > 2000, impuesto = salario * 0.20
Si no, impuesto = salario * 0.10
Muestra el impuesto y el salario neto.

## Ejercicio 3.11 – Número par o impar (ternario)
- Pide un número. Usa el operador ternario para asignar a una variable
 String el texto "Par" o "Impar". Luego muestra el resultado.

## Ejercicio 3.12 – Tipo de carácter
- Pide un carácter. Determina si es vocal (a,e,i,o,u), consonante 
o dígito. Usa `switch` con `char`.


---




# Ejercicios prácticos – Módulo 4: Bucles

## Ejercicio 4.1 – Tabla de multiplicar (for)
- Pide un número al usuario. Usa `for` para mostrar su tabla de multiplicar del 1 al 10.

## Ejercicio 4.2 – Suma hasta 0 (while)
- Pide números al usuario hasta que ingrese 0. Muestra la suma total de todos los 
números ingresados (sin incluir el 0).

## Ejercicio 4.3 – Números pares (for)
- Usa `for` para mostrar todos los números pares entre 1 y 100.

## Ejercicio 4.4 – Factorial (while)
- Pide un número entero positivo. Usa `while` para calcular su 
factorial (ej: $5! = 5*4*3*2*1 = 120$).

## Ejercicio 4.5 – Pirámide de asteriscos (for anidados)
- Usa `for` anidados para imprimir:
    ```
    *
    **
    ***
    ****
    *****
    ```

## Ejercicio 4.6 – Adivina el número (do-while)
- Genera un número aleatorio entre 1 y 100 (usa `Math.random()`). Pide 
al usuario que adivine. Usa `do-while` para seguir pidiendo hasta que 
acierte. Muestra "Muy alto", "Muy bajo" o "Correcto".

## Ejercicio 4.7 – Suma de dígitos (while)
- Pide un número entero. Usa `while` para sumar sus dígitos. Ejemplo: $123 → 1+2+3 = 6$.

## Ejercicio 4.8 – Tabla de multiplicar completa (for anidados)
- Usa `for` anidados para mostrar todas las tablas de multiplicar del 1 al 10.

## Ejercicio 4.9 – Secuencia Fibonacci (for)
- Pide un número `n`. Usa `for` para mostrar los primeros `n`
 números de la secuencia Fibonacci (0,1,1,2,3,5,8...).

## Ejercicio 4.10 – Números primos (for + if)
- Pide un número. Usa `for` y condicionales para determinar si es primo.
 Un número primo solo es divisible por 1 y por sí mismo.

## Ejercicio 4.11 – Pirámide invertida (for anidados)
- Usa `for` anidados para imprimir:
    ```
    *****
    ****
    ***
    **
    *
    ```

## Ejercicio 4.12 – Contador de vocales (for + `charAt`)
- Pide una frase al usuario. Usa `for` para recorrer cada 
carácter (`.charAt()`) y contar cuántas vocales tiene.

---




# Ejercicios prácticos – Módulo 5: Arrays y cadenas

## Ejercicio 5.1 – Mostrar array
- Crea un array de 5 nombres. Recórrelo con `for` y muestra cada nombre.

## Ejercicio 5.2 – Mayor y menor
- Crea un array de 5 números enteros. Encuentra y muestra el mayor y el menor valor.

## Ejercicio 5.3 – Suma y promedio
- Crea un array de 6 números decimales. Calcula y muestra la suma y el promedio.

## Ejercicio 5.4 – Invertir array
- Crea un array de 4 elementos. Muestra el array original y 
luego el array invertido. Ejemplo: `[1,2,3,4] → [4,3,2,1]`

## Ejercicio 5.5 – Buscar en array
- Crea un array de 5 colores. Pide un color al usuario y busca si está en el array. 
Muestra "Encontrado" o  "No encontrado". Usa `equals()` para comparar Strings.

## Ejercicio 5.6 – Contar vocales en frase (String)
- Pide una frase al usuario. Usa `charAt()` y un bucle 
`for` para contar cuántas vocales tiene la frase.

## Ejercicio 5.7 – Invertir texto
- Pide una palabra al usuario. Usa `charAt()` y un bucle `for` 
para mostrar la palabra invertida. Ejemplo: "Hola" → "aloH".

## Ejercicio 5.8 – Palíndromo
- Pide una palabra al usuario. Determina si es palíndromo (se lee 
igual al derecho y al revés). Ejemplo: "reconocer" es palíndromo.

## Ejercicio 5.9 – Mayúsculas y minúsculas
- Pide una frase al usuario. Muestra la frase en mayúsculas, en 
minúsculas y con la primera letra de cada palabra en mayúscula.

## Ejercicio 5.10 – Eliminar espacios
- Pide una frase al usuario. Usa `trim()` para eliminar espacios al inicio y final. 
Luego reemplaza los espacios internos por guiones bajos usando `replace()`.

## Ejercicio 5.11 – Contador de palabras
- Pide una frase al usuario. Usa `split(" ")` para separar por 
espacios y cuenta cuántas palabras tiene la frase.

## Ejercicio 5.12 – For-each con array
- Crea un array de 6 números enteros. Usa un bucle `for-each` 
para mostrar cada número multiplicado por 2.

## Ejercicio 5.13 – Subcadena
- Pide una frase al usuario. Extrae y muestra los primeros 3 
caracteres y los últimos 3 caracteres usando `substring()`.

## Ejercicio 5.14 – Reemplazar caracteres
- Pide una frase al usuario. Reemplaza todas las vocales 'a' por '@', 'e' 
por '3', 'i' por '1', 'o' por '0', 'u' por 'u'. Usa `replace()` o `replaceAll()`.

## Ejercicio 5.15 – Validar email
- Pide un email al usuario. Usa métodos de String para verificar si contiene '@' 
y si contiene un punto después del '@'. Muestra "Email válido" o "Email inválido".

---




# Ejercicios prácticos – Módulo 6: Métodos

## Ejercicio 6.1 – Método saludar
- Crea un método `saludar(String nombre)` que reciba un nombre y 
muestre "Hola, [nombre]". Llámalo desde `main`.

## Ejercicio 6.2 – Método sumar
- Crea un método `sumar(int a, int b)` que devuelva la suma. 
Pruébalo con diferentes valores.

## Ejercicio 6.3 – Método esPar
- Crea un método `esPar(int numero)` que devuelva `true` si 
es par, `false` si es impar. Pruébalo con varios números.

## Ejercicio 6.4 – Método factorial
- Crea un método `factorial(int n)` que devuelva el factorial de `n` (ej: `5! = 120`). 
Usa un bucle `for` o `while`. Maneja el factorial de 0 (debe ser 1).

## Ejercicio 6.5 – Método esPrimo
- Crea un método `esPrimo(int n)` que devuelva `true` si el número es primo,
 `false` si no. Pruébalo con varios números.

## Ejercicio 6.6 – Método área del círculo
- Crea un método `areaCirculo(double radio)` que devuelva el 
área ($π * r²$). Usa `Math.PI`.

## Ejercicio 6.7 – Método máximo
- Crea un método `maximo(int a, int b, int c)` que 
devuelva el mayor de los tres números.

## Ejercicio 6.8 – Método sumaDigitos
- Crea un método `sumaDigitos(int n)` que sume los dígitos 
de un número. Ejemplo: $123 → 6$.

## Ejercicio 6.9 – Método invertirNumero
- Crea un método `invertirNumero(int n)` que devuelva 
el número invertido. Ejemplo: 123 → 321.

## Ejercicio 6.10 – Método mostrarMenu
- Crea un método `mostrarMenu()` que muestre un menú sin 
parámetros y sin retorno. Llámalo desde `main`.

## Ejercicio 6.11 – Calculadora con métodos
- Crea métodos separados para:
    ```
    sumar(a,b)
    restar(a,b)
    multiplicar(a,b)
    dividir(a,b)
    ```

- En `main`, pide dos números y llama a cada método mostrando los resultados.

## Ejercicio 6.12 – Sobrecarga de métodos
- Crea tres métodos llamados `multiplicar`:
    - `multiplicar(int a, int b)` → devuelve int
    - `multiplicar(double a, double b)` → devuelve double
    - `multiplicar(int a, int b, int c)` → devuelve int

- Prueba los tres desde `main`.

## Ejercicio 6.13 – Método validarEdad
- Crea un método `validarEdad(int edad)` que devuelva `true` si la edad
 está entre 0 y 120, `false` si no. Úsalo para validar entrada del usuario.

## Ejercicio 6.14 – Método convertirTemperatura
- Crea un método `celsiusAFahrenheit(double celsius)` que devuelva la conversión. 
También crea `fahrenheitACelsius(double fahrenheit)`. Prueba ambos.

## Ejercicio 6.15 – Método generarContraseña
- Crea un método `generarContraseña(int longitud)` que devuelva un String con una 
contraseña aleatoria de la longitud indicada (solo letras minúsculas).


---


# Ejercicios prácticos – Módulo 7: POO

## Ejercicio 7.1 – Clase `Persona`
- Crea una clase `Persona` con atributos:
    - `nombre` (String)
    - `edad` (int)

- Métodos:
    - Constructor que reciba nombre y edad
    - `mostrarInfo()` que muestre los datos

- Desde `main`, crea dos objetos `Persona` y muestra su información.

## Ejercicio 7.2 – Clase Perro
- Crea una clase `Perro` con atributos:
    - `nombre` (String)
    - `raza` (String)
    - `edad` (int)

- Métodos:
    - Constructor que reciba todos los atributos
    - `ladrar()` que muestre "Guau guau"

- Crea un objeto y haz que ladre.

## Ejercicio 7.3 – Clase CuentaBancaria (con encapsulamiento)
- Crea una clase `CuentaBancaria` con atributos privados:
    - `numeroCuenta` (String)
    - `saldo` (double)

- Métodos:
    - Constructor que reciba número de cuenta y saldo inicial
    - Getters para ambos atributos
    - Setter solo para saldo (con validación: saldo no puede ser negativo)
    - `depositar(double monto)`
    - `retirar(double monto)`

- Desde `main`, crea una cuenta, deposita, retira y muestra el saldo.

## Ejercicio 7.4 – Clase Libro
- Crea una clase `Libro` con atributos privados:
    - `titulo` (String)
    - `autor` (String)
    - `paginas` (int)

- Métodos:
    - Constructor completo
    - Getters y setters
    - `leer()` que muestre "Estás leyendo [titulo] de [autor]"
    - `mostrarInfo()`

- Crea tres libros y muestra su información.

## Ejercicio 7.5 – Clase Coche
- Crea una clase `Coche` con atributos privados:
    - `marca` (String)
    - `modelo` (String)
    - `velocidad` (int) (inicia en 0)

- Métodos:
    - Constructor que reciba marca y modelo
    - Getters para todos los atributos
    - `acelerar(int incremento)` → aumenta velocidad
    - `frenar(int decremento)` → disminuye velocidad
    - `mostrarVelocidad()`

- Desde `main`, acelera y frena varias veces mostrando la velocidad actual.

## Ejercicio 7.6 – Clase Producto
- Crea una clase `Producto` con atributos privados:
    - `nombre` (String)
    - `precio` (double)
    - `cantidad` (int)

- Métodos:
    - Constructor completo
    - Getters y setters
    - `calcularTotal()` que devuelva precio * cantidad
    - `aplicarDescuento(double porcentaje)` que reduzca el precio

- Desde `main`, crea un producto, aplica un descuento y muestra el total.

## Ejercicio 7.7 – Clase Estudiante (para proyecto final)
- Crea una clase `Estudiante` con atributos privados:
    - `nombre` (String)
    - `edad` (int)
    - `calificacion` (double)

- Métodos:
    - Constructor
    - Getters y setters (validar edad > 0, calificación 0-10)
    - `mostrarInfo()`

- Desde `main`, crea un array de 3 estudiantes y muestra su información.

## Ejercicio 7.8 – Clase Rectangulo
- Crea una clase `Rectangulo` con atributos privados:
    - `base` (double)
    - `altura` (double)

- Métodos:
    - Constructor que reciba base y altura
    - `calcularArea()` → base * altura
    - `calcularPerimetro()` → 2*(base + altura)
    - `esCuadrado()` → devuelve true si base == altura

- Desde `main`, crea varios rectángulos y prueba los métodos.

## Ejercicio 7.9 – Clase Fecha
- Crea una clase `Fecha` con atributos privados:
    - `dia` (int)
    - `mes` (int)
    - `anio` (int)

- Métodos:
    - Constructor
    - Getters y setters (validar día 1-31, mes 1-12)
    - `mostrarFormatoCorto()` → dd/mm/aaaa
    - `mostrarFormatoLargo()` → 15 de Enero de 2024

- Desde `main`, crea una fecha y muéstrala en ambos formatos.

## Ejercicio 7.10 – Clase Banco (con array de cuentas)
- Crea una clase `Banco` con atributo privado:
    - `cuentas` (array de CuentaBancaria, máximo 10)

- Métodos:
    - `agregarCuenta(CuentaBancaria cuenta)`
    - `mostrarTodasLasCuentas()`
    - `buscarCuenta(String numeroCuenta)`

- Desde `main`, crea un banco, agrega varias cuentas y búscalas.

---



# Ejercicios prácticos – Módulo 8: Proyecto integrador

## Proyecto: Sistema de Gestión de Estudiantes

### Requisitos obligatorios:

1. **Clase Estudiante** con:
- Atributos privados: `nombre`, `edad`, `calificacion`
- Constructor que reciba todos los atributos
- Getters y setters con validaciones:
- Edad debe ser mayor a 0
- Calificación debe estar entre 0.0 y 10.0
- Método `mostrarInfo()` que muestre todos los datos

2. **Clase SistemaEstudiantes** con:
- `main` que ejecute el programa
- Menú con opciones:
1. Agregar estudiante
2. Listar estudiantes
3. Buscar estudiante por nombre
4. Calcular promedio de calificaciones
5. Salir
- Array o `ArrayList` para almacenar estudiantes

3. **Funcionalidades específicas:**

### Ejercicio 8.1 – Agregar estudiante
- Pide al usuario: nombre, edad, calificación. Crea un objeto `Estudiante` 
y agrégalo al array. Muestra mensaje de confirmación.

### Ejercicio 8.2 – Listar estudiantes
- Recorre el array y muestra la información de cada estudiante usando `mostrarInfo()`. 
Si no hay estudiantes, muestra "No hay estudiantes registrados".

### Ejercicio 8.3 – Buscar estudiante por nombre
- Pide un nombre al usuario. Recorre el array y muestra los datos del estudiante si lo encuentra 
(usa `equalsIgnoreCase()`). Si no lo encuentra, muestra "Estudiante no encontrado".

### Ejercicio 8.4 – Calcular promedio
- Recorre el array, suma todas las calificaciones y calcula el promedio. Muestra el resultado con 2 decimales. 
Si no hay estudiantes, muestra "No hay estudiantes para calcular promedio".

### Ejercicio 8.5 – Menú completo
- Implementa el menú con `do-while` y `switch`. El programa debe 
seguir funcionando hasta que el usuario elija la opción 5.

---

## Ampliaciones opcionales:

### Opción 1 – Usar ArrayList
- Reemplaza el array fijo por `ArrayList<Estudiante>` para que no haya límite de estudiantes.

### Opción 2 – Eliminar estudiante
- Agrega una opción en el menú para eliminar un estudiante por nombre.

### Opción 3 – Ordenar estudiantes
- Agrega una opción para ordenar los estudiantes por calificación (de mayor a menor).

### Opción 4 – Validar entrada
- Valida que el usuario no ingrese edades negativas ni calificaciones
 fuera de rango. Pide repetir la entrada si es inválida.

### Opción 5 – Guardar en archivo
- Agrega una opción para guardar los estudiantes en un archivo 
de texto y otra para cargarlos.

### Opción 6 – Buscar por rango de calificación
- Agrega una opción para buscar estudiantes con calificación 
mayor a un valor ingresado.

### Opción 7 – Modificar estudiante
- Agrega una opción para modificar la calificación de un 
estudiante existente (buscándolo por nombre).

### Opción 8 – Contador de estudiantes
- Muestra en el menú cuántos estudiantes hay registrados actualmente.

### Opción 9 – Mejor y peor estudiante
- Agrega una opción para mostrar el estudiante con la calificación más alta y el de la más baja.

### Opción 10 – Reporte completo
- Agrega una opción que muestre un reporte con:
    - Total de estudiantes
    - Promedio general
    - Cantidad de aprobados (calificación >= 6.0)
    - Cantidad de reprobados (calificación < 6.0)
