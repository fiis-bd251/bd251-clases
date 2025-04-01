# Crear un Pull Request en Github
Durante el desarrollo del curso, cada integrante deberá incorporar sus cambios al repositorio de su grupo haciendo uso de un Pull Request (PR).

A continuación, presentamos los pasos para que puedan realizar la creación.

## Clonar / Actualizar el repositorio
En caso no tengan una copia de su repositorio localmente, pueden utilizar `git clone`:
````
git clone https://github.com/xyz/mirepo
````
Si ya tiene una copia local del repositorio, puede ingresar a esa carpeta y ejecutar el siguiente comando. Debemos tener cuidado, ya que si tenemos cambios que no hayamos confirmado (commit), es posible que los perdamos:
````
git pull
````

## Crear una nueva rama (branch)
Para poder rabajar de forma rápida y no generar conflictos con el trabajo de sus compañeros, deberá crear una rama (branch). A partir de dicha rama se creará el Pull Request para incluir sus cambios (merge) a la rama principal (main). Este es el comando para la creación:

````
git checkout -b nombre-rama
````
## Incluir sus cambios
Puede trabajar en VSCode o en cualquier otro editor de texto para modificar los archivos necesarios con el contenido que sea agregar, luego de ello debe agregar sus cambios (add) y confirmarlos (commit). Los comando son los siguientes (agrega todos los archivos modificados):

````
git add .
git commit -m "Mensaje del commit (descripcion de cambios)
````
## Subir sus cambios a Github
Hasta ahora todos los procesos se han trabajado localmente, para que los cambios realizados se puedan subir a Github, es necesario subirlos (pull). Este es el comando (debe indicar el nombre de la rama en la que ha estado trabajando).

````
git push origin nombre-rama
````

## Crear Pull Request
Una vez que se haya subido puede seguir [estos pasos](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) para la creación del Pull Request. Para objeto del curso, es necesario que cada PR sea aprobada por lo menos por un integrate del grupo (que actuará como "Reviewer"). Una vez que se tengan todas las aprobaciones, podrá presionar el botón `Merge` y sus cambios serán incorporados a la rama principal.

