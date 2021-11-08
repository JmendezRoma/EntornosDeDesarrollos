En mi caso realice una clonacion del repositorio remoto ttps://github.com/jpexpositoh/libro mediante los siguientes comando: “git 
clone https://github.com/jpexposito/libro.git , cd libro”<br>
<img src = "Screenshot from 2021-11-08 14-54-24.png">

Ejercicio 1 <br>
    • Mostrar el historial de cambios del repositorio.  <br>
      “ git log”<br>
    • Crear la carpeta capítulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto. <br>
    	Git es un sistema de control de versiones ideado por Linus Torvalds.<br>
      “mkdir capitulos”<br>

“ cat > capitulos/capitulo1.txt” <br>

   • Añadir los cambios a la zona de intercambio temporal. <br>
      “git add .”<br>
    
   • Hacer un commit de los cambios con el mensaje Añadido capítulo 1. <br>
      “git commit -m "Añadido capítulo 1.”<br>
   
  • Volver a mostrar el historial de cambios del repositorio. <br>
      “git log”<br>
      <img src="Screenshot from 2021-11-08 14-54-58.png"><br>

Ejercicio 2<br>
   • Crear el fichero capitulo2.txt en la carpeta capítulos con el siguiente texto. <br>
     " > cat > capitulos/capitulo2.txt"<br>
     "guardar con ctrl+D"<br>
    
El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal.
3- Hacer un commit de los cambios.<br>
  • Añadir los cambios a la zona de intercambio temporal.<br>
     "git add ."<br>
    
  • Hacer un commit de los cambios con el mensaje Añadido capítulo 2. <br>
     "git commit -m "Añadido capítulo 2."<br>
   
  • Mostrar las diferencias entre la última versión y dos versiones anteriores.<br>
     "git diff HEAD~2..HEAD"<br>
      <img src=" Screenshot from 2021-11-08 15-08-04.png"><br>

Ejercicio 3<br>
    • Crear el fichero capitulo3.txt en la carpeta capítulos con el siguiente texto. <br>
    Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.<br>
    "cat > capitulos/capitulo3.txt"<br>
    "guardar con ctrl+D"<br>
    
   • Añadir los cambios a la zona de intercambio temporal. <br>
    "git add ."<br>
    
   • Hacer un commit de los cambios con el mensaje Añadido capítulo 3. <br>
    "git commit -m "Añadido capítulo 3.""<br>
    "git log"<br>
    
   • Mostrar las diferencias entre la primera y la última versión del repositorio. <br>
    "git diff <codigo hash de la primera version>..HEAD"<br>
    <img src="Screenshot from 2021-11-08 15-11-34.png"><br>

Ejercicio 4<br>
   • Crea el fichero índice.txt la siguiente línea: <br>
    Indice de los cápitulos, con conceptos avanzados de git<br>
    "cat > indice.txt"<br>
    
   • Añadir los cambios a la zona de intercambio temporal. <br>
    "git add ."<br>
    
   • Hacer un commit de los cambios con el mensaje "Indice de los cápitulos, con conceptos avanzados de git. <br>
     "git commit -m "Se crea el indice."<br>
     "echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt"<br>
     "git add"<br>
     "git commit -m "Añadido el índice ."<br>
    
   • Mostrar quién ha hecho cambios sobre el fichero indice.txt. <br>
      "git annotate indice.txt"<br>
      <img src= "Screenshot from 2021-11-08 15-25-36.png"><br>

Ejercicio 5<br>
    Crear una nueva rama bibliografía y mostrar las ramas del repositorio.<br>
    "  git branch bibliografia<br>
       git branch -av"<br>
       <img src="Screenshot from 2021-11-08 15-30-58.png"><br>

Ejercicio 6<br>
   • Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente: <br>
    En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.<br>
    "cat > capitulos/capitulo4.txt"<br>
    "ctrl+D" para guardar cambios.<br>
    
   • Añadir los cambios a la zona de intercambio temporal.<br>
    "git add"<br>
   • Hacer un commit con el mensaje “Añadido capítulo 4.” <br>
    "git commit -m "Añadido capítulo 4."<br>
    
   • Mostrar la historia del repositorio incluyendo todas las ramas. <br>
    "git log --graph --all --oneline"<br>
    <img src="Screenshot from 2021-11-08 15-32-52.png"><br>

Ejercicio 7<br>
   • Cambiar a la rama bibliografía.<br>
    " git checkout bibliografia"<br>
    
   • Crear el fichero bibliografia.txt y añadir la siguiente referencia: <br>
      Chacon, S. and Straub, B. Pro Git. Apress.<br>
      "cat > bibliografia.txt<br>
      Chacon, S. and Straub, B. Pro Git. Apress."<br>
	"Ctrl+D" para guardar los cambios.<br>

   • Añadir los cambios a la zona de intercambio temporal. <br>
    	"git add ."<br>
    
   • Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.” <br>
    "git commit -m "Añadida primera referencia bibliográfica."<br>
    
   • Mostrar la historia del repositorio incluyendo todas las ramas. <br>
    "git log --graph --all --oneline"<br>
    <img src="Screenshot from 2021-11-08 15-36-00.png"><br>

Ejercicio 8<br>
   • Fusionar la rama bibliografía con la rama main. <br>
    "git checkout main"<br>
    "git merge bibliografia"<br>
    
   • Mostrar la historia del repositorio incluyendo todas las ramas. <br>
    "git log --graph --all --oneline"<br>
   • Eliminar la rama bibliografía. <br>
    "git branch D- bibliografia"<br>
   • Mostrar de nuevo la historia del repositorio incluyendo todas las ramas. <br>
    "git log --graph --all --oneline"<br>
    <img src="Screenshot from 2021-11-08 15-46-41.png"><br>

Ejercicio 9<br>
   • Crear la rama bibliografía. <br>
    "git branch bibliografia"<br>
    
   • Cambiar a la rama bibliografía. <br>
    "git checkout bibliografia"<br>
    
   • Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias: <br>
	Scott Chacon and Ben Straub. Pro Git. Apress.<br>
	Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014)<br>
	" cat > bibliografia.txt "<br>
	"Crtl+D" para guardar<br>
    
   •Cambiar a la rama main. <br>
    "git checkout main"<br>
    
   • Cambiar el fichero bibliografia.txt para que - contenga las siguientes referencias: <br>
	Chacon, S. and Straub, B. Pro Git. Apress.<br>
	Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.<br>
	"cat > bibliografia.txt"<br>
	
   • Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia 	bibliográfica.” <br>
    "git commit -a -m "Añadida nueva referencia bibliográfica.""<br>
   
  • Fusionar la rama bibliografía con la rama main. <br>
   "git merge bibliografia"<br>
   
  • Resolver el conflicto dejando el fichero bibliografia.txt con las referencias: <br>
	Chacon, S. and Straub, B. Pro Git. Apress.<br>
	Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.<br>
	Hodson, R. Ry’s Git Tutorial. Smashwords (2014)<br>
	"git nano bibliografia"<br>
	"cat > bibliografia.txt"<br>
    
   • Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.” <br>
    " git commit -a -m "Solucionado conflicto bibliografía."<br>
    
   
   • Mostrar la historia del repositorio incluyendo todas las ramas. <br>
    "git log --graph --all --oneline"<br>
    <img src= "Screenshot from 2021-11-08 15-46-41.png"><br>
