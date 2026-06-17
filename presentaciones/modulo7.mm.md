---

markmap:
  initialExpandLevel: 1
---

# **Módulo 7 – Introducción a la Programación Orientada a Objetos**

## 1. Introducción a la Programación Orientada a Objetos
- Clases, objetos y encapsulamiento

## 2. Objetivos del módulo
- Comprender los conceptos de clase y objeto
- Definir clases con atributos, métodos y constructores
- Crear objetos y usarlos
- Aplicar encapsulamiento con `private` y getters/setters

## 3. Paradigma orientado a objetos
- Modela el mundo real mediante **objetos**
- Cada objeto tiene:
  - **Estado** (atributos / propiedades)
  - **Comportamiento** (métodos)
- Ventajas: reutilización, modularidad, facilidad de mantenimiento

## 4. Concepto de clase
- Una **clase** es un plano o plantilla para crear objetos
- Define los atributos y métodos que tendrán los objetos
- No ocupa memoria por sí sola
- Ejemplo: Clase `Perro` define que todo perro tiene nombre, edad y puede ladrar

## 5. Concepto de objeto
- Un **objeto** es una instancia concreta de una clase
- Tiene valores específicos para sus atributos
- Ocupa memoria en el heap
- Ejemplo: `Perro miPerro = new Perro();`

## 6. Atributos (variables de instancia)
- Variables declaradas dentro de la clase, pero fuera de los métodos
- Representan el estado del objeto
- Cada objeto tiene sus propios valores
- ```
  public class Perro {
      String nombre;   // atributo
      int edad;        // atributo
  }
  ```

## 7. Métodos de instancia
- Métodos que operan sobre los atributos de un objeto específico
- Pueden acceder a los atributos directamente
- ```
  public class Perro {
      String nombre;
      
      public void ladrar() {
          System.out.println(nombre + " dice guau");
      }
  }
  ```

## 8. Sintaxis de una clase en Java
- ```
  public class NombreClase {
      // Atributos
      tipo nombreAtributo;
      
      // Constructor
      public NombreClase(parámetros) {
          // inicializar atributos
      }
      
      // Métodos
      public tipoRetorno nombreMetodo() {
          // código
      }
  }
  ```

## 9. Creación de objetos (palabra new)
- ```
  Perro miPerro = new Perro();
  miPerro.nombre = "Rex";
  miPerro.edad = 3;
  miPerro.ladrar();
  ```
- `new` reserva memoria y llama al constructor

## 10. El constructor (propósito y sintaxis)
- Método especial que se ejecuta al crear un objeto (`new`)
- Tiene el mismo nombre que la clase
- No tiene tipo de retorno (ni `void`)
- Sirve para inicializar los atributos
- ```
  public class Perro {
      String nombre;
      
      public Perro(String nombre) {
          this.nombre = nombre;
      }
  }
  ```

## 11. Constructor por defecto y parametrizado
- ```
  public class Persona {
      String nombre;
      int edad;
      
      // Constructor por defecto
      public Persona() {
          nombre = "Sin nombre";
          edad = 0;
      }
      
      // Constructor parametrizado
      public Persona(String nombre, int edad) {
          this.nombre = nombre;
          this.edad = edad;
      }
  }
  ```
- Si no escribes ningún constructor, Java proporciona uno por defecto vacío
- Puedes tener múltiples constructores (sobrecarga)

## 12. Acceso a atributos y métodos (operador punto)
- ```
  Persona p1 = new Persona("Ana", 25);
  Persona p2 = new Persona();
  
  System.out.println(p1.nombre);  // Ana
  p1.edad = 26;                   // modificar
  
  p2.nombre = "Luis";
  p2.edad = 30;
  ```

## 13. Encapsulamiento – modificador private
- Los atributos deberían ser `private` (no accesibles desde fuera de la clase)
- Protege los datos de modificaciones incorrectas
- ```
  public class Persona {
      private String nombre;
      private int edad;
  }
  
  // Esto daría ERROR:
  Persona p = new Persona();
  p.nombre = "Ana";  // Error: nombre es private
  ```

