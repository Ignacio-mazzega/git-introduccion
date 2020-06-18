1. ¿Qué es git?

GIT es un sistema de control de versiones open source, es decir controla distintas versiones de un programa.

2. ¿Por qué queremos utilizar git?

Porque como desarrolladores queremos controlar un proyecto que va a crecer y va a sufrir cambios o actualizaciones.

3. ¿Qué es el bash que instala git?

Es un terminal o consola pero con mejores funcionalidades, trae todos los conceptos de Unix.

4. Describa los estados (working directory, staging area, repository)

Working directory: Aquí es donde podemos hacer cualquier cambio y no afectar nuestro repositorio en lo absoluto.
Una vez que hemos hecho los cambios necesarios, pasamos nuestros archivos al “staging area” con el comando:
git add nombreDeArchivo
Cuando pasas el código de Working Directory a Stagin Area, cambias el estado del código de modificado a preparado.

Staging area: Aquí es donde le podemos dar nombre a nuestra nueva versión. Y crear una “copia” de cómo quedaría nuestro repositorio en producción.

Para pasar nuestro código de staging area al Git Repository (aun no se publica el código en Github), escribimos el siguiente comando:
git commit -m "Nombre del la nueva versión"

Nota que cuando haces el commit el código pasa de estado preparado a confirmado.

Repository: Una vez que el código esta confirmado ya esta listo para sincronizarse con el servidor de Git (github, bitbucket,etc). Para hacer esto, escribimos:
git push -u origin master



5. Describa el flujo para crear un nuevo repositorio git.

Ingresamos a Github, nos vamos a "repositorios" y a la derecha damos click al botón "New", ya en la siguiente ventana colocamos un nombre al repositorio y una descripción si asi lo desea, decidimos si va a ser público o privado (opción paga) y le damos click a 'Create repository'.

6. Describa el flujo para agregar un archivo simple al repositorio.

Para agregar un archivo usamos el comando git remote mas el link del repositorio que creamos:
git remote add origin https://github.com/Ignacio-mazzega/git-introduccion.git
luego usamos el comando git push -u origin master que lo cargara a Git.


7. Describa el flujo para cambiar el archivo agregado y guardar los cambios en el repositorio.
8. ¿Cómo hago para ignorar un archivo o carpeta?

Lo hace creando un archivo llamado .gitignore, dentro de él se colocan los nombres de la carpeta o archivos que queremos ignorar y luego se agrega el archivo .gitignore con el comando git add.

9. Explique qué es un branch. Dé un pequeño ejemplo de cómo haría uno.

Es el apuntador a la rama local en la que tú estés en ese momento(master). Se realiza colocando el comando git branch y el nombre que le queramos poner, "login" por ejemplo.

10. ¿Qué hago con `git add .`?

Es para pasar los archivos del working directory al staging area.

11. ¿Cómo cambiamos de un branch a otro?

Con el comando git checkout y el nombre del branch al que queramos pasar.

12. Investigue qué es Markdown y responda todas las preguntas anteriores en este lenguaje (con el nombre de archivo RESPUESTAS.md). Súbalo al repositorio.


Ejercicio 1:
Abrir una cuenta en Github / Gitlab.
Crear un repositorio público.
Subir el repositorio que hemos creado anteriormente siguiendo el video y que tenga las respuestas del cuestionario.
Dejar el link del repositorio junto al nombre del alumno. Para ellos habrá un formulario en la plataforma.