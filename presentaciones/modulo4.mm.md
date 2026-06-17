---

markmap:
  initialExpandLevel: 1
---


# **Módulo 4 – Bucles**

##  Bucles
- Repitiendo bloques de código

## 2. Objetivos del módulo
- Usar `for` para iteraciones con número fijo de repeticiones
- Usar `while` para iteraciones con condición al inicio
- Usar `do-while` para iteraciones con condición al final
- Emplear `break` y `continue` para control de flujo

## 3. Concepto de bucle o iteración
- Un bucle repite un bloque de código varias veces
- Evita escribir el mismo código muchas veces
- Tipos: `for`, `while`, `do-while`
- Control: variable contador o condición de parada

## 4. Bucle for (sintaxis y partes)
- ```
  for (inicialización; condición; incremento) {
      // Código a repetir
  }
  ```
- Inicialización: se ejecuta una vez al inicio
- Condición: se evalúa antes de cada iteración (si es `false`, termina)
- Incremento: se ejecuta al final de cada iteración

## 5. Diagrama de flujo del for
- Inicialización → Evaluar condición → True → Ejecutar bloque → Incremento → Volver a evaluar
- False → Salir del bucle

## 6. Ejemplos de for
- Ascendente: `for (int i = 0; i < 10; i++)` → 0,1,2,3,4,5,6,7,8,9
- Descendente: `for (int i = 10; i > 0; i--)` → 10,9,8,7,6,5,4,3,2,1
- Paso personalizado: `for (int i = 0; i <= 20; i += 2)` → 0,2,4,6,8,10,12,14,16,18,20

## 7. Bucle while (sintaxis)
- ```
  while (condición) {
      // Código a repetir
  }
  ```
- La condición se evalúa antes de cada iteración
- Si la condición es `false` al inicio, el bloque no se ejecuta nunca

## 8. Diagrama de flujo del while
- Evaluar condición → True → Ejecutar bloque → Volver a evaluar
- False → Salir del bucle

## 9. Ejemplo de while
- ```
  int i = 0;
  while (i < 5) {
      System.out.println(i);
      i++;
  }
  ```
- Imprime: 0,1,2,3,4

## 10. Comparación for vs while
- for:
  - Número fijo de iteraciones
  - Inicialización, condición e incremento juntos
  - Ejemplo: recorrer un array
- while:
  - Número variable de iteraciones
  - Inicialización, condición e incremento separados
  - Ejemplo: leer hasta que el usuario ingrese 0

## 11. Bucle do-while (sintaxis)
- ```
  do {
      // Código a repetir
  } while (condición);
  ```
- La condición se evalúa al final
- El bloque se ejecuta al menos una vez

## 12. Diagrama de flujo del do-while
- Ejecutar bloque → Evaluar condición → True → Volver a ejecutar bloque
- False → Salir del bucle

## 13. Ejemplo de do-while
- ```
  int i = 0;
  do {
      System.out.println(i);
      i++;
  } while (i < 5);
  ```
- Imprime: 0,1,2,3,4
- Si `i = 10` al inicio, imprime 10 una sola vez

## 14. Diferencia entre while y do-while
- while:
  - 0 o más iteraciones
  - Evalúa al inicio
  - Puede no ejecutarse nunca
- do-while:
  - 1 o más iteraciones
  - Evalúa al final
  - Siempre se ejecuta al menos una vez

## 15. Sentencias break y continue
- `break`: termina inmediatamente el bucle (sale de él)
- `continue`: salta a la siguiente iteración (no ejecuta el resto del bloque)
- ```
  for (int i = 0; i < 10; i++) {
      if (i == 5) break;      // termina cuando i llega a 5
      if (i % 2 == 0) continue; // salta los números pares
      System.out.println(i);  // solo impares antes del 5: 1,3
  }
  ```

## 16. Bucles anidados
- Un bucle dentro de otro bucle
- Útil para trabajar con matrices, tablas, pirámides
- El bucle interno se ejecuta completamente por cada iteración del externo
- ```
  for (int i = 1; i <= 3; i++) {
      for (int j = 1; j <= 3; j++) {
          System.out.println(i + " x " + j + " = " + (i * j));
      }
  }
  ```

## 17. Errores comunes con bucles
- Bucle infinito: olvidar actualizar la variable de control
  - `while (true) { }` → nunca termina
  - `for (int i = 0; i < 10; i--) { }` → nunca llega a 10
- Índice fuera de rango en arrays
- Usar `=` en lugar de `==` en la condición
- Olvidar las llaves `{}` para más de una línea

## 18. Buenas prácticas con bucles
- Asegurar que la condición eventualmente sea `false`
- Usar nombres descriptivos para las variables contador (`i`, `j`, `contador`)
- Evitar modificar la variable de control dentro del bloque del bucle
- Preferir `for` cuando se conoce el número exacto de iteraciones
- Preferir `while` cuando se desconoce el número de iteraciones

## 19. Resumen del módulo
- `for` → iteraciones con número fijo conocido
  - Sintaxis: `for (inicialización; condición; incremento) { }`
- `while` → iteración con condición al inicio (0 o más veces)
  - Sintaxis: `while (condición) { }`
- `do-while` → iteración con condición al final (1 o más veces)
  - Sintaxis: `do { } while (condición);`
- `break` → sale inmediatamente del bucle
- `continue` → salta a la siguiente iteración
- Bucles anidados → un bucle dentro de otro bucle

## 20. Actividad práctica
- Enunciado: Crear un programa que imprima la tabla de multiplicar de un número ingresado por el usuario
- Tipo a usar: `int` para el número y para el contador
- Estructura a usar: `for`
- Mostrar: la tabla del 1 al 10 usando `System.out.println`
- Ejecutar: probar en el IDE con diferentes valores
- Ejemplo de entrada: `número = 7`
- Ejemplo de salida esperada:
  - `7 x 1 = 7`
  - `7 x 2 = 14`
  - `7 x 3 = 21`
  - `7 x 4 = 28`
  - `7 x 5 = 35`
  - `7 x 6 = 42`
  - `7 x 7 = 49`
  - `7 x 8 = 56`
  - `7 x 9 = 63`
  - `7 x 10 = 70`
- Ampliación opcional 1: Pedir números al usuario hasta que ingrese 0 y mostrar la suma total (usar `while`)
- Ampliación opcional 2: Imprimir una pirámide de asteriscos con `for` anidados

