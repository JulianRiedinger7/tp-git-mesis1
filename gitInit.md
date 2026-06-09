# Git Init

## ¿Qué es?

`git init` es un comando que se utiliza para crear un nuevo repositorio Git en una carpeta. Al ejecutarlo, Git comienza a realizar el seguimiento de los archivos del proyecto y genera la estructura necesaria para gestionar versiones.

## Sintaxis

```bash
git init
```

## ¿Qué hace?

Cuando se ejecuta `git init`, Git crea una carpeta oculta llamada `.git` dentro del directorio actual. Esta carpeta contiene toda la información necesaria para almacenar el historial de cambios, las ramas, la configuración del repositorio y otros datos utilizados por Git.

## Ejemplo de uso

```bash
mkdir mi-proyecto
cd mi-proyecto
git init
```

Luego de ejecutar el comando, la carpeta `mi-proyecto` quedará configurada como un repositorio Git.

## ¿Cuándo se utiliza?

Se utiliza al comenzar un proyecto nuevo que aún no está siendo gestionado por Git y se desea empezar a controlar las versiones de sus archivos.
