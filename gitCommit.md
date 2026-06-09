# Git Commit

## ¿Qué es?

`git commit` es un comando que se utiliza para guardar de forma permanente los cambios que fueron preparados previamente con `git add`. Cada commit representa un punto en el historial del proyecto.

## Sintaxis

```bash id="a8k2qp"
git commit -m "mensaje del commit"
```

## ¿Qué hace?

Cuando se ejecuta `git commit`, Git toma todos los cambios que están en el área de preparación (*staging area*) y los guarda en el historial del repositorio. A cada commit se le asigna un identificador único (hash), lo que permite volver a ese estado del proyecto en cualquier momento.

## Ejemplo de uso

```bash id="q1m8dd"
git add archivo.txt
git commit -m "feat: agregar archivo de texto"
```

En este caso, primero se agregan los cambios al área de preparación y luego se guarda una nueva versión del proyecto en el historial.

## ¿Por qué es importante?

* Permite llevar un registro ordenado de los cambios.
* Facilita volver a versiones anteriores del proyecto.
* Ayuda a trabajar en equipo sin perder modificaciones.
* Cada commit representa un “punto de guardado” del proyecto.
