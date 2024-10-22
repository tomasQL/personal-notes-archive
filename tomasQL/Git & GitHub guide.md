## Personal Guide

> @tomasQL <https://github.com/tomasQL>  
> Fecha de creación Jueves 01 de septiembre del 2022.

Generar clave SSH:

	- Paso 1: ir hasta la carpeta de usuario mediante línea de comandos.
	Normalemente C:/Users/NombreDeUsuario  
	- Paso 2: verificar que no exista ya una carpeta .ssh con:
	$ ls .ssh  
	
	- Paso 3: $ mkdir .ssh  y luego entrar a la carpeta $ cd .ssh  
	- Paso 4: $ ssh-keygen -t rsa -C "tucorreoemail@email.com"  (el de github)
	- Paso 5: le saldrá el path donde se va a generar, apretar ENTER.
	- Paso 6: les pedirá ingresar un passphrase, por ahora dejenlo vacío (ENTER)  
	  les aparecerá dos veces, dejenlo vacío.
	- Paso 7: Debería salir una "key's randomart image"
	- La clave SSH ya fue creada.  
	- Revisen la carpeta oculta .ssh que debería estar en C:/Users/MiUsuario/.ssh/
	deberían haber dos archivos, si habilitan ver la extensión o tipo de archivo,  
	verán un id_rsa y un id_rsa.pub  
	- Paso 8: dirigirese a GitHub, configuración, entrar al apartado SSH and GPG  
	  keys.
	- Paso 9: Denle un título a la clave (WINDOWS Usuario o lo que quieran) 
	- Paso 10: Abrir el archivo id_rsa.pub con un editor de texto, copian y pegan  
	  todo.
	- Paso 11: agregar y probar si todo salió bien, en la terminal desde cualquier  
	  directorio $ ssh -T git@github.com  les saldrá una opción yes/no, colocar yes.
	- Paso 12: verificar que de respuesta en la terminal les salga un $ Hi  
	  UsuarioGitHub  
	- Paso 13: probar la conexión clonando cualquier repositorio de github por SSH,
	  por ejemplo el de nosotros o cualquier otro $ git clone  
	  git@github.com:usuario/repositorio.git  
	- Con esto ya deberían poder hacer pull o push a sus repositorios o al del 
	proyecto  

	No olvidar vincular con los comandos de abajo "Configuración Global del usuario"
	el username y email de su cuenta de github.


## 1. Conceptos fundamentales

    git help nombre_comando    

Nos lleva a la documentación del comando elegido.  

**Configuración global del usuario**

    git config --global user.name "tomasQL"     
    git config --global user.email "tomasgaticagomez@gmail.com"

Consultar los usuarios registrados.

    git config --global -e    

Entorno linux (Arch-MANJARO)  
Setear idioma de español al inglés.    

    alias git='LANG=en_US git'

### **Iniciando repositorios**

Dentro de la carpetra mediante CLI ejecutamos

    git init // Inicializa el repositorio  
    git status 
    git add . //  Añade todos los archvos de la carpeta.
    git commit -m "Primer commit" //  Comprometerlos - realizar los cambios del snapshot

**Sobre la inicialización de repositorios**

Una vez que hemos inicializado el repo y, en general, cada vez que tenemos archivos nuevos *untracked* debemos usar si o si el formato extendido de 
git add . y git commit -m "MENSAJE". Una vez que el seguimiento de git fue aplicado podemos utilizar en dichos archivos o carpetas los alias de git simplificados.

<hr>

### **Stage y Commit**

En git existen dos conceptos fundamentales, el stage y el commit.
El stage es el momento donde preparamos los archivos para ser comprometidos y el commit como dice su nombre en EN es comprometerlos.  

<hr>  


ALIAS shortcuts in GIT CLI

git status --short             //  visualiza el status de manera resumida 

git config --global alias.s "status --short"

    ALIAS Popular FH git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) % (dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
    
    git config --global alias.s "status --short"

<hr>

### **Warnings y cambios ligeros**

Error Warning LF CRLF  

    git config core.autocrlf true

Si necesitamos cambiar el nombre de una rama (repo local-only):

    git branch -m master main  

Global para las siguientes ramas de manera default:

    git config --global init.defaultBranch <nombre>  

<hr>

### **Deshaciendo cambios**

    git checkout -- . 

Reconstruye (solo lo que este TRACKED/en seguimiento) el repositorio dede el estado del último snapshot.  
  
Cuando queremos bajar un archivo del stage (after git add .)

    git reset <Filename> // i.e git reset README.md  
  
<hr>

Después de comenzar a dar seguimiento a los archivos, podemos realizar los commits  
con la forma abreviada que otorga Git.

    git commit -am "MENSAJE"
  
<hr>
  
### **Sobre los archivos**
Para añadir, filtrando por tipos de archivos  
git add *.tipo_archivo   
*i.e*

    git add *.py             //  añade todos los archivos desde el root con
                             //  extensión .py en subdirectorios 
    git add carpeta/         //  añade la carpeta
    git add carpeta/*.js     //  añade los archivos js de la carpeta llamada carpeta

Para remover un archivo del seguimiento (ya mencionado)

    git reset .DS_Store //    archivo de OSX, el archivo ya no es parte de la snapshot
  
En algunos casos podremos tener carpetas vacías; las carpetas vacías no son ni  
alarmadas a git. Pero por motivos de etapas en el desarrollo podremos querer  
mantenerlas, deberemos añadir el archivo **.gitkeep** dentro de dicho directorio.  

**OBS:**  
Los archivos que no tienen nombre pero si una extensión como el ejemplo anterior  
.gitkeep; cuando queremos añadirlos específicamente (dir/file) hay que quitarle  
el asterísco al comando add.

    git add carpeta/.filename  
    i.e git add uploads/.gitkeep    // no uploads/*.gitkeep

<hr>
  
Para observar diferencias de los cambios hechos en el repo  
utilizaremos el comando git diff. No obstante, el tooling  
visual como el que otorga VSCode u otros IDEs de desarrollo  
pueden llegar a ser más útiles ya que al usar un *git diff*  
lo estaremos observando desde la consola.  

  
    git diff <filename> // sin el filename cuando solo  
                        // hemos modificado 1 archivo  
                        // sin haberlo pasado al stage
    
    git diff --staged   // flag añadida para cuando  
                        // queremos ver la diff en un  
                        // archivo en el stage.  


<hr>
  
### **Actualizando commit message**  
  
**Last commit**  
  
    git commit --amend -m "NEW MESSAGE"  

#### **Revirtiendo commits**



