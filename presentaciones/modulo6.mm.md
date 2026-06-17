---

markmap:
  initialExpandLevel: 1
---


# **Módulo 6 – Métodos (funciones)**

## 1. Métodos (funciones)
- Organizando y reutilizando código

## 2. Objetivos del módulo
- Definir métodos con y sin parámetros
- Usar métodos con y sin retorno
- Comprender el ámbito de las variables
- Introducir la sobrecarga de métodos

## 3. Concepto de método o función
- Un método es un bloque de código con un nombre que se puede ejecutar cuando se le llama
- Ventajas:
  - Reutilización: escribir una vez, usar muchas veces
  - Organización: dividir problemas grandes en pequeños
  - Legibilidad: código más claro y fácil de mantener

## 4. Sintaxis de un método
- ```
  modificador tipo_retorno nombreMetodo(parámetros) {
      // Código del método
      return valor;  // si tipo_retorno no es void
  }
  ```
- Modificador: normalmente `public static` en este nivel
- Tipo retorno: `void` si no devuelve nada, o un tipo concreto (`int`, `double`, `String`, etc.)
- Nombre: verbo que indica la acción que realiza
- Parámetros: opcionales, van entre paréntesis

## 5. Tipo de retorno (void y tipos concretos)
- Método sin retorno (`void`):
  - ```
    public static void saludar() {
        System.out.println("Hola");
    }
    ```
- Método con retorno `int`:
  - ```
    public static int sumar(int a, int b) {
        return a + b;
    }
    ```
- `void` no necesita `return` (o usa `return;` para salir antes)
- Los demás tipos **obligan** a usar `return valor;`

## 6. Parámetros (argumentos)
- ```
  public static void saludar(String nombre) {
      System.out.println("Hola " + nombre);
  }
  
  public static int multiplicar(int a, int b) {
      return a * b;
  }
  ```
- Los parámetros son variables locales al método
- Se reciben los valores al llamar al método
- Puede haber 0, 1 o más parámetros

## 7. Llamada a un método
- ```
  public static void main(String[] args) {
      // Llamada a método void
      saludar("Ana");
      
      // Llamada a método con retorno
      int resultado = multiplicar(3, 5);
      System.out.println(resultado);  // 15
      
      // También se puede usar directamente
      System.out.println(multiplicar(4, 6));
  }
  ```

## 8. Ejemplo – método sin parámetros y sin retorno
- ```
  public static void mostrarMenu() {
      System.out.println("=== MENÚ ===");
      System.out.println("1. Agregar");
      System.out.println("2. Listar");
      System.out.println("3. Salir");
  }
  ```
- No recibe datos de entrada
- No devuelve ningún valor
- Solo ejecuta acciones internas (imprimir en pantalla)

## 9. Ejemplo – método con parámetros
- ```
  public static void imprimirSuma(int a, int b) {
      int suma = a + b;
      System.out.println("La suma de " + a + " + " + b + " es: " + suma);
  }
  ```
- Recibe datos para trabajar
- Puede tener múltiples parámetros del mismo o diferente tipo

## 10. Ejemplo – método con retorno
- ```
  public static int obtenerDoble(int numero) {
      return numero * 2;
  }
  
  // Uso:
  int x = 5;
  int doble = obtenerDoble(x);  // doble = 10
  ```
- El método produce un resultado que se puede usar en expresiones
- El tipo de retorno debe coincidir con el valor devuelto

## 11. Ámbito de variables (locales vs globales)
- **Variable local:** declarada dentro de un método. Solo existe dentro de ese método.
- **Variable de instancia/clase:** declarada dentro de la clase pero fuera de métodos. Existe mientras existe el objeto.
- **Parámetros:** también son variables locales.
- ```
  public static void miMetodo(int param) {
      int local = 10;   // variable local
      // param y local solo existen aquí dentro
  }
  // local NO se puede usar fuera del método
  ```

