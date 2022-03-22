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
### 5. Para consultar los commits realizados a un repositorio 
```
git log --oneline
```
### 6. Para movernos entre commits y ramas
```
git checkout 3d9dffe
```
### 7. Para subir un repositorio local a GitHub por primera vez
podemos hacerlo por medio de SSH o por HTTPS, en este caso usamos SSH
```
git remote add origin git@github.com:jose-016al/Curso-git.git
git push -u origin master
```
### 8. Para subir los ultimos cambios a GitHub 
```
git push
```
### 9. Para bajar los ultimos cambios realizados en el repositorio
```
git pull
```
### 10. Para clonar un repositorio de GitHub 
Se puede clonar por medio de HTTPS y por medio de SSH
```
git clone git@github.com:jose-016al/Curso-git.git
```
### 11. Crear una nueva rama
```
git checkout -b feature-posts-styles
```
### 12. Para ver las ramas de un repositorio
```
git branch
```
### 13. Para mezclar una rama con otra
```
git merge feature-posts-styles
```