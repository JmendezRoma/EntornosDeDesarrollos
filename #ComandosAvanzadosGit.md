En mi caso realice una clonacion del repositorio remoto ttps://github.com/jpexpositoh/libro mediante los siguientes comando: “git clone https://github.com/jpexposito/libro.git , cd libro”
Ejercicio 1
    • Mostrar el historial de cambios del repositorio.  
      “ git log”
    • Crear la carpeta capítulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto. 
    	Git es un sistema de control de versiones ideado por Linus Torvalds.
      “mkdir capitulos”
	
	  “ cat > capitulos/capitulo1.txt”

    • Añadir los cambios a la zona de intercambio temporal. 
      “git add .”
    
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 1. 
      “git commit -m "Añadido capítulo 1.”
   
   • Volver a mostrar el historial de cambios del repositorio. 
      “git log”
      <img src:"">

Ejercicio 2
    • Crear el fichero capitulo2.txt en la carpeta capítulos con el siguiente texto. 
      " > cat > capitulos/capitulo2.txt"
      "guardar con ctrl+D"
    
El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios.
    • Añadir los cambios a la zona de intercambio temporal.
      "git add ."
    
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 2. 
      "git commit -m "Añadido capítulo 2."
   
   • Mostrar las diferencias entre la última versión y dos versiones anteriores.
      "git diff HEAD~2..HEAD"
      <img src:"">

Ejercicio 3
    • Crear el fichero capitulo3.txt en la carpeta capítulos con el siguiente texto. 
    Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.
    "cat > capitulos/capitulo3.txt"
    "guardar con ctrl+D"
    
    • Añadir los cambios a la zona de intercambio temporal. 
    "git add ."
    
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 3. 
    "git commit -m "Añadido capítulo 3.""
    "git log"
    
    • Mostrar las diferencias entre la primera y la última versión del repositorio. 
    "git diff <codigo hash de la primera version>..HEAD"
    <img src:"">

Ejercicio 4
    • Crea el fichero índice.txt la siguiente línea: 
    Indice de los cápitulos, con conceptos avanzados de git
    "cat > indice.txt"
    
    • Añadir los cambios a la zona de intercambio temporal. 
    "git add ."
    
    • Hacer un commit de los cambios con el mensaje "Indice de los cápitulos, con conceptos avanzados de git. 
     "git commit -m "Se crea el indice."
     "echo "Indice de los cápitulos, con conceptos avanzados de git" >> indice.txt"
     "git add"
     "git commit -m "Añadido el índice ."
    
    • Mostrar quién ha hecho cambios sobre el fichero indice.txt. 
      "git annotate indice.txt"
      <img src:"">

Ejercicio 5
    Crear una nueva rama bibliografía y mostrar las ramas del repositorio.
    "  git branch bibliografia
       git branch -av"
       <img src:"">

Ejercicio 6
    • Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente: 
    En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.
    "cat > capitulos/capitulo4.txt"
    "ctrl+D" para guardar cambios.
    
    • Añadir los cambios a la zona de intercambio temporal.
    "git add"
    • Hacer un commit con el mensaje “Añadido capítulo 4.” 
    "git commit -m "Añadido capítulo 4."
    
    • Mostrar la historia del repositorio incluyendo todas las ramas. 
    "git log --graph --all --oneline"

Ejercicio 7
    • Cambiar a la rama bibliografía. 
    • Crear el fichero bibliografia.txt y añadir la siguiente referencia: 
      Chacon, S. and Straub, B. Pro Git. Apress.
    • Añadir los cambios a la zona de intercambio temporal. 
    • Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.” 
    • Mostrar la historia del repositorio incluyendo todas las ramas. 

Ejercicio 8
    • Fusionar la rama bibliografía con la rama main. 
    • Mostrar la historia del repositorio incluyendo todas las ramas. 
    • Eliminar la rama bibliografía. 
    • Mostrar de nuevo la historia del repositorio incluyendo todas las ramas. 

Ejercicio 9
    • Crear la rama bibliografía. 
    • Cambiar a la rama bibliografía. 
    • Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias: 
Scott Chacon and Ben Straub. Pro Git. Apress.
Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014)
    • Cambiar a la rama main. 
    • Cambiar el fichero bibliografia.txt para que - contenga las siguientes referencias: 
Chacon, S. and Straub, B. Pro Git. Apress.
Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.
    • Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.” 
    • Fusionar la rama bibliografía con la rama main. 
    • Resolver el conflicto dejando el fichero bibliografia.txt con las referencias: 
Chacon, S. and Straub, B. Pro Git. Apress.
Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.
Hodson, R. Ry’s Git Tutorial. Smashwords (2014)
    • Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.” 
    • Mostrar la historia del repositorio incluyendo todas las ramas. 
