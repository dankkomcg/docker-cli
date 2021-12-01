# Docker CLI

# requisitos
* MacOS/Linux: `git` y `docker`. 
* Windows: WSL + Docker Desktop.

# iniciar cli
* Asignarle permisos al módulo `run`: `chmod u+x run`
* Ejecutar `./run`
* Seguir las instrucciones del menú

# recetas
Acceder a `gestión de recetas`:
* `remotas`: recetas que se solicitan desde un repositorio remoto. Es necesario indicar el nombre del directorio donde se almacenará y la url del repositorio.
* `locales`: crea el directorio y el `Dockerfile` pero es necesario cubrirlo a mano

## recetas remotas
Es necesario que: 
* la versión debe coincidir con la versión etiquetada en el repositorio remoto.
* indicar un `Dockerfile` en el directorio raíz del proyecto remoto del que parte la receta*. Si no lo incluye, se creará pero deberá ser cubierto a mano.

# imágenes
Acceder a `gestión de imágenes`:
* Indicar el nombre asignado a la receta de la que partirá la imagen (debe estar construida la receta previamente desde `gestión de recetas`)$

# Contenedores
Seleccionar "gestión de contenedores":
* seleccionar alguna de las opciones del menú.
* Recomendable listar los contenedores previamente.
