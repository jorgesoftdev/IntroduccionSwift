1. Imprime los numeros de 1 al 10 utilizando los ciclos for, while y repeat.
2. Imprime los SOLO los numeros pares del 1 al 20 utilizando el bucle for.
3. Utilizando el bucle for agrega los valores [ 2 , 4 , 6 , 8 , 10] al arreglo
```swift
var arreglo : [Int] = []
```
4. Impime una cuenta regresiva del 10 al 1 usando while
5. Crea una funcion que no reciba parametros llamada nombreCompleto que imprima tu nombre
6. Crea una funcion que reciba como parametros tu nombre y apellido e imprima "Hola soy nombre apellido"
7. Crea una funcion que reciba como paramatros la base y altura de un triangulo y regrese el area como valor de retorno
8. Crea una estructura llamada estudiante con todos sus atributos.
9. Crea un set con los numeros del 1 al 10
10. Revisa si el numero 7 esta en el set
11. Con las variables
```swift
let a : Set<Int> = [4, 5, 8, 9]
let b : Set<Int> = [3, 4, 5, 7]
```
a) Encuentra la union y la interseccion de a con b


```swift
import UIKit

//Ejercicio 1
// For
for i in 1...10{
    print(i)
}
// While
var j = 1
while j < 11 {
    print(j)
    j += 1
}
// repeat
var k = 1
repeat {
    print(k)
    k += 1
} while k<11




// Ejercicio 2
for par in stride(from: 2, to: 22, by: 2){
    print(par)
}



// Ejercicio 3
var arreglo : [Int] = []
for agregado in 1...10 {
    if agregado % 2 == 0 {
        arreglo.append(agregado)
    }
}
print(arreglo)


// Ejercicio 4
var regresiva = 10
while regresiva > 0 {
    print(regresiva)
    regresiva -= 1
}


/*
 Crea un set con los numeros del 1 al 10
 Elimina un elemento del set
 Con las variables
 */

// Ejercicio 5
func nombreCompleto(){
    print("Jorge Reyes")
}
nombreCompleto()
// Ejercicio 6
func nombreParametros(nombre: String,apellido: String){
    print("Hola soy \(nombre) \(apellido)")
}
nombreParametros(nombre: "Jorge", apellido: "Reyes")


// Ejercicio 7

func areaTriangulo(base: Double,altura: Double) -> Double {
    let areaTmp = base*altura
    return areaTmp/2
}
let area = areaTriangulo(base: 3, altura: 4)

// Ejercicio 8
struct Estudiante {
    var nombre : String
    var apellido : String
    var promedio : Double
    var numeroCuenta : String
    var carrera : String
    func pasarLista(){
        print("Presente soy \(nombre)")
    }
}
let yo = Estudiante(nombre: "Jorge", apellido: "Reyes", promedio: 9.9, numeroCuenta: "31832268", carrera: "MAC")
yo.pasarLista()

// Ejercicio 9

var miset : Set<Int> = [1,2,3,4,5,6,7,8,9,10]


// Ejercicio 10
if miset.contains(7){
    print("Verdadero")
}

// Ejercicio 11
let a : Set<Int> = [4, 5, 8, 9]
let b : Set<Int> = [3, 4, 5, 7]

let interseccion = a.intersection(b)
let union = a.union(b)
```
