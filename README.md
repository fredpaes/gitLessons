__________________________________
# RESUMEN
# INTRODUCCIÓN
## Qué es git
Es un software de control de versiones, para el mantenimiento de código fuente.

Su principal propósito es mantener el registro de cambios y coordinar el trabajo que varias personas realizan sobre archivos compartidos.

Diseñado por Linus Torvalds.

## INSTALACIÓN
### Ubuntu
```
sudo apt install git
```
### Windows
Descargar el ejecutable desde [GIT SCM](https://git-scm.com/download/win)
### MacOS
```
brew install git
```
Para revisar la instalación / versión:
```
git --version
```

## CONFIGURACIÒN
```
git config --global user.name "Fred Paucar Espinoza"

git config --global user.email fred.paucarespinoza@gmail.com
```
Para revisar la configuración:
```
git config --list
```

## ESTADOS DE GIT
### Working Directory
Área de trabajo local
### Staging Area
Área de preparación - previo al commit
### Repository
Repositorio donde está almacenado el proyecto

![alt text](./assets/git_stages.png "GIT STAGES")
<!-- >Ejemplo
> `git init`
> `touch file{1..10}.txt`
> `git add file1.txt`
> `git add .`
> `git rm --cached file1.txt`
> `git commit -m "Se añadieron los archivos iniciales"`
> `git status`

> `echo "Hola mundo" >> file2.txt`
> `git commit -am "Se hizo la modificación del segundo archivo"`
> TRUCO `-am` -->

## RAMAS
| ACCIÓN | COMANDO |
| :----- | :-----: |
| Revisión | ` git branch ` |
| Creación | ` git branch new_feature ` |
| Navegación | ` git checkout master ` |
| Eliminación | ` git branch -d hot_fix ` |
### Tip
> Para crear y movernos a una nueva rama `git checkout -b rama_tip`

* El estado de los archivos de la rama nueva será desde donde estamos creándola

## TRABAJANDO EN EQUIPO
| ACCIÓN | COMANDO |
| :----- | :----- |
| Clonar un repositorio | ` git clone <url_del_repositorio>` |
| Obtener los cambios remotos | ` git pull origin master ` |
| Enviar mis cambios | ` git push origin master ` |
| Unir ramas | ` git merge rama_nueva ` |

## EXTRAS
| ACCIÓN | SOLUCIÓN |
| :----- | :----- |
| Ignorar archivos | **.gitignore** |
| Mantener directorios | **.gitkeep** |
| Revisar el log de cambios | ` git log `<br>` git log --oneline `<br>` git log --graph ` |
