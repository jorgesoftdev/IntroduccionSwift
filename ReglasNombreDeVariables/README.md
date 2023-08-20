# Reglas para Nombrar Variables en Swift

En el lenguaje de programación Swift, el nombramiento de variables es una parte esencial de escribir un código limpio y comprensible. Aquí hay algunas reglas y pautas a seguir al nombrar variables en Swift:

1. **Empieza con una letra o un guión bajo:** Los nombres de variables deben comenzar con una letra (mayúscula o minúscula) o un guión bajo (_). No pueden comenzar con un número ni ningún otro carácter especial.

```swift
let 5istema = "MacOS" // Esto es un error
let Sistema = "MacOS" // Esto es correcto
var $dinero = 1000 // Esto es un error
var _dinero = 1000 // Esto es correcto
```
2. **Evita caracteres especiales:** Aunque se permite el uso de guiones bajos en los nombres de variables, evita el uso excesivo de caracteres especiales. El objetivo es crear nombres legibles y comprensibles.

```swift
var x^2 = 30 // Esto es un error
var x_cuadrada = 30 // Esto es correcto 
```

3. **Evita palabras reservadas:** No puedes usar palabras reservadas del lenguaje Swift como nombres de variables. Por ejemplo, no puedes nombrar una variable var.

```swift
var var = 15.1 // Esto es un error
var variable = 15.1 // Esto es correcto
var Int = 7 // Esto es un error
var entero = 7 // Esto es correcto
```

4. **Evita el uso de espacios:** No puedes usar espacios para nombrar variables porque ocurrira un error, mejor usa guiones bajos o formato Camel Case.
```swift
let nombre completo = "Alberto Besne" // Esto provocara un error
let nombre_completo = "Alberto Besne" // Esto es correcto
let nombreCompleto = "Alberto Besne" // Esto es correcto y usa el formato CamelCase
