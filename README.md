# Curso Git & GitHub

### El archivo README.md trabaja bajo el lenguaje Markdown, para saber mas sobre Markdown podemos ver la guia [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Markdown Cheatsheet")

### 1. Para iniciar un repositorio en un directorio local
```
git init
```
### 2. Para ver el estado actual del repositorio
```
git status
```
### 3. Antes de hacer un commit debemos añadir a stage area
#### Con . nos referimos al directorio actual o podemos especificar los archivos que queramos añadir a stage area 
```
git add . 
```
### 4. Una vez añadidos a stage area podemos hacer un commit 
```
git commit -m "mensaje del commit"
```
### 5. Para subir un repositorio local a GitHub por primera vez
podemos hacerlo por medio de SSH o por HTTPS, en este caso usamos SSH
```
git remote add origin git@github.com:jose-016al/Curso-git.git
git push -u origin master
```