---
layout: default
title: Practica C++
nav_order: 2
---
# Ejercicios para practicar C++

Resuelve los siguientes ejercicios para familiarizarte con C++.

Puedes usar el siguiente código como plantilla para los ejercicios.
```cpp
#include <iostream>

int main(int argc, char **argv) {
    std::cout << "Hola, mundo!\n";
    return 0;
}
```

Recuerda compilar y ejecutar con la siguiente secuencia de comandos.

> Linux/MacOs
> ```bash
> g++ miprograma.cpp -o miprograma.o
> ```

> Windows
> ```bash
> g++ miprograma.cpp -o miprograma.exe
> ```

También puedes ejecutar el programa de python **evaluar.py**, el cual, junto con el archivo **conf_eval.json** probará tus programas para saber si estan correctos. 

```bash
python evaluar.py
```

:warning: Cada ejercicio cuenta con un ejemplo, con la entrada y la salida esperada. Las palabras "Entrada:" y "Salida:" no deben imprimirse en la consola. Revisa bien que la salida sea escriba exactamente con el formato que el texto de ejemplo muestra, si no el programa evaluador lo marcará como fallido.

- :heavy_check_mark: Ejemplo:
     ```
     Entrada: 22
     Salida: Categoría: Adulto
     ```
- ✖️: Ejemplo:
    ```
    Entrada: Ingrese su edad: 22
    Salida: Categoría: Adulto
    ```
En ningún programa se requiere que imprima un mensaje para solicitar los valores de entrada. 

## **Ejemplo:** única entrada

1. **Dime tu edad:**
   - Descripción: Ingresa tu edad y muestrala en pantalla.
   - Nombre de archivo: edad.cpp
   - Ejemplo:
     
    ```
     Entrada: 22
     Salida: Tu edad es: 22.
    ```
    **Solución:**

    ```cpp
    #include <iostream>

    int main(int argc, char **argv) {
        int edad;
        std::cin >> edad;
        std::cout << "Tu edad es: "<< edad << ".";
        return 0;
    }
    ```

## **Ejemplo:** multiples entradas

1. **Fecha de nacimiento:**
   - Descripción: Ingresa tu edad y el año actual muetrala el año de nacimiento.
   - Nombre de archivo: nacimiento.cpp
   - Ejemplo:
     
    ```
     Entrada: 22, 2023
     Salida: Naciste en el 2001.
    ```
    **Solución:**

    ```cpp
    #include <iostream>

    int main(int argc, char **argv) {
        int edad;
        int anio_actual;
        std::cin >> edad;
        std::cin >> anio_actual;
        std::cout << "Naciste en el "<< (anio_actual-edad) << ".";
        return 0;
    }
    ```

> :warning: **Únicamente sube al repositorio los archivos fuente solicitados, aquellos que terminan en ".cpp".** 

> :warning: **No los coloques dentro de carpetas.**


# Condicionales IF
1. [ ] **Número Positivo/Negativo:**
   - Descripción: Determina si un número es positivo, negativo o cero.
   - Nombre de archivo: positivonegativo.cpp
   - Ejemplo:
     ```
     Entrada: 5
     Salida: El número 5 es positivo.
     Entrada: -3
     Salida: El número -3 es negativo.
     Entrada: 0
     Salida: El número 0 es cero.
     ```

2. [ ] **Número Par/Impar:**
   - Descripción: Verifica si un número es par o impar.
   - Nombre de archivo: parimpar.cpp
   - Ejemplo:
     ```
     Entrada: 10
     Salida: El número 10 es par.
     Entrada: 3
     Salida: El número 3 es impar.
     ```

3. [ ] **Comparación de Números:**
   - Descripción: Compara dos números y muestra cuál es mayor o si son iguales.
   - Nombre de archivo: comparanumeros.cpp
   - Ejemplo:
     ```
     Entrada: 7, 12
     Salida: El número 12 es mayor que 7.
     Entrada: 7, 12
     Salida: El número 12 es mayor que 7.
     ```

4. [ ] **Clasificación de Notas:**
   - Descripción: Convierte una calificación numérica en una clasificación (A, B, C, etc.).
   - Nombre de archivo: notas.cpp
   
   | Calificación | Valor | Notas                   |
   |--------------|-------|-------------------------|
   | A            | 10    | Sobresaliente           |
   | B            | 9 - 8 | Bien                    |
   | C            | 7 - 6 | Suficiente (Mínimo para aprobar) |
   | D            | 5 o menos     | Reprobado                |

   - Ejemplo:
     ```
     Entrada: 8.5
     Salida: Calificación: B
     ```

5. [ ] **Categorización de Edades:**
   - Descripción: Categoriza una edad en "niño", "adolescente" o "adulto".
   - Nombre de archivo: edades.cpp
   
   | Edad |  Categoria |
   |--------------|-------|
   | 0 - 12       | Niño    |
   | 12 - 20      | Adolescente |
   | 21 o más     | Adulto |

   - Ejemplo:
     ```
     Entrada: 22
     Salida: Categoría: Adulto
     ```

6. [ ] **Verificación de Contraseña:**
   - Descripción: Verifica si una contraseña ingresada es correcta.
   - Nombre de archivo: password.cpp
   - Ejemplo:
     ```
     Entrada: "clave123"
     Salida: Contraseña correcta.
     Entrada: "hackeado"
     Salida: Contraseña incorrecta.
     ```

7. [ ] **Divisibilidad:**
   - Descripción: Determina si un número es divisible por otro número.
   - Nombre de archivo: divisible.cpp
   - Ejemplo:
     ```
     Entrada: 15, 3
     Salida: 15 es divisible por 3.
     Entrada: 7, 5
     Salida: 7 no es divisible por 5.
     ```

