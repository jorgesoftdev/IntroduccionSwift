# Condicionales en Swift

Los condicionales son una parte fundamental en la programación, ya que permiten que un programa tome decisiones y realice diferentes acciones según las condiciones que se cumplan en un momento dado.

## If
El condicional "if" es una estructura fundamental en la programación que se utiliza para tomar decisiones y ejecutar ciertas partes de código solo si se cumple una determinada condición

Su sintaxis es la siguiente: 
```swift
if condicion {
    // Código a ejecutar si la condición es verdadera
}
```
Por ejemplo se puede utilizar para saber si un numero es positivo: 
```swift
let numero = 20
if ( numero > 0 ) {
    print ("El numero es positivo")
}
```
 
## Else

Acompaña al condicional "if" y permite ejecutar determinada instruccion si es que no se cumple una condicion

Su sintaxis es la siguiente: 
```swift
if condicion {
    // Código a ejecutar si la condición es verdadera
} else {
    // Código a ejecutar si la condición no es verdadera 
}
```
Acompañados del ejemplo anterior agregaremos una condicion para saber si el numero es positivo o es negativo:
```swift
let numero = 10

if numero > 0 {
    print("El número es positivo")
} else {
    print("El número es negativo")
}
```
## if anidados
Los condicionales "if" anidados se utilizan cuando deseas evaluar múltiples condiciones en diferentes niveles y realizar acciones basadas en esas condiciones. Esto te permite crear una estructura de decisiones más compleja en la que las acciones se toman en función de varias situaciones posibles

```swift
let temperatura = 25
if temperatura > 30 {
    print("Hace mucho calor.")
} else {
    if temperatura > 20 {
        print("El clima es agradable.")
    } else {
        print("Hace un poco de frío.")
    }
}
```

## else if
La declaración else if en Swift se utiliza para evaluar una condición alternativa si la condición anterior en una estructura if no se cumple. En otras palabras, permite manejar múltiples casos de manera secuencial, evaluando cada condición hasta que una de ellas sea verdadera o hasta que se llegue al bloque else final.
```swift
let temperatura = 25
if temperatura > 30 {
    print("Hace mucho calor.")
} else if temperatura > 20 {
    print("El clima es agradable.")
} else {
    print("Hace un poco de frío.")
}
```
## Operador ternario

El operador ternario, también conocido como operador condicional, es una forma concisa de expresar una decisión en una sola línea de código. Se utiliza para evaluar una condición y retornar un valor en función de si la condición es verdadera o falsa.

```swift
condicion ? valorSiVerdadero : valorSiFalso
```
Un ejemplo de su uso es:

```swift
let numero = 7
let resultado = numero > 5 ? "Es mayor que 5" : "No es mayor que 5"
print(resultado)
```

## Switch

El comando switch en Swift es una estructura de control que permite tomar decisiones basadas en el valor de una expresión. Se utiliza para comparar un valor con múltiples casos posibles y ejecutar un bloque de código correspondiente al caso que coincida con el valor evaluado. El switch es particularmente útil cuando tienes varias opciones diferentes para manejar diferentes valores.

```swift
switch valorAEvaluar {
case valor1:
    // Código a ejecutar si valorAEvaluar es igual a valor1
case valor2:
    // Código a ejecutar si valorAEvaluar es igual a valor2
// ...
default:
    // Código a ejecutar si no coincide con ningún caso anterior
}
```
Un ejemplo de su uso seria el siguiente:
```swift
let numero = 3
switch numero {
case 0:
    print("El número es cero")
case 1:
    print("El número es uno")
case 2, 3:
    print("El número es dos o tres")
default:
    print("El número es otro valor")
}
```
Tambien se puede usar con caracteres:
```swift
let caracter: Character = "a"
switch caracter {
case "a", "A":
    print("El caracter es 'a' o 'A'")
case "b", "B":
    print("El caracter es 'b' o 'B'")
default:
    print("El caracter no es 'a', 'A', 'b' ni 'B'")
}
```

[<< Anterior](../Arreglos) | [Siguiente >>](../EstructurasDeRepeticion)
