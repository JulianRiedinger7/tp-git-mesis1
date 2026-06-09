# Git Add

## ¿Qué es?

`git add` es un comando que se utiliza para preparar archivos antes de realizar un commit. Permite indicar qué cambios serán incluidos en el próximo registro del historial.

## Sintaxis

```bash
git add <archivo>
```

o para agregar todos los cambios:

```bash
git add .
```

## ¿Qué hace?

Cuando se modifica, crea o elimina un archivo, Git detecta esos cambios pero todavía no los incluye en el próximo commit. Al ejecutar `git add`, los cambios seleccionados pasan al área de preparación (*staging area*), donde quedan listos para ser confirmados mediante un commit.

## Ejemplo de uso

```bash
git add README.md
```

Este comando agrega únicamente el archivo `README.md` al área de preparación.

```bash
git add .
```

Este comando agrega todos los cambios realizados en el directorio actual y sus subdirectorios.

## ¿Cuándo se utiliza?

Se utiliza después de realizar modificaciones en los archivos y antes de ejecutar `git commit`, para indicar exactamente qué cambios se desean guardar en el historial del repositorio.
