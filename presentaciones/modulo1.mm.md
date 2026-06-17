---

markmap:
  initialExpandLevel: 1
---
# **Módulo 1 – Fundamentos de programación y entorno Java**

## 🎯 1. Primeros pasos en Java

## 📌 2. Objetivos del módulo
- Comprender qué es un algoritmo y un programa
- Instalar el JDK y un IDE
- Conocer la estructura básica de un programa Java
- Usar `System.out.println` para mostrar información
- Declarar y usar variables con tipos primitivos

## 🧠 3. ¿Qué es un algoritmo?
- Secuencia ordenada de pasos para resolver un problema
- Ejemplo cotidiano: receta de cocina
- Características: preciso, finito, definido

## 📝 4. Ejemplo de algoritmo en pseudocódigo
- Problema: Calcular el área de un rectángulo
- Pasos del algoritmo:
  - 1. Inicio
  - 2. Leer base y altura
  - 3. Calcular área = base × altura
  - 4. Mostrar área
  - 5. Fin

## 💻 5. ¿Qué es un programa?
- Implementación de un algoritmo en un lenguaje de programación
- Lenguajes: Java, Python, C++
- Debe ser compilado o interpretado

## ☕ 6. Introducción a Java
- Creado por Sun Microsystems (1995), ahora Oracle
- Características:
  - Orientado a objetos
  - Independiente de plataforma (JVM)
  - Seguro y robusto
  - Amplia comunidad y bibliotecas

## 🔧 7. Instalación del JDK
- JDK = Java Development Kit
- Incluye: compilador (javac), JVM, bibliotecas
- Pasos de instalación:
  - Descargar de oracle.com o adoptium.net
  - Ejecutar el instalador
  - Configurar variable de entorno PATH
- Verificar: `java -version`

## 🛠️ 8. Instalación de un IDE
- IDE = Entorno de Desarrollo Integrado
- Opciones recomendadas:
  - IntelliJ IDEA (Community)
  - Eclipse
  - NetBeans
- Pasos: descargar, instalar, crear primer proyecto

## 🏗️ 9. Estructura de un programa Java
- Código base: `public class MiPrograma { // Código aquí }`
- El nombre de la clase debe coincidir con el archivo (.java)
- Las llaves `{}` delimitan bloques de código

## 🚀 10. El método main
- Código: `public static void main(String[] args) { // Punto de entrada }`
- Es obligatorio
- La JVM lo ejecuta al iniciar el programa

## 📢 11. Salida por consola
- `System.out.println("Hola mundo");` → Con salto de línea
- `System.out.print("Hola mundo");` → Sin salto de línea
- `System` es una clase, `out` es un objeto de salida, `println` e `print` son métodos

## 📦 12. Variables – concepto y sintaxis
- Espacio en memoria que almacena un valor
- Sintaxis: `tipo nombre = valor;`
- Ejemplo: `int edad = 25;`

## 🔢 13. Tipos primitivos
- `int`: 32 bits → `int num = 10;`
- `double`: 64 bits → `double pi = 3.14;`
- `char`: 16 bits → `char letra = 'A';`
- `boolean`: 1 bit → `boolean ok = true;`

## ✍️ 14. Declaración e inicialización
- `int edad;` → Declaración
- `edad = 30;` → Inicialización
- `double altura = 1.75;` → Declaración + inicialización
- `char inicial = 'J';`
- `boolean activo = false;`

## 📄 15. Ejemplo completo de programa básico
- ```
  public class MiPrograma { 
    public static void main(String[] args) { 
        String nombre = "Ana"; 
        int edad = 22; 
        double estatura = 1.65; 
        System.out.println("Nombre: " + nombre); 
        System.out.println("Edad: " + edad); 
        System.out.println("Estatura: " + estatura); 
        } 
    }

## 16. Resumen del módulo
- Algoritmo: secuencia de pasos para resolver un problema
- Programa: implementación de un algoritmo en un lenguaje
- JDK: kit de desarrollo de Java
- IDE: entorno integrado (IntelliJ, Eclipse, NetBeans)
- Estructura básica: clase + método main + llaves
- Salida: `System.out.println()` y `System.out.print()`
- Tipos primitivos: int, double, char, boolean
- Variables: espacio en memoria que almacena un valor

## 17. Actividad práctica
- Enunciado: Crear un programa que declare variables con tu edad, altura y letra inicial
- Tipos a usar: `int` para edad, `double` para altura, `char` para inicial
- Mostrar: cada valor por consola usando `System.out.println`
- Ejecutar: probar en el IDE
- Ejemplo de salida: `Edad: 25`, `Altura: 1.75`, `Inicial: J`
- Ampliación opcional: agregar nombre completo con `String` y mensaje personalizado