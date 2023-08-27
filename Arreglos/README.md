# Arreglos en Swift

Los arreglos son una estructura de datos fundamental en Swift y en la programación en general. Aquí hay algunas cosas importantes que debes saber sobre los arreglos en Swift:

1. **Definición de Arreglos:**
   - Un arreglo es una colección ordenada de elementos del mismo tipo.
   - Se define usando corchetes (`[]`) y separando los elementos por comas.
   
   ```swift
   var numeros: [Int] = [1, 2, 3, 4, 5]
   var nombres: [String] = ["Ana", "Juan", "María"]
   ```
2. **Acceso a Elementos:**
   -Los elementos en un arreglo se acceden mediante su índice, que comienza en 0.
   -Puedes acceder a un elemento usando la notación arreglo\[indice].

   ```swift
   let primerNumero = numeros[0] // primerNumero es 1
   let segundoNombre = nombres[1] // segundoNombre es "Juan"
   ```
3. **Modificación de Elementos:**
   -Puedes modificar un elemento en un arreglo asignando un nuevo valor al índice correspondiente.
   ```swift
   numeros[2] = 10 // Cambiar el tercer elemento a 10
   nombres[0] = "Ana María" // Cambiar el primer nombre
   ```
4. **Longitud de un Arreglo:**
   -La propiedad count de un arreglo devuelve la cantidad de elementos que contiene.
   ```swift
   let cantidadNombres = nombres.count // cantidadNombres es 3
   ```
5. **Agregar y Eliminar Elementos:**
   -Para agregar elementos al final de un arreglo, se utiliza el método append(_:).
   -Para eliminar elementos, se usan los métodos remove(at:) para eliminar por índice o removeLast() para eliminar el último elemento.
   ```swift
   numeros.append(6) // Agregar el número 6 al final
   nombres.remove(at: 1) // Eliminar el segundo nombre ("Juan")
   ```
6. **Iteración en Arreglos:**
   -Los bucles for-in son muy útiles para iterar sobre los elementos de un arreglo.
   -También puedes usar la función forEach para iterar y realizar una acción en cada elemento.
   ```swift
   for numero in numeros {
    print(numero)
   }
   nombres.forEach { nombre in
   print("Hola, \(nombre)!")
   }
   ```
7. **Ordenamiento:**
   -Puedes ordenar los elementos de un arreglo utilizando los métodos sorted() o sort().
   -sorted() devuelve un nuevo arreglo ordenado sin modificar el original, mientras que sort() ordena el arreglo original.
   ```swift
   var numerosDesordenados = [3, 1, 4, 2]
   let numerosOrdenados = numerosDesordenados.sorted() // Devuelve un nuevo arreglo ordenado
   numerosDesordenados.sort() // Ordena el arreglo original
   ```
