---

markmap:
  initialExpandLevel: 1
---

# **Módulo 5 – Arrays y cadenas**

## 1. Almacenando múltiples datos y manejando texto

## 2. Objetivos del módulo
- Declarar, inicializar y recorrer arrays
- Usar el bucle `for` mejorado (for-each)
- Aplicar métodos básicos de la clase `String`

## 3. Concepto de array (arreglo)
- Un array es una estructura que almacena múltiples valores del mismo tipo
- Los valores se almacenan en posiciones contiguas de memoria
- Cada posición se accede mediante un índice (empieza en 0)
- Tamaño fijo: se define al crearlo y no cambia

## 4. Declaración de arrays
- `int[] numeros;`
- `String[] nombres;`
- Otra sintaxis válida: `int numeros2[];`

## 5. Inicialización de arrays
- Con tamaño fijo: `int[] edades = new int[5];` → `[0, 0, 0, 0, 0]`
- Con valores explícitos: `int[] numeros = {10, 20, 30, 40, 50};`
- Con `new`: `String[] dias = new String[]{"Lun", "Mar", "Mié"};`
- Valores por defecto: `int` → `0`, `double` → `0.0`, `boolean` → `false`, `String` → `null`

## 6. Acceso a elementos (índices)
- ```
  int[] numeros = {10, 20, 30, 40, 50};
  System.out.println(numeros[0]);  // 10 (primer elemento)
  System.out.println(numeros[2]);  // 30 (tercer elemento)
  numeros[1] = 99;  // modifica el segundo elemento
  System.out.println(numeros[1]);  // 99
  ```
- Los índices van desde `0` hasta `length - 1`
- Acceder a un índice fuera de rango produce error: `ArrayIndexOutOfBoundsException`

## 7. Propiedad length de arrays
- `int[] nums = new int[10];` → `nums.length` → `10`
- `String[] nombres = {"Ana", "Luis"};` → `nombres.length` → `2`
- `length` es una propiedad, no un método (sin paréntesis)

## 8. Recorrido de arrays con for
- ```
  int[] numeros = {10, 20, 30, 40, 50};
  for (int i = 0; i < numeros.length; i++) {
      System.out.println(numeros[i]);
  }
  ```
- Útil cuando se necesita el índice

## 9. Recorrido con for mejorado (for-each)
- ```
  int[] numeros = {10, 20, 30, 40, 50};
  for (int valor : numeros) {
      System.out.println(valor);
  }
  ```
- Más simple y legible
- No se tiene acceso al índice
- No se puede modificar el array (solo lectura)

## 10. Ejemplo práctico con arrays
- ```
  int[] numeros = {5, 12, 8, 23, 16};
  int suma = 0;
  int maximo = numeros[0];
  for (int i = 0; i < numeros.length; i++) {
      suma += numeros[i];
      if (numeros[i] > maximo) {
          maximo = numeros[i];
      }
  }
  double promedio = (double) suma / numeros.length;
  System.out.println("Suma: " + suma);
  System.out.println("Promedio: " + promedio);
  System.out.println("Máximo: " + maximo);
  ```

## 11. Errores comunes con arrays
- Índice fuera de rango:
  - `int[] nums = new int[5]; nums[5] = 10;` → Error: índice máximo es 4
- Uso de `length` incorrecto:
  - `nums.length();` → Error: `length` no es método
- Olvidar inicializar:
  - `int[] nums; nums[0] = 5;` → Error: array `null`

## 12. Introducción a la clase String
- `String` es una clase en Java (no tipo primitivo)
- Los Strings son inmutables (no cambian después de crearse)
- Se pueden usar como tipos: `String nombre = "Juan";`
- Tiene muchos métodos útiles para manipular texto

## 13. Método length() de String
- ```
  String texto = "Hola mundo";
  int longitud = texto.length();  // 10
  ```
- `length()` es un **método** (con paréntesis)
- Diferente a la propiedad `length` de arrays

