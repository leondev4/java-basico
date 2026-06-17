---

markmap:
  initialExpandLevel: 1
---

# **Módulo 8 – Proyecto integrador**

## 1. Proyecto integrador
- Mini sistema de gestión de estudiantes

## 2. Objetivos del proyecto
- Aplicar todos los conceptos aprendidos durante el curso
- Implementar un sistema completo con menú interactivo
- Usar clases, arrays, métodos, condicionales y bucles
- Entregar un proyecto funcional y bien estructurado

## 3. Descripción del proyecto
- Mini sistema de gestión de estudiantes
- Funcionalidades obligatorias:
  - Agregar estudiantes
  - Listar todos los estudiantes
  - Buscar un estudiante por nombre
  - Calcular el promedio de calificaciones
  - Salir del programa

## 4. Requerimientos funcionales
- El programa muestra un menú con opciones numeradas
- El usuario elige una opción ingresando un número
- Después de cada acción, se vuelve a mostrar el menú
- El programa termina solo cuando el usuario elige "Salir"
- Los estudiantes se almacenan en un array o `ArrayList`

## 5. Clase Estudiante (atributos)
- ```
  public class Estudiante {
      private String nombre;
      private int edad;
      private double calificacion;
  }
  ```
- Todos los atributos deben ser `private`
- La edad debe ser positiva (mayor que 0)
- La calificación debe estar entre 0.0 y 10.0

## 6. Clase Estudiante (constructores)
- ```
  public Estudiante(String nombre, int edad, double calificacion) {
      this.nombre = nombre;
      this.edad = edad;
      this.calificacion = calificacion;
  }
  ```
- Constructor que recibe todos los atributos como parámetros
- Validar edad y calificación dentro del constructor o en setters

## 7. Clase Estudiante (getters y setters)
- ```
  public String getNombre() { return nombre; }
  public void setNombre(String nombre) { this.nombre = nombre; }
  
  public int getEdad() { return edad; }
  public void setEdad(int edad) {
      if (edad > 0) {
          this.edad = edad;
      }
  }
  
  public double getCalificacion() { return calificacion; }
  public void setCalificacion(double calificacion) {
      if (calificacion >= 0 && calificacion <= 10) {
          this.calificacion = calificacion;
      }
  }
  ```

## 8. Clase Estudiante (método mostrarInfo)
- ```
  public void mostrarInfo() {
      System.out.println("Nombre: " + nombre);
      System.out.println("Edad: " + edad);
      System.out.println("Calificación: " + calificacion);
  }
  ```
- También se puede sobrescribir el método `toString()`

## 9. Clase principal – menú de opciones
- ```
  public class SistemaEstudiantes {
      public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
          Estudiante[] estudiantes = new Estudiante[100];  // máximo 100 estudiantes
          int contador = 0;
          int opcion;
          
          do {
              mostrarMenu();
              opcion = sc.nextInt();
              sc.nextLine();  // limpiar buffer
              
              switch (opcion) {
                  case 1:
                      agregarEstudiante(sc, estudiantes, contador);
                      contador++;
                      break;
                  case 2:
                      listarEstudiantes(estudiantes, contador);
                      break;
                  case 3:
                      buscarEstudiante(sc, estudiantes, contador);
                      break;
                  case 4:
                      calcularPromedio(estudiantes, contador);
                      break;
                  case 5:
                      System.out.println("Saliendo del sistema...");
                      break;
                  default:
                      System.out.println("Opción no válida");
              }
          } while (opcion != 5);
      }
  }
  ```

## 10. Funcionalidad – mostrar menú
- ```
  public static void mostrarMenu() {
      System.out.println("\n=== SISTEMA DE GESTIÓN DE ESTUDIANTES ===");
      System.out.println("1. Agregar estudiante");
      System.out.println("2. Listar estudiantes");
      System.out.println("3. Buscar estudiante por nombre");
      System.out.println("4. Calcular promedio de calificaciones");
      System.out.println("5. Salir");
      System.out.print("Seleccione una opción: ");
  }
  ```

## 11. Funcionalidad – agregar estudiante
- ```
  public static void agregarEstudiante(Scanner sc, Estudiante[] estudiantes, int contador) {
      System.out.print("Ingrese el nombre: ");
      String nombre = sc.nextLine();
      
      System.out.print("Ingrese la edad: ");
      int edad = sc.nextInt();
      
      System.out.print("Ingrese la calificación (0-10): ");
      double calificacion = sc.nextDouble();
      sc.nextLine();  // limpiar buffer
      
      estudiantes[contador] = new Estudiante(nombre, edad, calificacion);
      System.out.println("Estudiante agregado exitosamente");
  }
  ```

