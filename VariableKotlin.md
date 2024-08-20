## Int
Formato 
tipo - nombre - variable - valor
```
var name: String = 14
```
* var : Cambia el valor.
* val : No cambia el valor.
## String
* $ : Concatenacion
```
println("Hola $name")
```
## Nulabilida
Alveces la variables pueden ser nulas(null), no hay valor

```
var name:String? = null
```
* ? : Pregunta si no es nulo, se ejecuta el get; sino, no se realiza nada
```
println(name?.get(3))
```
## Funciones 
```
fun Name( var:Int): Float{

}
```
## when

```
when (valor){
    in 3 .. 6 this -> 20
    else this-> 0
}
```

## Para arreglos
```
val weekDays = arrayOf("Lunes","Martes")
```
## For
```
for (position in weekDays.indices){
    println(weekDays[position])
}

for ((position, value) in weekDays.withIndex){
    println("La posición $position, contiene $ value")
}
```