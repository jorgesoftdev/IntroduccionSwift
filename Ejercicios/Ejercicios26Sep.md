1. Con las siguientes variables:
let numero1 = 7
let numero2 = 11
Realiza tres operaciones aritmeticas y tres operaciones de comparación. 
2. Declara un arreglo de enteros con mas de 5 elementos.
3. Encuentra el numero de elementos del arreglo.
4. Imprime el arreglo ordenado utilizando el metodo sorted()
5. Agrega dos elementos al arreglo
6. Elimina el tercer elemento del arreglo
7. Con las variables:
let a = 4
let b = 3
Si 'a' es mas grande que 'b' imprime un mensaje que diga "A es mas grande que B"
Utilizando If
8. En una variable declara tu edad y utilizando el operador ternario determina si eres mayor de 21 o no impreso en pantalla
9. Haz una estructura if, else if, else para cada variable siguiente donde se determine si un numero es positivo, negativo o es cero.
let num1 = 3
let num2 = -4
10. Declara la variable
let clima = "Soleado"
Y crea una estructura switch para para determinar si el clima es agradable con los casos:
case "Soleado" -> Es agradable
case "Nublado" -> No es agradable
case "Lloviendo" -> No es agradable

```swift
import UIKit

// Ejercicio 1

let numero1 : Double = 7
let numero2 : Double = 11

// Suma
let suma = numero1 + numero2
// Resta
let resta = numero1 - numero2
// Mulitiplicacion
let multi = numero1 * numero2
// Igualdad
let igual = numero1==numero2
// Mayor
let mayor =  numero1 > numero2
// Menor
let menor = numero1 < numero2


// Ejercicio 2
var arreglo : [Int] = [8,3,4,7,2,1]
// Ejercicio 3
let elementos = arreglo.count
// Ejercicio 4
print(arreglo.sorted())
// Ejercicio 5
arreglo.append(6)
arreglo.append(11)
// Ejercicio 6
arreglo.remove(at: 2)
print(arreglo)

// Ejercicio 7
let a = 4
let b = 3
if a > b {
    print("A es mayor que B")
}

// Ejercicio 8
let edad = 22
edad > 21 ? print("Soy mayor de 21") : print("Soy menor o tengo 21 ")

// Ejercicio 9
let num1 = 3
let num2 = -4
if num2 > 0 {
    print("El numero es positivo")
} else if num2 < 0 {
    print("El numero es negativo")
} else {
    print("El numero es 0")
}


// Ejercicio 10
let clima = "Solead"
switch clima {
case "Soleado":
    print("El clima es agradable")
case "Nublado", "Lloviendo":
    print("El clima esta feo")
default:
    print("Algo salio mal")
}

```