## 14. Métodos getters y setters
- **Getter:** método público que devuelve el valor de un atributo privado
- **Setter:** método público que modifica el valor de un atributo privado (puede incluir validaciones)
- ```
  public class Persona {
      private String nombre;
      private int edad;
      
      // Getter
      public String getNombre() {
          return nombre;
      }
      
      // Setter
      public void setNombre(String nombre) {
          this.nombre = nombre;
      }
      
      public int getEdad() {
          return edad;
      }
      
      public void setEdad(int edad) {
          if (edad >= 0) {
              this.edad = edad;
          }
      }
  }
  ```

## 15. Beneficios del encapsulamiento
- **Control:** se puede validar antes de modificar (ej: edad no negativa)
- **Ocultamiento:** los detalles internos no son visibles
- **Mantenibilidad:** se puede cambiar la implementación interna sin afectar a quien usa la clase
- **Seguridad:** se evitan modificaciones accidentales

## 16. Ejemplo completo de clase con encapsulamiento
- ```
  public class CuentaBancaria {
      private String numeroCuenta;
      private double saldo;
      
      // Constructor
      public CuentaBancaria(String numeroCuenta, double saldoInicial) {
          this.numeroCuenta = numeroCuenta;
          if (saldoInicial >= 0) {
              this.saldo = saldoInicial;
          } else {
              this.saldo = 0;
          }
      }
      
      // Getters
      public String getNumeroCuenta() {
          return numeroCuenta;
      }
      
      public double getSaldo() {
          return saldo;
      }
      
      // Métodos de negocio
      public void depositar(double monto) {
          if (monto > 0) {
              saldo += monto;
              System.out.println("Depósito exitoso. Nuevo saldo: " + saldo);
          } else {
              System.out.println("El monto debe ser positivo");
          }
      }
      
      public void retirar(double monto) {
          if (monto > 0 && monto <= saldo) {
              saldo -= monto;
              System.out.println("Retiro exitoso. Nuevo saldo: " + saldo);
          } else {
              System.out.println("Monto inválido o saldo insuficiente");
          }
      }
  }
  ```

## 17. Buenas prácticas con POO
- Usar `private` para atributos (encapsulamiento)
- Proporcionar getters y setters solo cuando sean necesarios
- Usar nombres descriptivos para clases, atributos y métodos
- Una clase debe tener una única responsabilidad
- Inicializar atributos en el constructor
- Usar `this` para referirse a atributos de la instancia

## 18. Resumen del módulo
- **Clase:** plantilla que define atributos y métodos
- **Objeto:** instancia concreta de una clase, creada con `new`
- **Atributos:** variables que representan el estado del objeto
- **Métodos:** funciones que definen el comportamiento del objeto
- **Constructor:** método especial que inicializa el objeto
- **Encapsulamiento:** ocultar los datos usando `private`
- **Getter:** método público que devuelve el valor de un atributo privado
- **Setter:** método público que modifica el valor de un atributo privado
- **`this`:** referencia al objeto actual dentro de la clase

## 19. Actividad práctica
- Enunciado: Crear una clase `CuentaBancaria` con los siguientes requisitos
- **Atributos privados:**
  - `numeroCuenta` (String)
  - `saldo` (double)
  - `titular` (String)
- **Constructores:**
  - Constructor que reciba número de cuenta, titular y saldo inicial
- **Getters y setters:**
  - Getter para `saldo`
  - Getter y setter para `titular`
  - Solo getter para `numeroCuenta` (no debe modificarse después de creado)
- **Métodos de negocio:**
  - `depositar(double monto)` → aumenta el saldo si el monto es positivo
  - `retirar(double monto)` → disminuye el saldo si hay fondos suficientes
  - `mostrarInformacion()` → muestra todos los datos de la cuenta
- **Desde `main`:**
  - Crear dos objetos `CuentaBancaria`
  - Realizar depósitos y retiros
  - Mostrar la información después de cada operación
- Ampliación opcional 1: Agregar método `transferir(CuentaBancaria destino, double monto)`
- Ampliación opcional 2: Validar que el número de cuenta tenga un formato específico (ej: 10 dígitos)
- Ampliación opcional 3: Crear un array de cuentas y un menú para operar sobre ellas
