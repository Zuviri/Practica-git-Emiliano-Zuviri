# Práctica de Git y GitHub

## Nombre del estudiante

Emiliano Zuviri Castillo 

## Matrícula

2630326

## Nombre de la práctica


*Creación y sincronización de repositorios con Git y GitHub*

## Objetivo

La práctica tiene como finalidad familiarizarse con el manejo de Git y GitHub mediante la creación y administración de un proyecto. Se trabajará con un repositorio almacenado en el equipo y posteriormente se establecerá una conexión con GitHub para transferir y actualizar los archivos entre ambos entornos.


## Descripción del procedimiento

## Descripción del procedimiento realizado

Para comenzar con la actividad, se generó una carpeta denominada `Practica_git_Emiliano_Zuviri`, la cual fue utilizada como espacio de trabajo para los archivos. Posteriormente, se inició PowerShell en dicha ubicación y se ejecutó `git init`, con lo que la carpeta quedó configurada como un repositorio local.

Una vez creado el repositorio, se estableció `main` como rama principal mediante `git branch -M main`. Luego se incorporaron los archivos `README.md` y `datos.txt`; en este último se escribió información inicial correspondiente a la práctica.

Para comprobar la situación de los archivos se ejecutó `git status`. Después, los archivos fueron preparados para su registro utilizando `git add .` y se generó el primer registro en el historial mediante `git commit -m "Primer commit"`.

El siguiente paso consistió en crear un repositorio público en GitHub con el mismo nombre, dejando el repositorio vacío para evitar conflictos con archivos creados previamente. Desde PowerShell se estableció la conexión entre ambos repositorios mediante `git remote add origin`, y posteriormente se comprobó que la dirección remota estuviera configurada correctamente con `git remote -v`.

Una vez establecida la conexión, se ejecutó `git push -u origin main`, permitiendo subir a GitHub los archivos que se encontraban almacenados localmente.

Para comprobar el proceso inverso, se realizó una modificación directamente en `datos.txt` desde GitHub, añadiendo una línea adicional y registrando el cambio mediante un commit. Después, en PowerShell se ejecutó `git pull origin main`, con el propósito de actualizar el repositorio local y obtener la modificación realizada desde GitHub.

Finalmente, se volvió a editar `datos.txt`, pero esta vez desde la computadora. Se revisaron los cambios con `git status`, se prepararon mediante `git add .`, se registraron en el historial con un nuevo `git commit` y, por último, se utilizó `git push` para actualizar nuevamente el repositorio remoto.

Con estas acciones se pudo comprobar la comunicación entre el repositorio local y GitHub, realizando tanto el envío de información desde la computadora hacia el repositorio remoto como la descarga de modificaciones realizadas directamente en GitHub.


## Comandos de Git utilizados

| Comando | Funciónamieto |
|---|---|
| git init | Inicializa un nuevo repositorio Git local. |
| git branch -M main | Cambia el nombre de la rama principal a main. |
| git status | Muestra el estado actual del repositorio. |
| git add . | Agrega los archivos modificados al área de preparación. |
| git commit -m "Primer commit" | Guarda los cambios en el historial local. |
| git remote add origin URL | Vincula el repositorio local con GitHub. |
| git remote -v | Muestra los repositorios remotos configurados. |
| git push -u origin main | Envía los cambios del repositorio local a GitHub. |
| git pull origin main | Descarga los cambios realizados en GitHub. |
| git push | Envía los nuevos commits locales a GitHub. |

## Creación del repositorio local

Para iniciar la práctica, se preparó el espacio de trabajo y se inicializó Git para comenzar a llevar un control de los cambios. Luego, se estableció `main` como la rama principal, se agregaron los archivos requeridos y finalmente se registró la primera versión del proyecto en el historial mediante un commit.


## Vinculación con GitHub

En GitHub se habilitó un nuevo repositorio de acceso público para alojar el proyecto. Posteriormente, se configuró el repositorio local para comunicarse con este espacio remoto mediante `git remote add origin`, estableciendo así el vínculo necesario para intercambiar los archivos y cambios entre ambos repositorios.


## Sincronización Local - GitHub

Para comprobar este flujo se realizó un commit en el repositorio
local y posteriormente se utilizó git push. De esta manera los
archivos y cambios realizados localmente fueron enviados al
repositorio de GitHub.

## Sincronización GitHub - Local

Para comprobar el flujo contrario se modificó el archivo
datos.txt directamente desde GitHub. Después se utilizó el
comando git pull origin main desde PowerShell para descargar
los cambios al repositorio local.

## Archivos del repositorio

### README.md

Tiene  la documentación de la práctica, los comandos utilizados
y la explicación del procedimiento realizado.

### datos.txt

Contiene información relacionada con la práctica y fue utilizado
para comprobar la sincronización de cambios entre GitHub y el
repositorio local.

## Conclusión

Al realizar esta práctica pude comprender mejor el funcionamiento de Git y la manera en que permite llevar un registro de las modificaciones realizadas en un proyecto. También aprendí a utilizar GitHub como una plataforma para almacenar y compartir el repositorio de forma remota.

Además, comprendí la utilidad de los comandos push y pull: push permite enviar los cambios realizados en el repositorio local hacia GitHub, mientras que pull permite descargar las actualizaciones del repositorio remoto. Finalmente, aprendí que un proyecto puede mantenerse sincronizado trabajando tanto desde la computadora como directamente desde GitHub.