8. [ ] **Categorización de Números:**
   - Descripción: Categoriza un número en "positivo", "negativo" o "cero", y luego en "pequeño" o no. "pequeño" es cuando el valor absoluto es menor que 10.
   - Nombre de archivo: categorizanumeros.cpp
   - Ejemplo:
     ```
     Entrada: -8
     Salida: El número -8 es negativo y es pequeño.
     Entrada: 12
     Salida: El número 12 es positivo y no es pequeño.
     ```

9. [ ] **Determinar Día de la Semana:**
   - Descripción: Asocia un número del 1 al 7 con un día de la semana.
   - Nombre de archivo: diasemana.cpp
   - Ejemplo:
     ```
     Entrada: 3
     Salida: El número 3 corresponde al miércoles.
     ```

10. [ ] **Año Bisiesto:**
    - Descripción: Verifica si un año es bisiesto o no.
    - Nombre de archivo: bisiesto.cpp
    - Ejemplo:
      ```
      Entrada: 2024
      Salida: El año 2024 es bisiesto.
      ```

# Ciclo FOR
11. [ ] **Suma de Números:**
      - Descripción: Calcula la suma de los números del 1 al `n`.
      - Nombre de archivo: sumafor.cpp
      - Ejemplo:
      ```
      Entrada: 5
      Salida: La suma de los números del 1 al 5 es 15.
      ```

12. [ ] **Tabla de Multiplicar:**
      - Descripción: Muestra la tabla de multiplicar de un número dado.
      - Nombre de archivo: tablafor.cpp
      - Ejemplo:
      ```
      Entrada: 7
      Salida: Tabla de multiplicar del 7:
      7 x 1 = 7
      7 x 2 = 14
      ...
      7 x 10 = 70
      ```
      > :warning: Revisa que cada línea impresa la termines con un salto de linea, incluso la final.

13. [ ] **Factorial:**
      - Descripción: Calcula el factorial de un número.
      - Nombre de archivo: factorialfor.cpp
      - Ejemplo:
      ```
      Entrada: 4
      Salida: El factorial de 4 es 24.
     ```

14. [ ] **Secuencia de Números Pares:**
      - Descripción: Genera los primeros `n` números pares.
      - Nombre de archivo: nparesfor.cpp
      - Ejemplo:
      ```
      Entrada: 6
      Salida: Los primeros 6 números pares son: 2, 4, 6, 8, 10, 12,
      ```
      > :warning: Observa que el símbolo final de la línea es una coma "," esto para que no agregues condiciones innecesarias para el ejercicio.

15. [ ] **Conteo Regresivo:**
      - Descripción: Realiza un conteo regresivo desde un número hasta 1.
      - Nombre de archivo: regresivofor.cpp
      - Ejemplo:
      ```
      Entrada: 9
      Salida: Conteo regresivo desde 9: 9, 8, 7, 6, 5, 4, 3, 2, 1,
      ```
      > :warning: Observa que el símbolo final de la línea es una coma "," esto para que no agregues condiciones innecesarias para el ejercicio.

# Ciclo While
16. [ ] **Contador Ascendente:**
      - Descripción: Usa un bucle `while` para contar desde 1 hasta un número dado por el usuario.
      - Nombre de archivo: contadorwhile.cpp
      - Ejemplo:
      ```
      Entrada: 5
      Salida: 1, 2, 3, 4, 5,
      ```
      > :warning: Observa que el símbolo final de la línea es una coma "," esto para que no agregues condiciones innecesarias para el ejercicio.


17. [ ] **Secuencia de Fibonacci:**
      - Descripción: Genera y muestra los primeros `n` términos de la secuencia de Fibonacci utilizando un bucle `while`.
      - Nombre de archivo: fibonacciwhile.cpp
      - Ejemplo:
      ```
      Entrada: 8
      Salida: Secuencia de Fibonacci: 0, 1, 1, 2, 3, 5, 8, 13,
      ```
      > :warning: Observa que el símbolo final de la línea es una coma "," esto para que no agregues condiciones innecesarias para el ejercicio.

18. [ ] **Suma de Números:**
      - Descripción: Solicita al usuario que ingrese números hasta que ingrese un valor negativo. Luego, calcula y muestra la suma de los números ingresados.
      - Nombre de archivo: sumanumeroswhile.cpp
      - Ejemplo:
      ```
      Entrada: 4, 7, 2, -1
      Salida: La suma de los números ingresados es 13.
      ```

19. [ ] **Tabla de Potencias:**
      - Descripción: Genera una tabla de potencias de 2 (2^0, 2^1, 2^2, ...) hasta que la potencia sea mayor que un valor dado por el usuario.
      - Nombre de archivo: potenciaswhile.cpp
      - Ejemplo:
      ```
      Entrada: 10
      Salida: 2^0 = 1
               2^1 = 2
               2^2 = 4
               2^3 = 8
      ```
      > :warning: Revisa que cada línea impresa la termines con un salto de linea, incluso la final.

20. [ ] **Contador Regresivo con Salto:**
      - Descripción: Solicita al usuario ingresar un número inicial y un tamaño de salto. Luego, realiza un conteo regresivo desde el número inicial hasta 1, utilizando el tamaño de salto especificado en cada iteración.
      - Nombre de archivo: regresivosaltowhile.cpp
      - Ejemplo:
      ```
      Entrada: Número inicial: 20, Tamaño del salto: 3
      Salida: 20, 17, 14, 11, 8, 5, 2,
      ```
      > :warning: Observa que el símbolo final de la línea es una coma "," esto para que no agregues condiciones innecesarias para el ejercicio.
