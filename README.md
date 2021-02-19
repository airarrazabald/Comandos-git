# Comando útiles GIT

## 1. git init

Inicializa un proyecto, me permite utilizar Git como control de versiones.
Nos posicionamos en la carpeta del proyecto y ejecutamos
```bash
git init
```
## 2. git add .

agrega nuevos archivos al control de versiones

* Agregar todos los nuevos archivos: 
```bash
git add .
```
* Agregar un archivo especifico
```bash
git add <file>
git add nuevoarchivo.js
```
## 3. git reset .
## 4. git commit
El commando git Coomit permite guardar los cambios realizados.
Debemos incluir el ocmando -m pa elmensaje del commit
```bash
git commit -m "Mensaje del commit"
```
Una forma mas rapida de agregar archivos al control de versiones (evitando el comando git add) es agregando -am
```bash
git commit -am "MEnsaje del commit"
```
## 5. git checkout -- .
Para reversar cambios locales como por ejemplo eliminación de archivos o modificación de archivos.

```bash
git checkout -- .
```

Este comando reversara todos los archivos del directorio actual.
## 6. git log
Nos permite revisar el historial de commit de la rama actual
```bash
git log 
```
## 7. git commit --amend
## 8. git checkout -b nombre-rama

## 9. git checkout nombre-rama
Comando para cambiar de rama.
```bash
git checkout <nombre-rama>
git checkout rama-pruebas
```
## 10. git branch -d rama-heroes
## 11. git push
Con este comando podemos subir nuestro codigo a un repositorio como por ejemplo github, gitlab, bitbucket, etc.
```bash
git push
```

Al trabajar con ramas, y si necesitamos subir los cambios a un repositorio remoto, debemos ejecutar el siguiente comando
```bash
git push origin <nombre_rama>
```

## 12. git pull
Comando para actualizar con los ultimos cambios.
Loque realiza es descargar y fusionar los cambios del repositorio remoto.
```bash
git pull
```

## 13. git status

Comando que nos permite ver el estado del proyecto en control de versiones
* Puede indicar si debe agregar archivos
* Realizar push en el repositorio 
* Si no hay cambios indicara lo siguiente <b>your branch is up to date with origin/main</b> donde origin/main es la branch que esta trabajando 

## 14. Consideraciones
### .git ignore
### Ebook gratuito
Todos los comando incluidos en este pequeño manual los puedes revisar en mayor detalle en el siguiente ebook gratutio de la pgina oficial de git:
[Ebook git](https://git-scm.com/book/es/v2)


