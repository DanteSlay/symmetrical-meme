# P04 - GitHub (remoto) a local
__Javier Arreaza__
___
### TRABAJAR CON FICHEROS MARKDOWN
Vamos a crear un __repositorio público__, con una __descripción__, un fichero __README.md__, un fichero __.gitignore__(modelo por defecto para ficheros *Java*) y __licencia MIT__ dentro de nuestro perfil de __GitHub__.

![Crear un Repositorio GitHub](/img/crearRepositorio.png)

Para ___clonarlo y tener una copia del repositorio en local___, seguimos estos pasos:
1. En GitHub.com, navegue a la página principal del repositorio.
2. Encima de la lista de archivos, haga clic en __<> CODE__.

![Botón Code](/img/clonarRepositorio01.png)

3. Copia la dirección ___URL___ del repositorio.
    - Para clonar el repositorio con HTTPS, en «HTTPS» haz clic en 📋. 
    - Para clonar el repositorio mediante una clave SSH, incluido un certificado emitido por la entidad de certificación SSH de la organización, haga clic en Usar SSH y luego en 📋.
    - Para clonar un repositorio mediante GitHub CLI, haz clic en GitHub CLI y, después, haz clic en 📋.

    ![Copiar https:github](/img/clonarRepositorio02.png)

4. Abra ___Git Bash___ desde la carpeta 📁 donde quieras clonar el directorio.

5. Escriba `git clone` y pegue la _dirección URL_ que ha copiado antes.
~~~
$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
~~~
![Codigo git clone](/img/clonarRepositorio03.png)
![Confirmacion git clone](/img/confirmacionClonacionRepositorio.png)

Con esto ya tendremos __copiado__ el repositorio en _local_.

![Repositorio Clonado](/img/carpetaClonada.png)
___
### <u>BIFURCAR UN REPOSITORIO</u>
#### Qué ocurre si modificamos un repositorio clonado❔❔❔
Para ello vamos a ___bifurcar___ un repositorio __random__ de __GitHub__ que contenga ejercicios de _programación en Java_ 🍵.

En GitHub se bifurca desde la pagina de un repositorio, pinchando en el botón ___Frok___ de la esquina superior derecha.

![Botón Fork](/img/botonFork.png)

![Crear Bifurcación](/img/crearFork.png)


Ya nos dicen en este punto que una ___bifurcación no afecta al repositorio original___:


~~~
A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.
~~~
<img src="https://media.giphy.com/media/McHNcxIszjVStqZZ8s/giphy.gif" width="100" height="100"/>

Por lo que __confirmamos sin miedo__ 😎.

Ahora veremos que una ___copia___ de ese directorio aparece en nuestros __repositorios__.

![Página de repositorio bifurcado en GitHub](/img/bifurcacion.png)

Seguimos los pasos _anteriores_ para __clonar__ el repositorio en local.

![Repositorio clonado en local](/img/archivosRepBif.png)

Ahora para __probar__ que sucede si trabajamos sobre este proyecto vamos a __eliminar__ 💣 y __editar__ 📝 algun _archivo_.
- _Cambiamos el nombre_ del __README.md__ a __README2.md__.
- ___Eliminamos___ el archivo __.gitignore__.
- _Creamos_ la carpeta __HolaMundo__.

![Archivos editados en local](/img/bifEditada.png)

Confirmamos el proyecto y los subimos a __GitHub__:
1. Abrimos ___Git Bash___ y comprobamos el estado del _repositorio_ con:
    - `git status`.

    ![Git Status](/img/gitStatusGrande.png)

    - Si lo queremos ver en un estilo ___simplificado___ podemos usar `git status -s`.

    ![Git Status simplificado](/img/gitStatusPequeño.png)

2. ___Añadimos___ los cambios a la __zona de preparación__ con `git add "FILE"`.

![git add .](/img/archivosRepBif.png)

3. ___Comprobamos___ una vez más con `git status -s` y nos dice que _todos los cambios estan listos para hacer commit_.

![git status 2](/img/gitStatus2.png)

4. Hacemos ___commit___ con `git commit -m "text"`.

![git commit -m "text"](/img/gitCommit.png)

5. ___Conectamos___ el repositorio con __GitHub__ `git push -u origin master` 








