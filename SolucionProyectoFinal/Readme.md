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
        }
    }
}
repeat {
    print ("Que desea hacer?")
    print ("Imprime Tareas  ...... (1)")
    print ("Agrega tareas   ...... (2)")
    print ("Salir           ...... (3)")
    var eleccion = readLine()
    switch eleccion {
        case "1":
            imprimeTareas(arreglo: tareas)
        case "2":
            agregaTarea(arreglo: &tareas, identificador: contadorTareas)
            contadorTareas += 1 
        case "3":
            print ("Salir")
            flujoPrograma = false
        default:
            print ("Elige una opcion correcta")
    }
} while flujoPrograma
