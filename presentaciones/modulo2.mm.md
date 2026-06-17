---

markmap:
  initialExpandLevel: 1
---

# **Módulo 2 – Entrada de datos y operadores**

## 1. Interactuando con el usuario y realizando cálculos

## 2. Objetivos del módulo
- Leer datos ingresados por el usuario con `Scanner`
- Usar operadores aritméticos, relacionales y lógicos
- Comprender la precedencia de operadores

## 3. La clase Scanner
- Permite leer datos desde el teclado
- Pertenece al paquete `java.util`
- Importar: `import java.util.Scanner;`
- Crear: `Scanner sc = new Scanner(System.in);`

## 4. Métodos principales de Scanner
- `nextInt()` → Lee un número entero
- `nextDouble()` → Lee un número decimal
- `nextLine()` → Lee una línea de texto
- `next()` → Lee una palabra (hasta espacio en blanco)

## 5. Ejemplo de lectura de datos
- ```
  import java.util.Scanner;
  public class Lectura {
      public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
          System.out.print("Ingresa tu nombre: ");
          String nombre = sc.nextLine();
          System.out.print("Ingresa tu edad: ");
          int edad = sc.nextInt();
          System.out.println("Hola " + nombre + ", tienes " + edad + " años");
      }
  }
  ```

## 6. Operadores aritméticos
- `+` → Suma
- `-` → Resta
- `*` → Multiplicación
- `/` → División
- `%` → Módulo (resto de la división)

## 7. Prioridad de operadores aritméticos
- 1. Paréntesis `()`
- 2. Multiplicación, división, módulo (`*`, `/`, `%`)
- 3. Suma y resta (`+`, `-`)
- Ejemplo: `3 + 5 * 2` → `3 + 10` → `13`

## 8. Operadores relacionales
- `==` → Igual a
- `!=` → Diferente de
- `>` → Mayor que
- `<` → Menor que
- `>=` → Mayor o igual que
- `<=` → Menor o igual que
- Resultado: siempre `true` o `false`

## 9. Operadores lógicos
- `&&` → Y (AND) → true solo si ambos operandos son true
- `||` → O (OR) → true si al menos uno de los operandos es true
- `!` → No (NOT) → invierte el valor (true se vuelve false y viceversa)

## 10. Tabla de verdad básica
- `true && true` = `true`
- `true && false` = `false`
- `false && true` = `false`
- `false && false` = `false`
- `true || true` = `true`
- `true || false` = `true`
- `false || true` = `true`
- `false || false` = `false`
- `!true` = `false`
- `!false` = `true`

## 11. Precedencia de operadores (completa)
- 1. Paréntesis `()`
- 2. Operadores unarios (`!`)
- 3. Multiplicativos (`*`, `/`, `%`)
- 4. Aditivos (`+`, `-`)
- 5. Relacionales (`>`, `<`, `>=`, `<=`)
- 6. Igualdad (`==`, `!=`)
- 7. AND lógico (`&&`)
- 8. OR lógico (`||`)

## 12. Expresiones mixtas y conversión de tipos
- Si mezclas `int` y `double`, el resultado es `double`
- Ejemplo: `5 / 2.0` → `2.5`
- Si mezclas `int` y `int`, el resultado es `int`
- Ejemplo: `5 / 2` → `2` (división entera, se pierde el decimal)
- Casting explícito (convertir): `(int) 3.14` → `3`

## 13. Errores comunes con Scanner
- Olvidar `import java.util.Scanner;`
- Usar `nextLine()` después de `nextInt()` → consume el salto de línea pendiente
- Solución: agregar `sc.nextLine();` después de `nextInt()`

## 14. Ejemplo completo con operadores
- ```
  import java.util.Scanner;
  public class Calculadora {
      public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
          System.out.print("Ingresa el primer número: ");
          int a = sc.nextInt();
          System.out.print("Ingresa el segundo número: ");
          int b = sc.nextInt();
          int suma = a + b;
          int resta = a - b;
          int producto = a * b;
          int division = a / b;
          int modulo = a % b;
          boolean esMayor = a > b;
          System.out.println("Suma: " + suma);
          System.out.println("Resta: " + resta);
          System.out.println("Producto: " + producto);
          System.out.println("División: " + division);
          System.out.println("Módulo: " + modulo);
          System.out.println("¿Es a mayor que b? " + esMayor);
      }
  }
  ```

## 15. Buenas prácticas
- Cerrar el `Scanner` al final: `sc.close();`
- Usar nombres descriptivos para las variables
- Validar la entrada del usuario cuando sea posible
- Usar paréntesis para claridad en expresiones complejas

## 16. Resumen del módulo
- `Scanner` → clase para leer entrada del usuario
- `import java.util.Scanner;` → necesario para usar Scanner
- `Scanner sc = new Scanner(System.in);` → crear objeto Scanner
- `nextInt()`, `nextDouble()`, `nextLine()` → métodos para leer datos
- Operadores aritméticos: `+`, `-`, `*`, `/`, `%`
- Operadores relacionales: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Operadores lógicos: `&&` (AND), `||` (OR), `!` (NOT)
- Precedencia: `()` → `!` → `*/%` → `+-` → `><>=<=` → `==!=` → `&&` → `||`
- Casting: convertir un tipo a otro con `(tipo)`

## 17. Actividad práctica
- Enunciado: Crear un programa que pida dos números al usuario
- Tipos a usar: `int` para los dos números
- Operaciones a realizar: suma, resta, multiplicación, división, módulo
- Mostrar: cada resultado por consola usando `System.out.println`
- Adicional: mostrar si el primer número es mayor que el segundo (usar operador relacional)
- Ejecutar: probar en el IDE con diferentes valores
- Ejemplo de entrada: `primer número = 10`, `segundo número = 3`
- Ejemplo de salida esperada:
  - `Suma: 13`
  - `Resta: 7`
  - `Producto: 30`
  - `División: 3`
  - `Módulo: 1`
  - `¿Es 10 mayor que 3? true`
- Ampliación opcional: pedir un tercer número y mostrar el promedio de los tres