## 12. Sobrecarga de métodos (introducción)
- Varios métodos pueden tener el **mismo nombre** pero **diferentes parámetros** (número, tipo u orden)
- Java distingue cuál llamar según los argumentos
- ```
  public static int sumar(int a, int b) {
      return a + b;
  }
  
  public static double sumar(double a, double b) {
      return a + b;
  }
  
  public static int sumar(int a, int b, int c) {
      return a + b + c;
  }
  ```
- No basta con cambiar el tipo de retorno (solo los parámetros)

## 13. Ejemplo completo con métodos
- ```
  import java.util.Scanner;
  
  public class CalculadoraMetodos {
      
      public static int sumar(int a, int b) {
          return a + b;
      }
      
      public static int restar(int a, int b) {
          return a - b;
      }
      
      public static int multiplicar(int a, int b) {
          return a * b;
      }
      
      public static double dividir(int a, int b) {
          if (b != 0) {
              return (double) a / b;
          } else {
              System.out.println("Error: división por cero");
              return 0;
          }
      }
      
      public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
          System.out.print("Ingresa dos números: ");
          int x = sc.nextInt();
          int y = sc.nextInt();
          
          System.out.println("Suma: " + sumar(x, y));
          System.out.println("Resta: " + restar(x, y));
          System.out.println("Multiplicación: " + multiplicar(x, y));
          System.out.println("División: " + dividir(x, y));
      }
  }
  ```

## 14. Métodos que llaman a otros métodos
- Un método puede llamar a otros métodos
- ```
  public static int cuadrado(int n) {
      return n * n;
  }
  
  public static int sumaDeCuadrados(int a, int b) {
      return cuadrado(a) + cuadrado(b);
  }
  ```
- Facilita la reutilización y la organización del código

## 15. Buenas prácticas con métodos
- Usar nombres descriptivos (verbos en infinitivo o imperativo)
- Un método debe hacer **una sola cosa**
- Mantener los métodos cortos (idealmente menos de 20 líneas)
- Documentar métodos complejos con comentarios
- Evitar usar variables globales cuando se pueda usar parámetros
- Usar `void` solo cuando realmente no haya valor que retornar

## 16. Resumen del módulo
- **Método:** bloque de código reutilizable con un nombre
- **Sintaxis:** `modificador tipo_retorno nombre(parámetros) { código }`
- **Modificador común:** `public static`
- **Tipo retorno:**
  - `void` → no devuelve nada
  - `int`, `double`, `String`, etc. → devuelve un valor con `return`
- **Parámetros:** valores que recibe el método para trabajar
- **Llamada:** `nombreMetodo(argumentos);`
- **Ámbito:** variables locales solo existen dentro del método
- **Sobrecarga:** mismo nombre, diferentes parámetros

## 17. Actividad práctica
- Enunciado: Crear un programa con los siguientes métodos
- Método 1: `esPar(int numero)` → devuelve `true` si es par, `false` si es impar
- Método 2: `factorial(int n)` → devuelve el factorial de `n` (ej: `5! = 5*4*3*2*1 = 120`)
- Método 3: `esPrimo(int n)` → devuelve `true` si el número es primo, `false` si no
- Método 4: `mostrarMenu()` → muestra un menú de opciones sin parámetros y sin retorno
- En `main`: probar cada método con diferentes valores
- Ejecutar: probar en el IDE
- Ejemplo de salida esperada:
  - `esPar(4)` → `true`
  - `factorial(5)` → `120`
  - `esPrimo(7)` → `true`
  - `esPrimo(10)` → `false`
- Ampliación opcional 1: Método `sumaDigitos(int n)` que sume los dígitos de un número
- Ampliación opcional 2: Método `invertirNumero(int n)` que devuelva el número invertido (ej: 123 → 321)
- Ampliación opcional 3: Crear una calculadora completa con menú que use métodos para cada operación
