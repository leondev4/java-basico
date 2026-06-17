---

markmap:
  initialExpandLevel: 1
---

# **Módulo 3 – Estructuras condicionales**

## 1. Estructuras condicionales
- Tomando decisiones en el código

## 2. Objetivos del módulo
- Usar `if`, `else if` y `else` para decisiones simples y múltiples
- Implementar `switch` para múltiples opciones
- Emplear el operador ternario para asignaciones condicionales

## 3. Estructura if simple
- ```
  if (condición) {
      // Código que se ejecuta si la condición es true
  }
  ```
- La condición debe ser una expresión booleana
- Si la condición es `false`, el bloque se omite

## 4. Diagrama de flujo del if
- Inicio → Evaluar condición → Verdadero → Ejecutar bloque → Fin
- Falso → Saltar bloque → Fin

## 5. Estructura if-else
- ```
  if (condición) {
      // Código si es true
  } else {
      // Código si es false
  }
  ```
- Un bloque se ejecuta siempre
- Nunca se ejecutan ambos

## 6. Diagrama de flujo del if-else
- Inicio → Evaluar condición → Verdadero → Bloque A → Fin
- Falso → Bloque B → Fin

## 7. Estructura else if múltiple
- ```
  if (condición1) {
      // bloque 1
  } else if (condición2) {
      // bloque 2
  } else if (condición3) {
      // bloque 3
  } else {
      // bloque por defecto
  }
  ```
- Se evalúa en orden
- Solo se ejecuta el primer bloque cuya condición sea true

## 8. Ejemplo de else if múltiple
- ```
  int nota = 85;
  if (nota >= 90) {
      System.out.println("A");
  } else if (nota >= 80) {
      System.out.println("B");
  } else if (nota >= 70) {
      System.out.println("C");
  } else {
      System.out.println("Reprobado");
  }
  ```
- En este ejemplo, con nota 85, se imprime "B"

## 9. Estructura switch
- ```
  switch (variable) {
      case valor1:
          // código
          break;
      case valor2:
          // código
          break;
      default:
          // código por defecto
  }
  ```
- Funciona con: `int`, `char`, `String`, `enum`
- `break` evita la caída a los siguientes casos

## 10. Ejemplo de switch
- ```
  int dia = 3;
  switch (dia) {
      case 1:
          System.out.println("Lunes");
          break;
      case 2:
          System.out.println("Martes");
          break;
      case 3:
          System.out.println("Miércoles");
          break;
      default:
          System.out.println("Día no válido");
  }
  ```
- En este ejemplo, con dia = 3, se imprime "Miércoles"

## 11. Comparación entre if-else y switch
- if-else:
  - Cualquier expresión booleana
  - Permite rangos (ej: `nota >= 90`)
  - Mejor para 2-3 opciones
- switch:
  - Solo igualdad (ej: `dia == 3`)
  - Valores concretos (no rangos)
  - Mejor para muchas opciones con valores fijos

## 12. Cuándo usar cada estructura
- if-else: rangos, operadores lógicos, 2-3 opciones
- switch: muchas opciones con valores fijos (menú, días de semana, meses)
- Operador ternario: asignaciones simples de dos vías

## 13. Operador ternario
- Sintaxis: `variable = (condición) ? valorTrue : valorFalse;`
- ```
  int mayor = (a > b) ? a : b;
  // Equivalente a:
  if (a > b) {
      mayor = a;
  } else {
      mayor = b;
  }
  ```

## 14. Switch con String (Java 7+)
- ```
  String color = "rojo";
  switch (color) {
      case "rojo":
          System.out.println("Alto");
          break;
      case "amarillo":
          System.out.println("Precaución");
          break;
      case "verde":
          System.out.println("Siga");
          break;
      default:
          System.out.println("Color no válido");
  }
  ```

## 15. Buenas prácticas en condicionales
- Usar llaves `{}` siempre, incluso para una línea
- Evitar anidamientos muy profundos (más de 3 niveles)
- Colocar la condición más probable primero
- Usar `switch` cuando haya más de 3 valores fijos
- Siempre incluir `break` en cada `case` del `switch`
- Incluir `default` en `switch` para manejar casos no contemplados

## 16. Resumen del módulo
- `if` → decisión simple (opcional)
- `if-else` → decisión binaria (dos opciones)
- `else if` → múltiples opciones excluyentes
- `switch` → selección por valores fijos concretos
- Operador ternario → `(condición) ? valorTrue : valorFalse`
- `break` en `switch` → evita la caída a los siguientes casos
- `default` en `switch` → caso por defecto cuando ningún `case` coincide
- Comparación: `if-else` permite rangos, `switch` solo igualdad

## 17. Actividad práctica
- Enunciado: Crear un programa que lea un número del 1 al 7 y muestre el día de la semana correspondiente
- Tipo a usar: `int` para el número
- Estructura a usar: `switch`
- Mostrar: el nombre del día usando `System.out.println`
- Validar: si el número está fuera del rango 1-7, mostrar "Día no válido"
- Ejecutar: probar en el IDE con diferentes valores
- Ejemplo de entrada: `número = 5`
- Ejemplo de salida esperada: `Viernes`
- Ampliación opcional 1: Modificar el programa para usar `if-else` en lugar de `switch`
- Ampliación opcional 2: Leer una nota (0-100) y mostrar la calificación en letra usando `if-else` (A: 90-100, B: 80-89, C: 70-79, D: 60-69, F: 0-59)


