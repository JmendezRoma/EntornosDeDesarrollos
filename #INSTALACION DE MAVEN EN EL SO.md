INSTALACION DE MAVEN EN EL SO
JONATHAN JOEL MENDEZ ROMANELLI
1ºDAW


Para instalar la herramienta maven la cual nos puede servir como compresor y gestor de archivos java, tenemos que seguir los siguientes pasos:

1)INSTALAR APACHE MAVEN CON APT:
Usaremos el siguiente comando “ sudo apt update” para actualizar el indice y luego tecleamos “ sudo apt install maven” para instalar maven. <br>

<img src="Screenshot from 2021-09-29 20-04-33.png">

Verificamos la version con “ mvn -version” <br>
La terminal nos muestra que hemos instalado correctamente la version de maven 3,6,3 <br>
<img src="Screenshot from 2021-09-29 20-04-53.png">


2)INSTALAR VERSION PARTICULAR DE APACHE MAVEN <br>
Primero he comprobado que efectivamente la ultima version de maven es la 3.8.2 .



Luego hay que descargar el maven en el directorio con el siguiente comando “wget https://www.apache.org/dist/maven/maven-3/3.8.2/binaries/apache-maven-3.8.2-bin.tar.gz -P /tmp”
para posteriormente extraer el archivo en el directorio /opt  “sudo tar xf /tmp/apache-maven-*.tar.gz -C /opt” .
Para tener mas control sobre las versiones nos centramos en el directorio de instalación de maven según la version que queremos aplicar “sudo ln -s /opt/apache-maven-3.8.2 /opt/maven” .
3)ESTABLECER VARIABLES DE ENTORNO <br>
Pondremos el siguiente comando : “sudo nano /etc/profile.d/maven.sh” y tendremos que pegar el siguiente código en la terminal :<br>
   export M2_HOME=/opt/maven<br>
 export MAVEN_HOME=/opt/maven<br>
 export PATH=${M2_HOME}/bin:${PATH}<br>
 Guardamos y cerramos el archivo.<br>
Para que lo que acabamos d hacer sea funcional con chmod usamos “ sudo chmod +x /etc/profile.d/maven.sh”  y finalmente cargamos las variables “source /etc/profile.d/maven.sh”<br>


4)VERIFICACION DE LA VERSION <br>
Para comprobar que tenemos la versión que necesitamos probamos con “ mvn -version”<br>
<img src="Screenshot from 2021-09-29 20-12-24.png">


 




