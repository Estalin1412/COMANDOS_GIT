# ANDROID STUDIO
# Linear Layout
El tipo de orden que se realizará
```
android:orientation="vertical"
```

# Constrain Layout
## Descargar Android Studio
Programa para crear aplicación en celular
El archivo.kt es donde va la logica de programación

## PROGRAMING
### variables
Este tipo de varible una vez que se asigna su avalor ya no puede cambiar
```
val name: float = 3.14
val name = 3.14f
```
Este tipo de variable puede cambiar sus valor
```
var name: float = 3.14
var name = 3.14f
```
Para cambiar de tipo de variable
```
val altura: float = 1.67
val alturaString: Stirng = altura.toString()
```
Layaout(En la primera parte del código)
Contralayaout : Para aplicacion responsiba
```
androidx.constraintlayout.widget.ConstraintLayout
```
## Forma de Cuadros
Para que el cuadro cambie dependiendo del texto
```
"wrap_content"
```
Para Ajustar toda la pantalla en forma horizontal
```
"match_parent"
```
## Asignar el brackend

Asigna el variable button1 al cuadro creado en el fromt con el id buttonLayout
```
button1 = findViewById(R.id.buttonLayout)
```
Para extraer el texto
```
val textoExtraido = NombreVariable.text
```
Para extraer el texto en String
```
val textoExtraido: String = NombreVariable.text.toString()
```
### Para cambiar titulo o nombre de otro cuadro
```
NombreDeVariable.setText("TextoQueQuieres")
```
## PARA AGREGAR OBJETOS DESDE PROGRAMA
Plaint text: Para editar texto
Button : Botón
Custom: Tipo de pantalla

## Para ubicacion de cuadros
Botton: parte inferior
Top: Parte superior
Start: Parte inicial, la izquierda
End: Parte final, derecha
* Conectar parte inferior con la parte inferior de la pared
```
add:layout_constraintBotton_toBottonOf="parent"
```

# FIRE BASE

# Activity
Layaout: La parte visual y que está en xsml, definir como lauche significa que sea la pantalla central

## CONEXION PARA CON FIRE BASE
### PRIMERO CONFIGURAR PROYECTO DE FIREBASE
- Apretar a android el celular que quieres o tienes
- Agregar un nombre ala base de datos
- Agregar el la especificacion de donde esta com.dots.appdots(Este es un ejemplo, pero debes agregar el nombre del directorio que tienes el main.kts)
- Ir a gradle(parte izquierda de la pantalla un elefante), luego en Execute grandle task(un cuadradito con un icono de youtbe) y agregar el siguiente comando "signingreport", estas ejecutando una tarea necesaria para hallar el numero que tienes que agregar(El numero esta en el SHA1)
- Luego Descargar archivo jason y pegarlo en el apartado app de tu proyecto
- Copiar y pegar las depeendencias necesarias
- Es probable que te salga error porque algunas dependencias se repiten en especial la siguiente ("    id("com.android.application"), Bórrala

# activityLogin
```
}<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".AuthodentyActivity">
    <LinearLayout
        android:id="@+id/lyEscribirID"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:layout_marginTop="32dp"
        >
    <EditText
        android:id="@+id/tvEmail"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        android:hint="Email."

        />
    <EditText
        android:id="@+id/tvPassword"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Contraseña."
        />

    </LinearLayout>
    <LinearLayout
        android:id="@+id/lyOpciones"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"

        android:gravity="center"
        android:orientation="horizontal"
        app:layout_constraintTop_toBottomOf="@+id/lyEscribirID"
        >
        <Button
            android:id="@+id/btnRegistrar"
            android:layout_width="160dp"
            android:layout_height="wrap_content"
            android:text="REGISTRAR"
            android:backgroundTint="@color/MarineBlue"
            android:layout_marginEnd="8dp"
            />
        <Button
            android:id="@+id/btnAcceder"
            android:layout_width="160dp"
            android:layout_height="wrap_content"
            android:text="ACCEDER"
            android:layout_marginStart="8dp"
            android:backgroundTint="@color/MarineBlue"
            />

    </LinearLayout>

</androidx.constraintlayout.widget.ConstraintLayout>
```
