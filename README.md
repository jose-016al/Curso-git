# Git ![Git](./img/git.png)

# Tabla de contenidos
- [Git](#git)
  - [Identificacion en Git](#identificacion-en-git)
  - [Stage area](#stage-area)
  - [Commits](#commits)
- [Github](#github)
  - [Subir repositorio](#subir-repositorio)
  - [Clonar repositorio](#clonar-repositorio)
  - [Ramas](#ramas)

# Git
Inicializar un repositorio Git en local, se crea una carpeta y una vez dentro de la carpeta 
```bash
git init 
```

## Identificacion en Git
Nos identificamos en Git, este nombre y email seran nuestras credenciales en GitHub
```bash
git config --global user.email "you@example.com"
```
```bash
git config --global user.name "Your Name"
```

## Stage area
Ver como esta actualmente nuestro repositorio
```bash
git status
```
Pasar ficheros a stage area
```bash
git add index.html
```
```bash
git rm index.html
```
Recuperar archivos borrados 
```bash
git restore index.html
```

## Commits
Hacer un commit
```bash
git commit -m "Add index.html"
```
Ver todos los commits de un repositorio
```bash
git log
```
```bash
git log --oneline
```
Podemos movernos entre distintas versiones de commits
```bash
git checkout bd59bb 
```
Para volver a donde estabamos y poder seguir hacienod cambios, accedemos al nombre de la rama, en este caso master
```bash
git checkout master
```
Para trabajarcon un commit anterior eliminando los anteriores commit 
```bash
git reset bd59bb
```
Con la opcion "--hard" perdemos todo lo que hayamos hecho hasta ese commit 
```bash
git reset --hard bd59bb
```

# GitHub

## Subir repositorio
Generemos las claves SSH a traves de **[Github](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent), una vez generada debemos añadirla a nuestro perfil de github
```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```
Subimos repositorio a github
```bash
git remote add origin git@github.com:jose-016al/Git.git
```
```bash
git push -u origin master
```

## Clonar repositorio
Clonamos un repositorio subido a github
```bash
git clone git@github.com:jose-016al/Git.git
```
bajar las ultimas modificaciones 
```bash
git pull
```

## Ramas
Creacion de una rama y no cambia de rama directamente
```bash
git checkout -b feature-post-styles
```
Ver todas las ramas disponibles
```bash
git branch
```
Cuando creamos una rama debemos crearla tambien en el remoto, es decir en github 
```bash
git push -u origin feature-post-styles
```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```
```bash

```


### El archivo README.md trabaja bajo el lenguaje Markdown, para saber mas sobre Markdown podemos ver la guia [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Markdown Cheatsheet")

