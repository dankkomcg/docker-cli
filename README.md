# Bash Docker Helper

## Requisitos
* Tener instalado `git`
* Tener instalado e iniciado `docker`

## Elementos a tener en cuenta:
* `Recetas`: directorios base de los que parten las imágenes.
    * `recetas locales`: se construye solo la estructura de la carpeta (crea un `Dockerfile`). Es necesario configurarlo a mano
    * `recetas remotas`: se descargan desde un repositorio remoto. Es necesario indicar el link del repositorio.

## Iniciar el programa
* Asignarle permisos al módulo `run`: `chmod u+x run`
* Ejecutar `./run`
* Seguir las instrucciones del menú

## Construir recetas
* Acceder a `gestión de recetas`
* `remotas`: recetas que se solicitan desde un repositorio remoto. Es necesario indicar el nombre del directorio donde se almacenará y la url del repositorio.
* `locales`: crea el directorio y el `Dockerfile` pero es necesario cubrirlo a mano

## Construir imágenes
Acceder a `gestión de imágenes`.
Indicar el nombre asignado a la receta de la que partirá la imagen (debe estar construida la receta previamente desde `gestión de recetas`). Requieren indicar el nombre y la versión tanto para remotas como para locales. 

### Sobre las imágenes desde recetas desde repositorios remotos
Es necesario que: 
* *la versión debe coincidir con la versión etiquetada en el repositorio remoto*.
* *indicar un `Dockerfile` en el directorio raíz del proyecto remoto del que parte la receta*. Si no lo incluye, se creará pero deberá ser cubierto a mano.

## Contenedores
* Seleccionar "gestión de contenedores" y seleccionar alguna de las opciones del menú.
* Recomendable listar los contenedores previamente.

## Enlaces de interés
* [Reemplazar contenedor por nueva instancia](knowledge-base/1.0.0_fba_reemplazar_contenedor)
* [Construir desde imágenes base](knowledge-base/1.0.0_fba_proyectos_imagenes_base)
* [Acceder vía IP a los contenedores](knowledge-base/1.0.0_fba_como_acceder_via_ip_contenedores.md)