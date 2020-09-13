GIT
# Introducción
## Qué es
Es un software de control de versiones, para el mantenimiento de código fuente.
Diseñado por Linus Torvalds.
Su principal propósito es mantener el registro de cambios y cooridnar el trabajo que varias personas realizan sobre archivos compartidos

## Instalación
### Ubuntu
```
apt install git
```
### Windows
[GIT SCM](https://git-scm.com/download/win)
### MacOS
```
brew install git
```

Para revisar la instalación/versión:
```
git --version
```
## Configuración
```
git config --global user.name "fredpaes"

git config --global user.email fred.paucarespinoza@gmail.com
```

```
git config --list
```
## Estados de git
### Working Directory
Área de trabajo local
### Staging Area
Área de preparación - previo al commit
### Git repository
Repositorio donde está almacenado el proyecto

> Ejemplo
> `git init`
> `touch file{1..10}.txt`
> `git add file1.txt`
> `git add .`
> `git rm --cached file1.txt`
> `git commit -m "Se añadieron los archivos iniciales"`
> `git status`

> `echo "Hola mundo" >> file2.txt`
> `git commit -am "Se hizo la modificación del segundo archivo"`
> TRUCO `-am`

## BRANCH
### revisión
`git branch`
### creación
`git branch rama_nueva`
### navegación
`git checkout master`
### eliminación
`git branch -d rama_nueva`
### TRUCO
`git checkout -b rama_truco`
> `git status`
* El estado de los archivos de la rama nueva será desde donde estamos creándola

## PULL && PUSH
## CLONE
## MERGE

## EXTRA
- .gitignore
- .gitkeep
- `git log` && `git log --oneline` && `git log --graph` &&& viaje en el tiempo - recuperando archivos eliminados