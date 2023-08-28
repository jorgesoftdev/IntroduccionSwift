# Tipos de Datos en Swift

En Swift, los tipos de datos son fundamentales para almacenar y manipular valores en un programa. A continuación se presentan algunos tipos de datos básicos en Swift, junto con ejemplos para cada uno:

## 1. Enteros

Representan números enteros, ya sean positivos o negativos.

Ejemplos:
```swift
let edad = 30
let cantidad = -5
let poblacion = 1000000
let distancia = 250
```
## 2. Números de Punto Flotante 

Representan números con decimales.

Ejemplos:
```swift
let pi = 3.14159
let gravedad = 9.81
let temperatura = -5.5
let pecio = 19.99
```
## 3. Booleanos

Representan valores verdadero o falso.

Ejemplos:
```swift
let estaSoleado = true
let tienePermiso = false
let estaRegistrado = true
let luzPrendida = false
```

## 4. Cadenas 

Representan secuencias de caracteres.

Ejemplos:
```swift
let saludo = "Hola, mundo"
let nombre = "Juan"
let direccion = "123 Calle Principal"
let bienvenida = "¡Bienvenidos a Swift!"
```
Inteerpolacion de cadenas: La interpolación de cadenas te permite insertar valores dentro de una cadena utilizando la sintaxis \(valor).

```swift
let nombre = "Juan"
let edad = 25
let mensaje = "Hola, mi nombre es \(nombre) y tengo \(edad) años."
print(mensaje) // Salida: "Hola, mi nombre es Juan y tengo 25 años."
```
Cadenas multilinea: Las cadenas multilínea te permiten crear cadenas que abarcan varias líneas de código sin la necesidad de escapar caracteres especiales.
```swift
let poema = """
Las rosas son rojas,
El mar es azul,
La azucar es dulce,
Y asi eres tu.
"""
print(poema)
```

## 5. Caracteres 
Representan un solo carácter.

Ejemplos:
```swift
let inicial = "J"
let genero = "M"
let grupo = "A"
let simbolo = "@"
```
## 6. Tuplas 

Permiten agrupar múltiples valores en una sola entidad.

Ejemplos:
```swift
let coordenadas: (Double, Double) = (latitud: 40.7128, altitud: -74.0060)
let persona: (String, Int) = (nombre: "Alicia", edad: 28)
let punto: (Int, Int) = (x: 10, y: 20)
let medidas: (Double, String) = (distancia: 3.5, unidad: "metros")
```
## 7. Arreglos

Representan colecciones ordenadas de elementos del mismo tipo.

Ejemplos:
```swift
let numeros: [Int] = [1, 2, 3, 4, 5]
let colores: [String] = ["Rojo", "Verde", "Azul"]
let temperaturas: [Double] = [25.5, 30.2, 18.7]
let edades: [Int] = [18, 25, 40, 32]
```
## 8. Diccionarios 

Representan colecciones no ordenadas de pares clave-valor.

Ejemplos:
```swift
let puntiaciones: [String: Int] = ["Alicia": 95, "Bob": 80, "Eve": 72]
let coordemadas: [String: Double] = ["latitud": 37.7749, "longitud": -122.4194]
let informacion: [String: Any] = ["nombre": "Jorge", "edad": 24]
```

## 9. Opcionales 

Permiten representar la posibilidad de que un valor no exista.

Ejemplos:
```swift
let usuario: String?
let temperatura: Double?
let numero: Int?
let direccion: String?
```
[<< Anterior](../ReglasNombreDeVariables) | [Siguiente >>](../TipadoExplicito)
