## ¿EN QUE ORGANISMO/GRUPO DE ORGANISMOS VAS A TRABAJAR?
Mariposas (Lepidoptera), en la familia Riodinidae, conocidas por una amplia
diversidad de patrones de coloracion


## BREVEMENTE DESCRIBE QUE PIENSAS HACER EN TU PROYECTO
Mi ptoyecto busca analizar como el color de las mariposas  este grupo cambia
cambia dependiendo del clima. Analizanod datos para ver si existe relacion entre
color y ambiente


## PROGRAMAS
R
IQ-TREE
FigTree
ImageJ
Python


## FOTO DEL ORGANISMO 
![alt text]https://upload.wikimedia.org/wikipedia/commons/c/c4/Brauner_W%C3%BCrfelfalter_%28Hamearis_lucina%29_02.jpg

##NOMBRE DE TU PROYECTO
Coloracion de las mariposas frente al ambiente

##AUTORES DEL PROYECTO
Mikaela Pavon-Naranjo

##PROPOSITO DEL PROGRAMA DE TU PROYECTO
El proyecto busca el analizar los efectos del ambiente sobre el color que expresan las mariposas.Se usarán árboles filogenéticos, datos de distribución geográfica y análisis de imágenes para detectar patrones de adaptación del color en relación con el clima.
El analisis puede ayudar a entender cómo las especies responden a diferentes ambientes y si determiados patrones o colores proveen de ventaja para el individuo bajo distintas condiciones ambientales.

##REQUISITOS PARA EJECUTAR EL PROGRAMA
-Tener descargado R con los siguientes programas: ggplot2, vegan y ape (De análisis filogenético)
-Python 
-IQ-TREE
-FigTree
-ImageJ (Análisis de color)


##COMO USAR EL PROGRAMA
#DATOS
Fotografías para el análisis en una carpeta en formato .jpg
Archivo .tree de la filogenia de la familia Riodinidae en fortmato fasta

#RSTUDIO
$library(ape)
$tree <- read.tree ("Filogenia Riodinidae.tree")}
$library(ggplot2)
$plot(tree)

##FigTree/IQ-TREE
Descargar el archivo con la filogenia y abrirlo en FigTree
File
Open
Escoger formato fasta

