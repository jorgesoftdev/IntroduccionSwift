```swift
//
//  main.swift
//  CursoSwift
//
//  Created by Jorge on 28/08/23.
//

var flujoPrograma = true
var tareas: [Tarea] = []
var contadorTareas = 1
struct Tarea {
    let nombre : String
    let descripcion : String
    var status: String = "Pendiente"
    let id : Int
}
func agregaTarea (arreglo: inout [Tarea], identificador: Int){
    print ("Ingrese el nombre de la tarea: ")
    guard var nom = readLine()  else { return }
    print ("Ingrese la descripcion de la tarea")
    guard var des = readLine()  else { return }
    let nuevaTarea = Tarea (nombre: nom,descripcion: des, id: identificador)
    arreglo.append(nuevaTarea)
    
}
func imprimeTareas (arreglo: [Tarea]){
    print ("Muestra todas las tareas       ...... (1)")
    print ("Muestra las tareas pendientes  ...... (2)")
    print ("Muestra las tareas completadas ...... (3)")
    let tipoTarea = readLine()
    if tipoTarea == "1" {
        for tarea in arreglo {
            print (tarea.nombre)
            print (tarea.descripcion)
            print (tarea.status)
            print (tarea.id)
            print ("---------------------")
        }
    } else if tipoTarea == "2"{
        for tarea in arreglo {
            if tarea.status == "Pendiente" {
                print (tarea.nombre)
                print (tarea.descripcion)
                print (tarea.status)
                print (tarea.id)
                print ("---------------------")
            }
        }
    } else if tipoTarea == "3"{
        for tarea in arreglo {
            if tarea.status == "Completado" {
                print (tarea.nombre)
                print (tarea.descripcion)
                print (tarea.status)
                print (tarea.id)
                print ("---------------------")
            }
        }
    } else {
        print ("Opcion Invalida")
    }
}
func completaTarea(arreglo: inout [Tarea]){
    print ("Ingresa el id: ")
    let idTexto = readLine() ?? ""
    if let idInt = Int(idTexto), idInt <= arreglo.count && idInt > 0 {
            let indice = idInt - 1
            arreglo[indice].status = "Completado"
            print("Tarea completada")
    } else {
            print("ID inválido")
    }
}
repeat {
    print ("Que desea hacer?")
    print ("Imprime tareas  ...... (1)")
    print ("Agrega tarea    ...... (2)")
    print ("Completar tarea ...... (3)")
    print ("Salir           ...... (4)")
    var eleccion = readLine()
    switch eleccion {
        case "1":
            imprimeTareas(arreglo: tareas)
        case "2":
            agregaTarea(arreglo: &tareas, identificador: contadorTareas)
            contadorTareas += 1
        case "3":
            print("Sabes el identificador de la tarea?")
            print ("Si .... (1)")
            print ("No .... (2)")
            var detectaTarea = readLine()
            if detectaTarea == "1" {
                completaTarea(arreglo: &tareas)
            } else if detectaTarea == "2"{
                print ("Imprime las tareas y busca el id")
                imprimeTareas(arreglo: tareas)
            } else {
                print ("Opción invalida")
            }
        case "4":
            print ("Salir")
            flujoPrograma = false
        default:
            print ("Elige una opcion correcta")
    }
} while flujoPrograma
```
