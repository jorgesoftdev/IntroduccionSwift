# Bucles
Son estructuras fundamentales en la programación que se utilizan para ejecutar un bloque de código repetidamente. Estas estructuras son esenciales para automatizar tareas repetitivas y para procesar colecciones de datos de manera eficiente. 

## For
Se utiliza comúnmente para iterar sobre una secuencia de valores, como un rango de números, y realizar una acción en cada iteración.

Su sintaxis en swift es la siguiente:
```swift
for variable in rango {
    // Código a ejecutar en cada iteración
}
```
Por ejemplo imprimir una secuencia de numeros: 
```swift
for i in 1 ... 10 {
    print (i)
}
```

Para crear la tabla de multiplicar de un numero: 
```swift
let numero = 9
for i in 1 ... 9 {
    print(" \(i) x \(numero) = \(i*numero)")
}
```

### for anidado
Un ciclo for dentro de otro for
```swift
for i in 1...5 {
    for j in 1...10 {
        let resultado = i * j
        print("\(i) x \(j) = \(resultado)")
    }
    print("--------------------")
}
```
### for con incrementos/decrementos personalizados
Los valores de inicio y fin del for tradicional pero con un incremento diferente a 1
```swift
//               inicio   fin    incremento/decremento
for i in stride(from: 10, to: 0, by: -2) {
    print(i)
}
```
## While 

El bucle while en Swift es una estructura de control que permite ejecutar un bloque de código repetidamente mientras una determinada condición sea verdadera. A diferencia del bucle for, que se utiliza para un número específico de iteraciones, el bucle while se utiliza cuando el número de iteraciones no es conocido de antemano y depende de la evaluación continua de una condición.

La sintaxis es: 
```swift
while condicion {
    // Código a ejecutar mientras la condición sea verdadera
}
```
Un ejemplo es:
```swift
var contador = 0
while contador < 5 {
    print("El contador es \(contador)")
    contador += 1 // HACER QUE LA CONDICION SE CUMPLA EN ALGUN PUNTO
}
```

## Repeat

La estructura repeat en Swift es similar a la estructura while, pero a diferencia de while, la condición en repeat se evalúa después de ejecutar el bloque de código. Esto garantiza que el bloque de código se ejecute al menos una vez antes de verificar la condición.

Su sintaxis es la siguiente:
```swift
repeat {
    // Código a ejecutar al menos una vez
} while condicion
```
Un ejemplo comparado con el bucle while es el siguiente:
```swift
var contador = 0
repeat {
    print("El contador es \(contador)")
    contador += 1
} while contador < 5
```
[<< Anterior](../Condicionales) | [Siguiente >>](../Funciones)
