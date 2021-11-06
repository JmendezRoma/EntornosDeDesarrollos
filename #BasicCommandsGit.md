TAREA 2
MANIPULACIÓN DE REPOSITORIOS EN GIT



Este informe trata de mostrar algunos de los comandos basicos para la interacción de los repositorios
de git directamente con la terminal de linux.

1. Configuración 
Configuración del nombre de usuario, correo electrónico y activacion del coloreado de salida. Porúltimo podemos
solicitar que se nos muestre la configuración resultante.
  git config --global user.name "Your-Full-Name"
  git config --global user.email "your-email-address"
  git config --global color.ui auto
  git config --list
<img src="Screenshot from 2021-11-04 20-11-41.png">

2. Creación de repositorio
Podemos crear un repositorio con el siguiente comando que lo llamaremos "dpl".
 mkdir dpl
 cd dpl
 git init
 ls -la
 <img src="Screenshot from 2021-11-04 20-12-17.png">
 
 3.Comprobación del estado actual del repositorio creado
 El primer paso es comprobar el estado del repositorio con "git status".
 El segundo es crear un fichero indice.txt con el siguiente contenido  Capítulo 1: Instalación de Git por el alumno XXX 
 (donde XXX es el nombre del alumno Capítulo 2: Flujo de trabajo básico con con el comando"cat > indice.txt" para guardar "Ctrl+D"
 El tercer paso comprobar de nuevo el estado con " git status".
 El cuarto aÑade el fichero a la zona de intercambio temporal "git add indice.txt".
 Y por último comprobar otra vez el estado "git status".
  <img src="Screenshot from 2021-11-04 20-17-24.png">
  
  4.Realizar un commit
  Insertar un commit de los útlimos cambios realizados aÑadiendo el mensaje "Añadido índice de la asignatura DPL."
  "git commit -m "Añadido índice de la asignatura DPL."
  "git status"
   <img src="Screenshot from 2021-11-03 22-33-38.png">
  
  5.Modificación de ficheros
  Modificar el fichero indice.txt con lo siguiente:"cat > indice.txt"
  
   Capítulo 1: Instalación de Git por el alumno XXX (donde XXX es el nombre del alumno)
   Capítulo 2: Flujo de trabajo básico
   Capítulo 3: Gestión de ramas
   capítulo 4: Repositorios remotos
   "Ctrl+D"
   Mostrar los cambios hechos y hacer un commit de los cambios con el mensaje "Añadido los capitulos 3 y 4."
   "git diff"
   "git add indice.txt"
   "git commit -m "Añadido los capitulos 3"
    <img src="Screenshot from 2021-11-05 16-27-49.png">
   
   6. Historial
   Mostrar cambios de la última versión respecto a la amterios "git show".
   Modificar el último mensaje del commit por "Añadido el capitulo sobre gestión de ramas al índice." con "git commit --amend -m "Añadido 
   el capitulo sobre gestión de ramas al índice."
   volver a mostrar los cambios "git show".
   <img src="Screenshot from 2021-11-05 16-33-04.png">
  


 


 
