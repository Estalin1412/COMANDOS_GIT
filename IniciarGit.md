# INICIAR GitHub
## Iniciar repositorio remoto
Configuramos nombre de usuario y correo electrónico para luego asociarlo a nuestor repositorio local(Recomendable que sea lo mismo que nuestro gitHub).
```
git config --global user.name "Estalin1412"
git config --global user.email "jose.munoz.d@uni.pe"
```
Creamos nuestro repositorio remoto en la carpeta que deseamos.
```
git init
```
```
git config user.name "Estalin1412"
git config user.email "jose.munoz.d@uni.pe"
```
## Comunicación Repositorio remoto con GitHub
Asociamos nuestro repositorio remoto con git (El nombre origin lo puedes cambiar, pero no olvidar con que nombre se guarda)
```
git remote add origin https://...

```
### Comandos extra remote
* Para ver que hay.
```
git remote -v 
```
* Para eliminar origin(Nombre del repositorio asociado)

```
git remote remove origin
```
## Subir archivos

Para subir los archivos necesitramos nombre el repositorio asociado(origin) y nombre de la rema que queremos subir(master)
```
git push -u origin master
```
# COMANDOS
## Comandos en Ramas
* Saber qué rama estamos.
```
git branch
```

* Crear una rama rama1
```
git branch rama1
```
* Cambiar nombre de rama1 a ramita
```
git branch rama1 ramita
```
* Eliminar ramita(nombre de la rama a eliminar)
```
git branch -d ramita 
```
* Cambiar de rama
```
git checkout master
```
## Comandos de guardado
* Para subir cambios( el punto significa todo pero tambien puedes especificar agregando solo los nombre que quieres subir)
```
git add .
```
* Para confirmar y guardar los cambios
```
git commit -m "MensajeDeConfirmacionQueDesees"
```