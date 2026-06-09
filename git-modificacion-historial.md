# Comandos de GIT relacionados a la modificacion del historial

## **git checkout**

Se utiliza para cambiar a otro punto en el tiempo del repositorio. Es comun utilizarlo con ramas ya que estas tambien son otro punto en el tiempo del repositorio.

Pero ademas de sus funciones relaciondas con el cambio/creacion de ramas, tambien lo podemos utilizar para regresar a un estado previo del repositorio pasandole el **hash** respectivo del commit.

Por ejemplo: **_git checkout 06b7383_**

Esto nos deja en un estado de **detached HEAD**, donde el mismo GIT nos advierte que es un modo de solo 'lectura', donde cualquier cambio que hagamos se va a perder.

Para volver nuevamente al presente del repositorio utilizamos: **_git checkout -_**

## **git reset**

Usamos este comando cuando queremos volver en el tiempo, pero no solo en modo 'lectura' como el **checkout**, sino con la posibilidad de hacer cambios.

### **git reset --soft**

Si utilizamos este flag a la hora de volver atras, todos los cambios posteriores siguen estando, no se pierden. Los commits no se observan, pero si los cambios respectivos.

### **git reset --hard**

A diferencia del **--soft**, pasando este nuevo flag a la hora de volver atras, todos los cambios posteriores SI se pierden. No solo cambia la historia si no que borra cambios.

Si queremos revertir esto, tenemos que usar el comando de inspeccion **git reflog** donde se guardan todas las referencias, incluyendo commits perdidos. Luego usamos el **git reset --hard** pasando dicha referencia.

## **git revert**

Este comando se utiliza para volver atras, pero sin cambiar la historia. En lugar de volver atras directamente, se crea un **commit** que vuelve atras.

Hay que tener en cuenta que los commits, incluyendo el del **revert**, puede generar conflictos.
