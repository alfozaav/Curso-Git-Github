# Comandos Github 💻 ⌨️

**Esta es una lista de todos los comandos que usé durante el Curso Profesional de Git y Github de platzi.**

Fue elaborada para tener un fácil acceso a ellos en caso de ser necesario.

 >*Además. mi letra es horrible  *  : V
 
 ### Comandos:
 - **$git  init //** Situado en la carpeta del proyecto, inicia el repositorio (master).
 - **$rm -rf.git //** Elimina el repositorio master.
 - **$git add nombre_archivo.txt//** Agrega un archivo al repositorio.
 - **$git commit -m "Mensaje"//** Guarda los cambios después de agregar el archivo, siempre va después de **$git add.**
 - **$git add . //** Agrega todos los archivos de la carpeta.
 - **$git status //** Muestra el estado del repositorio, en qué rama se encuentra y si hay cambios hechos sin guardar.
 - **$git show //** Muestra todos los cambios hechos.
 - **$git log archivo.txt //** Muestra la historia del archivo.
 - **ls //** Lista los archivos de la carpeta.
 - **ls -al //** Lista los archivos de la carpeta, incluyendo los que están ocultos.
 - **tab //** Autocompleta los comandos.
 - **cd nombre_carpeta //** Entra en la carpeta deseada.
 - **cd ~ //** Entra en el home (carpeta de usuario).
 - **cd .. //** Regresa un paso afuera de la carpeta en donde te encontrabas.
 - **pwd //** Muestra en donde te encuentras.
 - **mkdir nombre_carpeta //** Crea una carpeta.
 - **touch //** Crea un archivo vacío.
 - **cat nombre_archivo //** Muestra el contenido del archivo en consola.
 - **history //** Muestra toda la historia de comandos hechos, para repetir uno puedes usar las flechas **arriba/ abajo** o también poniendo el número que el comando tiene en la historia.
 - **rm nombre_archivo //** Borra archivo.
 - **comando --help //** Muestra los opciones del comando puesto.
 - **$git checkout //** Trae cambios del repositorio Master a tu carpeta local.
 - **$git config  --global user.name //** Añade tu usuario a Git.
 - **$git config --global --unset --all user.name //** Elimina usuario.
 - **$git config --global user.email //** Añade email de usuario.
 - **$git config --global --all user.email //** Elimina email.
 - **$git config -l / $git config -global --list //** Verificas que lo hiciste bien.
 - **vi nombre_archivo //** Edita archivo con Vim,para comenzar a escribir es **Esc + i** y para salir del editor es **Esc + Shift + z + z.**
 - **vim nombre_archivo //**  Crea archivo y lo edita con Vim.
 - **$git diff commit 2 commit 1/ $git diff //** Muestra las diferencias hechas entre commits en el archivo.
 - **$git reset numero_commit --hard //** Fuerza todo a volver una versión anterior (la que se seleccione con el número de commit) y borra lo que se encuentre en staging (en la memoria ram). **No se recomienda usar este comando mucho.**
 - **$git reset numero_commit --soft  //** Vuelve a la versión anterior del commit y lo que está en staging sigue ahí (lo que está en la memoria ram en el momento y no se ha guardado).
 - **$git log --stat //** Muestra todas las versiones hechas (todos los commits), con las flechas te mueves entre ellas y con **q** regresas a escribir comandos.
 - **$git checkout numero_commit nombre_archivo //** Cambia el archivo a la versión que seleccionaste.
 - **$git checkout master nombre_archivo //** Trae la última versión del archivo.
 - **$git rm -cached //** Elimina archivo del staging, pero no del disco duro.
 - **$git rm --force //** Elimina archivo del staging y del disco duro.
 - **$git reset HEAD //** Saca archivos del area de staging para que los cambios de estos no se envien al último commit, al menos que cambiemos de opinión y los incuyamos de nuevo con **$git add.**
 - **$git commit -am "mensaje" //** Solo funciona con archivos a los que ya le has hecho **git add** antes, guarda los cambios y los manda al master  (add + commit).
 - **$git branch nombre_rama //** Crea una rama.
 - **$git checkout nombre_rama //** Mueve de rama el repositorio (cambias entre las diferentes ramas que puedas tener).
 - **$git branch //** Muestra todas las ramas que tienes.
 - **$git merge nombre_rama //** Se ejecuta en la rama donde quieras fusionar los archivos con la rama que pusiste en el comando, fusiona los archivos para tener una version completa.
 - **$git remote add origin github_url //** Añade dirección remota para hacer fetch o push.
 - **$git remote //** Muestra origen.
 - **$git remote -v //** Muestra las Urls.
 - **$git pull origin master (fetch + merge) //** Trae lo último de Github al master local.
 - **$git pull origin master --allow-unrelated-histories //** Trae historias no relacionadas con el repositorio, como README.md y soluciona el error cuando ejecutas pull por primera vez.
 - **$git push origin master //** Envía al repositorio de github los cambios del repositorio local.
 - **$git log --all --graph --oneline //** Muestra el arbol con todos los cambios y ramas del proyecto.
 - **$alias nombre "comando" //** Pone un alias (nombre) a un comando para acceder a él de manera más corta y fácil.
 - **$git tag -a v0.1(nombre) -m "mensaje" numero_commit //** Crea una etiqueta para especificar alguna versión.
 - **$git show-ref --tags //** Para saber a que commit se relaciona la etiqueta.
 - **$git push origin --tags //** Manda las etiquetas a tu repositorio de Github.
 - **$git tag //** Muestra todas las etiquetas.
 - **$git -d tagname //** Borra una etiqueta de tu repositorio local, para borrarla de tu repositorio de Github tienes que poner después de eso el comando **$git  push origin: refs/tags/tagname. **
 - **$git show-branch //** Muestra ramas y sus historias.
 - **$git show-branch --all //** Más resumido.
 - **$gitk //** Muestra la historia de manera visual.
 - **$git push origin branchname //** Manda rama al repositorio en github.
 - **$git clone url //** Clona el repositorio en linea en tu repositorio local.
 - **Ctrl + Shit + r //** Fuerza la actualización de una página.
 - **$git branch -D //** Borra ramas.
 - **$git stash //** Recupera los cambios, como un Crtl + Z.
 - **$git stash pop //** Rehace los cambios.
 - **$git stash list //** Muestra los cambios.

