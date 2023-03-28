# Versionamiento de codigo

## Inicializacion de un repositorio

1. Crear la estructura de carpetas de nuestro proyecto.

- `mkdir nombre_carpeta`: Creamos la carpeta principal
- ` cd nombre_carpeta`: Ingresamos a la carptea
- `code .`: Abrimos VSC en el directorio en el que nos encontramos
- Una vez abierto el VSC nos creamos las carpteas y archivos necesarios
- Abrimos la terminal
- Ejecutamos el comando `git init`: Para inicializar el repositorio
- Ejecutamos el comando ` git add .`: Anadir TODOS los nuevos archivos y carpetas al espacio de preparacion (Staing area)
- Ejecutamos el comando `git commit -m "Mensaje del commit"`: Anade un comentario a los cambios echos

2. Crear el repositorio remoto en nuestra cuenta de Github

- Ingresar a nyuestra cuenta github
- Creamos nuestro repositorio
- Nos regresamos a la terminal del proyecto en VSC para ejcutar las ultimas lineas.
  - `git remove add origin https://github.com/J-Ciro/ejemplo.git` : para renombrar la rama pirmcipal
  - `git push -u origin maion:` Se suben todos los archivos al repositorio remoto

## Subir cambios a un repositorio

1. comporbar el estado de los archivos: `git status`
2. `git add .`
3. `git commit -m "mensaje del commit"`
4. `git push origin nombre_rama_actual`

## Trabajar con estrategias de branching

Existen dos tipos de estrategias de branching:

1. Trunk-based: Cuando trabajamos de manera individual
2. Git Flow: Cuando trabajamos de manera colaborativa

## Trabajar con Git Flow

1. Se ejcutan los pasos anteriores (Inicializacion del repositorio)
2. Va a crear la rama develop: `git checkout -b develop`
3. Agregar unos cambios minimos
4. Desde la rama develop ejecuta los pasos de `Subir cambios a un repositorio`
5. Ir al repositorio remoto en GitHub, dando click sobre el boton compare & pull request
6. Generamos el pull request
7. Github nos va a indicar si existen conflictos (Si existen, se deben resolver)
8. Una vez resueltos los conflictos realiamos el merge de develop a main y confirmamos el merge (todo esto pasa en la pagina de gitub)
9. En la terminal de VSC nos movemos a la rama main `git checkout main`
10. Ejecutamos `git pull` para actualizar nuestro repositorio local

#### Nota:

- `git reset`: deshace `git add .`
