# Constantes y Variables en Swift

En Swift, las variables juegan un papel fundamental en la programación, y se pueden clasificar en dos tipos principales: mutables e inmutables. Estos conceptos son importantes para comprender cómo se gestionan los datos en tu programa.

## Variables Mutables

Las variables mutables son aquellas cuyo valor puede cambiar después de su inicialización. En Swift, se definen utilizando la palabra clave `var`. Aquí hay un ejemplo de una variable mutable:

```swift
var edad = 25
edad = 26 // Se puede cambiar el valor
```
En este ejemplo, la variable edad se declara como mutable utilizando var. Luego, su valor se modifica de 25 a 26.

Algunos ejemplos de variables mutables son:

```swift
var altura = 1.80
var peso = 67
var distancia = 200
var ciudadResidencia = "CDMX"
var trabajo = "Maestro"
```

## Variables Inmutables

Las variables inmutables son aquellas cuyo valor no puede cambiar después de su inicialización. En Swift, se definen utilizando la palabra clave `let`. A continuación, se presenta un ejemplo de una variable inmutable:

```swift
let nombre = "Juan"
nombre = "Carlos" // Esto generará un error, ya que no se puede cambiar el valor
```
En este caso, la variable nombre se declara como inmutable utilizando let. Intentar cambiar su valor después de la inicialización generará un error en tiempo de compilación.

Algunos ejemplos de variables inmutables son:

```swift
let nombre = "Alberto"
let apellido = "Besne"
let curso = "Swift"
```
