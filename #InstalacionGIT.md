<h1>Tarea 1: Instalación de Git en linux</h1>
  
  
  JONATHAN MÉNDEZ ROMANELLI
  
  
  
  Git es una herramienta para desarrolladores la cual permite un control claro y robusto en el tratamiento del codigo<br>
  Para empezar necesitaremos tener incorporado a nuestro sistema linux un servidor propio al mismo y<br>
  también tener instalado la version 20.04 de Ubuntu.<br>
  
  Comprobamos que posiblemente no tengamos preinstalada una versión de alguna libreria propia de linux, <b>
  con el comando "git --version".<br>
  
  De no ser así tenemos dos posibilidades a la hora de afrontar la instalacion: *Directamente desde los comando <br>
  y librerias de serie de linux mediante los siguiente comandos,"sudo apt update" (para actualizar el sistema),<br>
  "sudo apt install git"(para instalar git), y por último" git --version" para comprobar de nuevo la version <br>
  resultando en esta específicamente git version 2.25.1.<br>
  *La otra vía de instalación seria a traves de la fuente.<br>
  
  1) Actualizar nuestro índice de paquetes e instalar los correspondientes mediante el comando :"sudo apt update <br>
sudo apt install libz-dev libssl-dev libcurl4-gnutls-dev libexpat1-dev gettext cmake gcc".<br>
  <img src="Screenshot from 2021-11-03 22-33-38.png">
  
  2)Creacion de un directorio temporal : "mkdir tmp , cd /tmp".
  <img src="Screenshot from 2021-11-03 22-41-54.png">
  
  3)Instalar curl.
  <img src="Screenshot from 2021-11-03 22-41-54.png">.
  
  4)Descarga de versión exacta que queramos instalar de git e incporarla en el directorio establecido.
  enlace para la descarga de version:  https://mirrors.edge.kernel.org/pub/software/scm/git/ 
  
  5)A través de este comando "curl -o git.tar.gz https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.29.3.tar.gz"
  
  6) Descomprimimos el archivo con :"tar -zxf git.tar.gz"
  <img src ="Screenshot from 2021-11-03 22-42-57.png">
  
  7)Creamos directorio git :"cd git-*"
  
  8)Creación de paquete e instalación :"make prefix=/usr/local all
  sudo make prefix=/usr/local install"
  
  9)sustitución de proceso de shell:" exec bash".
  <img src="Screenshot from 2021-11-03 22-48-38.png>
            
  10)Comprobamos version 2.29.3 :"git --version "
                                                 
  Ahora solo tenemos que configurarlo:
   1) Utilizaremos este comando y deberemos insertar nuestros datos (email y nombre).
   <img src="Screenshot from 2021-11-03 22-48-38.png>
  
  2)Para acceder a nuestro archivo git utilizaremos este comando :"nano ~/.gitconfig".
  <img src ="Screenshot from 2021-11-03 22-49-05.png">
 
  
  
  
  

  