### Llaves SSH 🔑 

Pasos para crear y enviar llaves SSH a github para establecer una conexión más segura y sin necesidad de estar poniendo tu contraseña a cada rato.

Desde el home:
**ssh -keygen -t rsa -b 4096 -C correo_repositorio**

Asegurarme de que el servidor de llaves SSH esté encendido.
Windos/Linux:
**$eval $(ssh-agent-s)**
Agregar llave al sistema
**$ssh-add ~/.ssh/keyname**

Mac:
**eval "$(ssh-agent-s)"**
Si estas en un Mac con software reciente, lo más probable es que no exista un archivo llamado config en el directorio .ssh, así que debes crearlo.
Crear archivo
**$vim config**
				Host
				AddKesyToAgent yes
				UseKeyChain yes
				IdentifyFile ~/.ssh/keynamefile (id_rsa)

Agregar este archivo al agente
**ssh-add -K ~/.ssh/keynamefile(id_rsa)**`


Cambiar Url de origen a la llave SSH
**$git remote set-url origin GithubUrl**

Eso es todo, ahora ya tienes tu llave SSH configurada en tu máquina, el siguiente paso es agregarla a tu perfil de Github y listo, tendrás una conexión segura e ininterrumpida con tu repostorio en la nube.

**Se recomienda tener una llave por equipo, en caso de que cambies de computadora es mejor generar otra que querer pasar tu llave actual a tu equipo**
 
 
 
 






