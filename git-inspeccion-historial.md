# Comandos de GIT relacionados a la inspeccion del historial

## **git log**

Es el comando mas basico para obtener informacion del historial de cambios. Nos muestra cada commit con su **hash** respectivo, asi como tambien el autor, la fecha y el comentario.

Ademas, tambien especifica donde nos encontramos parados actualmente, es decir donde se encuentra el **HEAD**.

Podemos usar el flag **--oneline** que nos muestra unicamente cada commit con un hash de 7 digitos y el comentario.

## **git reflog**

Este comando nos muestra cuando el **HEAD** cambia, por lo que observamos informacion no solo de commits, sino tambien de otras acciones como **checkouts**, **merges**, **conflicts**, que no son necesariamente escribir codigo.

---

_Con ambos de estos comandos, podemos observar mucha informacion de los commits, pero no sabemos exactamente los cambios que se realizaron_

## **git show**

Este comando nos permite inspeccionar un **commit** especifico. Debemos pasarle el hash respectivo de ese commit (obtenido con los comandos previos) y obtenemos informacion de lo que cambió durante el mismo.

## **git diff**

Este comando se utiliza para comparar y saber que **diferencias** hubo entre 2 commits. Si se utiliza para comparar un commit con el que se encuentra justo antes, no hay diferencia a usar **git show**, pero su utilidad se ve cuando queremos comparar commits que se encuentran mas alejados entre si.

Solo debemos pasarle el **hash** del primer commit, y luego el **hash** del segundo commit, y obtenemos informacion de la diferencia.
Tambien es muy util para pasarle el **HEAD**, es decir para ver la diferencia de un commit con la actualidad (esto es lo mismo que pasar un solo **hash**).

Si solo queremos ver que archivos se modificaron, y cuantas lineas se agregaron/eliminaron, podemos pasar el flag **--stat** al final.

Por ultimo, tambien podemos comparar entre ramas utilizando el **..**, por ejemplo **git diff main..feature/setup**
