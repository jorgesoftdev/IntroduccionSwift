# Enum

Los enum en Swift son una manera de definir un tipo de dato propio que representa un conjunto limitado de valores posibles. Son particularmente útiles para crear una serie de opciones predefinidas y relacionadas que un valor puede tener.

Un ejemplo practico de estos es: 
```swift
enum EstadoDeConexion {
    case desconectado
    case conectado(red: String)
    case conectadoSinRed
}

var estadoActual = EstadoDeConexion.conectado(red: "Wi-Fi")

switch estadoActual {
case .desconectado:
    print("No hay conexión")
case .conectado(let red):
    print("Conectado a la red: \(red)")
case .conectadoSinRed:
    print("Conectado sin red")
}
```

# Struct

Las estructuras (structs) en Swift son tipos de datos que te permiten agrupar propiedades y métodos relacionados en una única entidad. A diferencia de las clases, las estructuras son tipos de valor, lo que significa que se copian cuando se asignan o pasan como parámetros, en lugar de ser referenciadas como en el caso de las clases. 

Un ejemplo practico de esto seria el siguiente: 
```swift
struct Persona {
    var nombre: String
    var edad: Int
    
    func saludar() {
        print("¡Hola! Soy \(nombre) y tengo \(edad) años.")
    }
}

var persona1 = Persona(nombre: "Ana", edad: 30)
persona1.saludar()
```

# Sets

En Swift, un Set es una colección no ordenada de valores únicos del mismo tipo. Esto significa que un Set no permite elementos duplicados y no garantiza ningún orden específico para sus elementos. Los Sets son una herramienta útil cuando necesitas almacenar valores únicos sin importar su orden.

```swift
var numerosPares: Set<Int> = [2, 4, 6, 8, 10]
numerosPares.insert(12)
numerosPares.insert(6) // No se insertará porque ya está en el Set

if numerosPares.contains(8) {
    print("El conjunto contiene el número 8.")
}

var numerosImpares: Set<Int> = [1, 3, 5, 7, 9]

let numerosComunes = numerosPares.intersection(numerosImpares) // Intersección
let todosLosNumeros = numerosPares.union(numerosImpares) // Unión

print(numerosComunes) // Imprimirá los números comunes entre los Sets
print(todosLosNumeros) // Imprimirá todos los números sin duplicados
```