## 12. Funcionalidad – listar estudiantes
- ```
  public static void listarEstudiantes(Estudiante[] estudiantes, int contador) {
      if (contador == 0) {
          System.out.println("No hay estudiantes registrados");
          return;
      }
      
      System.out.println("\n=== LISTA DE ESTUDIANTES ===");
      for (int i = 0; i < contador; i++) {
          System.out.println("\n--- Estudiante " + (i + 1) + " ---");
          estudiantes[i].mostrarInfo();
      }
  }
  ```

## 13. Funcionalidad – buscar estudiante por nombre
- ```
  public static void buscarEstudiante(Scanner sc, Estudiante[] estudiantes, int contador) {
      if (contador == 0) {
          System.out.println("No hay estudiantes registrados");
          return;
      }
      
      System.out.print("Ingrese el nombre a buscar: ");
      String nombreBuscado = sc.nextLine();
      boolean encontrado = false;
      
      for (int i = 0; i < contador; i++) {
          if (estudiantes[i].getNombre().equalsIgnoreCase(nombreBuscado)) {
              System.out.println("\nEstudiante encontrado:");
              estudiantes[i].mostrarInfo();
              encontrado = true;
          }
      }
      
      if (!encontrado) {
          System.out.println("No se encontró ningún estudiante con ese nombre");
      }
  }
  ```

## 14. Funcionalidad – calcular promedio de calificaciones
- ```
  public static void calcularPromedio(Estudiante[] estudiantes, int contador) {
      if (contador == 0) {
          System.out.println("No hay estudiantes registrados para calcular promedio");
          return;
      }
      
      double suma = 0;
      for (int i = 0; i < contador; i++) {
          suma += estudiantes[i].getCalificacion();
      }
      
      double promedio = suma / contador;
      System.out.printf("El promedio de calificaciones es: %.2f\n", promedio);
  }
  ```

## 15. Versión con ArrayList (recomendada)
- Usar `ArrayList` en lugar de array fijo para mayor flexibilidad
- ```
  import java.util.ArrayList;
  ArrayList<Estudiante> estudiantes = new ArrayList<>();
  ```
- Agregar: `estudiantes.add(nuevoEstudiante);`
- Listar: `for (Estudiante e : estudiantes) { e.mostrarInfo(); }`
- Buscar: recorrer el `ArrayList` con for-each
- Promedio: recorrer el `ArrayList` sumando calificaciones

## 16. Resumen del módulo
- **Proyecto final:** Mini sistema de gestión de estudiantes
- **Clase Estudiante:**
  - Atributos privados: `nombre`, `edad`, `calificacion`
  - Constructor para inicializar
  - Getters y setters con validaciones
  - Método `mostrarInfo()`
- **Clase principal:**
  - Menú con opciones (do-while + switch)
  - Array o `ArrayList` para almacenar estudiantes
  - Métodos separados para cada funcionalidad
- **Funcionalidades:**
  - Agregar estudiante
  - Listar todos los estudiantes
  - Buscar por nombre (con `equalsIgnoreCase`)
  - Calcular promedio de calificaciones
- **Validaciones importantes:**
  - Edad debe ser positiva
  - Calificación entre 0 y 10
  - Verificar que haya estudiantes antes de listar o promediar

## 17. Actividad práctica (proyecto final)
- **Entregables:**
  - Código fuente completo (archivos .java)
  - Capturas de pantalla de la ejecución de cada funcionalidad
  - Respuesta a preguntas de opción múltiple sobre el proyecto
- **Criterios de evaluación:**
  - Clase Estudiante correcta (atributos privados, constructor, getters/setters) → 2 puntos
  - Funcionalidad agregar estudiante → 2 puntos
  - Funcionalidad listar estudiantes → 1 punto
  - Funcionalidad buscar estudiante → 2 puntos
  - Funcionalidad calcular promedio → 1 punto
  - Menú y flujo principal → 1 punto
  - Código limpio y organizado → 1 punto
- **Forma de entrega:** GitHub / ZIP / PDF (según indicación del instructor)
- **Ampliación opcional 1:** Usar `ArrayList` en lugar de array fijo
- **Ampliación opcional 2:** Agregar funcionalidad para eliminar estudiante
- **Ampliación opcional 3:** Agregar funcionalidad para ordenar estudiantes por calificación
- **Ampliación opcional 4:** Guardar y cargar estudiantes desde un archivo
- **Ampliación opcional 5:** Agregar validación para no superar el límite del array

## 18. Cierre del curso
- Felicitaciones por llegar al final del curso
- Has aprendido desde variables hasta POO y un proyecto completo
- Próximos pasos sugeridos:
  - `ArrayList` y colecciones (List, Set, Map)
  - Herencia y polimorfismo
  - Manejo de excepciones con try-catch
  - Archivos (lectura/escritura con FileWriter y BufferedReader)
  - Interfaces gráficas con Swing o JavaFX
  - Conexión a bases de datos con JDBC
- ¡Sigue practicando!


**¡Hemos completado los 8 módulos del curso!** 

¿Necesitas que ajuste algún módulo o que genere algún material adicional (ejercicios de completar, relacionar u opción múltiple)?