## 14. Método charAt()
- ```
  String texto = "Java";
  char letra = texto.charAt(0);  // 'J'
  char letra2 = texto.charAt(2); // 'v'
  ```
- Devuelve el carácter en una posición específica
- Índices desde `0` hasta `length() - 1`

## 15. Método substring()
- ```
  String texto = "Programación";
  String sub1 = texto.substring(0, 4);   // "Prog"
  String sub2 = texto.substring(4);      // "ramación"
  ```
- `substring(inicio)` → desde `inicio` hasta el final
- `substring(inicio, fin)` → desde `inicio` hasta `fin - 1`
- No modifica el original (devuelve un nuevo `String`)

## 16. Método equals() para comparar cadenas
- ```
  String a = "Hola";
  String b = "Hola";
  String c = "hola";
  System.out.println(a.equals(b));               // true
  System.out.println(a.equals(c));               // false
  System.out.println(a.equalsIgnoreCase(c));     // true
  ```
- **No usar `==` para comparar Strings** (compara referencias, no contenido)
- `equals()` compara el contenido textual
- `equalsIgnoreCase()` ignora mayúsculas/minúsculas

## 17. Otros métodos útiles de String
- `toUpperCase()` → convierte a mayúsculas: `"hola".toUpperCase()` → `"HOLA"`
- `toLowerCase()` → convierte a minúsculas: `"HOLA".toLowerCase()` → `"hola"`
- `trim()` → elimina espacios al inicio y final: `"  hola  ".trim()` → `"hola"`
- `indexOf()` → busca un carácter o substring: `"hola".indexOf('o')` → `1`
- `contains()` → verifica si contiene un substring: `"hola".contains("ol")` → `true`

## 18. Ejemplo completo con String
- ```
  String frase = "  Java es genial  ";
  String fraseLimpia = frase.trim();
  String fraseMayuscula = fraseLimpia.toUpperCase();
  System.out.println("Original: '" + frase + "'");
  System.out.println("Limpia: '" + fraseLimpia + "'");
  System.out.println("Mayúscula: '" + fraseMayuscula + "'");
  System.out.println("Longitud: " + fraseMayuscula.length());
  System.out.println("Primer carácter: " + fraseMayuscula.charAt(0));
  ```

## 19. Resumen del módulo
- **Arrays:**
  - Declaración: `int[] numeros;`
  - Inicialización: `new int[5]` o `{1, 2, 3}`
  - Acceso por índice: `numeros[0]`
  - Propiedad `length` → tamaño del array
  - Recorrido: `for` tradicional o `for-each`
- **String:**
  - Clase para texto: `String texto = "Hola";`
  - `length()` → longitud de la cadena (método)
  - `charAt(posición)` → carácter en posición
  - `substring(inicio, fin)` → extraer parte
  - `equals()` y `equalsIgnoreCase()` → comparar contenido
  - `toUpperCase()`, `toLowerCase()`, `trim()` → transformar
  - Strings son **inmutables** (no cambian, se crean nuevos)

## 20. Actividad práctica
- Enunciado: Crear un programa que almacene 5 nombres en un array y luego los muestre
- Tipos a usar: `String[]` para los nombres
- Estructuras a usar: `for` o `for-each` para recorrer
- Mostrar: cada nombre por consola usando `System.out.println`
- Ejecutar: probar en el IDE
- Ejemplo de salida esperada:
  - `Nombre 1: Ana`
  - `Nombre 2: Luis`
  - `Nombre 3: Carlos`
  - `Nombre 4: María`
  - `Nombre 5: José`
- Ampliación opcional 1: Crear un array de 5 números enteros, mostrar el mayor y el menor
- Ampliación opcional 2: Pedir una frase al usuario y mostrar cuántas vocales tiene (usar `charAt()` y un bucle)
- Ampliación opcional 3: Invertir el orden de los nombres del array y mostrarlos
