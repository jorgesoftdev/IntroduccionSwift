## Funciones en Swift

En Swift, una función es un bloque de código reutilizable que realiza una tarea específica. Las funciones permiten agrupar un conjunto de instrucciones bajo un nombre y parámetros, lo que facilita la organización y modularización del código. Las funciones también pueden devolver un valor si es necesario.

La sintaxis básica de una función en Swift es la siguiente:

```swift
func nombreDeLaFuncion(parametro1: Tipo, parametro2: Tipo) -> TipoDeRetorno {
    // Cuerpo de la función
    // Puedes usar los parámetros para realizar tareas
    // Puedes devolver un valor utilizando la palabra clave "return"
}
```
Ejemplo:
```swift
func saludar(nombre: String) -> String {
    let mensaje = "Hola, \(nombre)!"
    return mensaje
}

let resultado = saludar(nombre: "Juan")
print(resultado) // Imprimirá "Hola, Juan!"
```
Tambien se pueden crear funciones sin parametros ni valores de retorno:

```swift
func imprimirMensaje() {
    let nombre: String = "Alberto" // variable local
    print("Hola \(nombre) desde la función")
}
imprimirMensaje() // Llama a la función y muestra "Hola desde la función"
```
Ejemplo de función para sumar dos valores: 
```swift
func sumar(a: Int, b: Int) -> Int {
    return a + b
}
let resultadoSuma = sumar(a: 5, b: 3)
print(resultadoSuma) // Imprimirá 8
```
[<< Anterior](../EstructurasDeRepeticion) | [Siguiente >>](../EnumyStruct)
