# Operadores Aritméticos en Swift

En Swift, los operadores aritméticos son símbolos que se utilizan para realizar operaciones matemáticas en números. A continuación, se presentan los operadores aritméticos básicos en Swift junto con ejemplos de cómo usarlos:

1. **Suma (+):** Se utiliza para sumar dos valores.
```swift
let suma = 5 + 3 // Resultado: 8
let a = 2
let b = 3
let c = a + b
print(c) // Resultado: 5
```
2. **Resta (-):** Se utiliza para restar dos valores.
```swift
let resta = 10 - 4 // Resultado: 6
let x = 8
let y = 3
let z = x - y
print(z) // Resultado: 5
```
3. **Multiplicacion (*):** Se utiliza para multiplicar dos valores.
```swift
let multiplicacion = 3 * 7 // Resultado: 21
let multi = 3 * 3 // Resultado: 9
```
4. **Division (/):** Se utiliza para dividir dos valores
```swift
let division = 15 / 3 // Resultado: 5
let div = 16 / 4 // Resultado: 4
```
5. **Modulo (%):** También conocido como operador de resto, devuelve el residuo de la división entre dos valores
```swift
let modulo = 17 % 5 // Resultado: 2
```
6. **Operadores compuestos:** Son una combinación de un operador aritmético y un operador de asignación.
```swift
var valor = 10
valor += 5 // Equivalente a valor = valor + 5
valor *= 2 // Equivalente a valor = valor * 2
```
7. **Operador potencia:** Calcula la potencia de n de un numero
```swift
let potencia = 2 ** 3 // Resultado: 8
```
# Operadores logicos en swift

Los operadores lógicos se utilizan para combinar o evaluar expresiones booleanas, mientras que los operadores de comparación se utilizan para comparar valores y obtener un resultado booleano.

1. **AND Lógico (&&):** Devuelve true si ambas expresiones son verdaderas.

```swift
let a = true
let b = false
let result = a && b // Resultado: false
```
2. **OR Lógico (| |):** Devuelve true si al menos una de las expresiones es verdadera.

```swift
let x = true
let y = false
let resultado = x || y // Resultado: true
```
3. **NOT Lógico (!):** Niega el valor de la expresión, convirtiendo true en false y viceversa.

```swift
let condicion = true
let negacion = !condicion // Resultado: false
```
# Operadores de comparación

Los operadores de comparación se utilizan para evaluar si dos valores son iguales o son distintos entre si.

1. **Igual (==):** Comprueba si dos valores son iguales.
```swift
let num1 = 5
let num2 = 5
let igualdad = num1 == num2 // Resultado: true
```
2. **Diferente (!=):** Comprueba si dos valores son diferentes.
```swift
let val1 = "hola"
let val2 = "mundo"
let esDiferente = val1 != val2 // Resultado: true
```
3. **Mayor que (>):** Comprueba si el primer valor es mayor que el segundo.
```swift
let a = 10
let b = 5
let esMayor = a > b // Resultado: true
```
4. **Menor que (<):** Comprueba si el primer valor es menor que el segundo.
```swift
let x = 3.14
let y = 4.0
let esMenor = x < y // Resultado: true
```
5. **Mayor o igual que (>=):** Comprueba si el primer valor es mayor o igual que el segundo.
```swift
let valor1 = 8
let valor2 = 8
let esMayorIgual = value1 >= value2 // Resultado: true
```
6. **Mayor o igual que (<=):** Comprueba si el primer valor es menor o igual que el segundo.
```swift
let m = 20
let n = 25
let esMenorIgual = m <= n // Resultado: true
```
