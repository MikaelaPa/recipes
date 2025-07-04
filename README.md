## ¿EN QUE ORGANISMO/GRUPO DE ORGANISMOS VAS A TRABAJAR?
Mariposas (Lepidoptera), en la familia Riodinidae, conocidas por una amplia
diversidad de patrones de coloracion


## BREVEMENTE DESCRIBE QUE PIENSAS HACER EN TU PROYECTO
Generar un árbol filogenético que represente las relaciones evolutivas dentro de Riodinidae, usando datos moleculares, para clarificar la sistemática y evolución de dicho grupo.


## PROGRAMAS
* R
* IQ-TREE
* FigTree
* Muscle


## FOTO DEL ORGANISMO 
![alt text](https://upload.wikimedia.org/wikipedia/commons/c/c4/Brauner_W%C3%BCrfelfalter_%28Hamearis_lucina%29_02.jpg)

## NOMBRE DE TU PROYECTO
Reconstrucción filogenética de la familia Riodinidae

## AUTORES DEL PROYECTO
Mikaela Pavon-Naranjo

## PROPOSITO DEL PROGRAMA DE TU PROYECTO
El proyecto busca la reconstrucción y análisis de la filogenia de la familia Riodinidae basandonos en datos moleculares. Esto nos facilitará el conocer cómo se relacionan entre sí los diversos grupos de mariposas y las especies en ellos. Además de que nos ayudará a saber si los grupos forman un único conjunto de descendientes comunes y conocer su distribución según el lugar del que se originan.

## REQUISITOS PARA EJECUTAR EL PROGRAMA
* Descargarnos secuencias de ADN de las especies de Riodinidae en formato FASTA
* Tener descargado R con los siguientes programas: ggplot2, vegan y ape (De análisis filogenético)
* IQ-TREE para realizar el árbol filogenético
* FigTree para editar los árboles



# COMO USAR EL PROGRAMA
## DATOS
* Descargar secuencias de ADN en formato FASTA
* Alinear las secuencias con Muscle

## IQTREE
* Subir archivo de Muscle
* Ejecutar análisis para ver el mejor modelo
* Recontrucción del árbol de máxima verosimilitud

## FigTree
* Abrir archivo de IQTREE
* Interpretar

## R
* Importar árbol con paquete "ape"
* Análisis de distancias

# SCRIPT
* Descargar secuencias: esearch -db nucleotide -query "Riodinidae[Organism] AND COI" | efetch -format fasta > Riodinidae_COI.fasta
* Alineamiento: ./muscle3.8.31_i86linux64 -in Riodinidae_COI.fasta -out muscle_Riodinidae_COI.fasta -maxiters 1 -diags
* IQ-tree: module load iqtree/2.2.2.6
* for filename in musscle_*
> do
> iqtree2 -s $filename
> done 
* En una nueva ventana, fuera de Hoffman2 y en mi escritorio descargo el output:  scp dechavez@hoffman2.idre.ucla.edu:/u/scratch/d/dechavez/Bioinformatica-PUCE/RediseBio/MikaelaPa/(OUTPUT DE IQTREE) .
* Abro figtree → File → Abro concord.cf.tree → Acepto lo que dice label

