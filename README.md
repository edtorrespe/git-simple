# Git

[Ebook Pro Git en español](https://git-scm.com/book/es/v2)

## Configuración de Git

```bash
# Configuración global
git config --global user.name "<nombre-usuario>"
git config --global user.email "<nombre-email>"
git config --global core.editor <vim>
git config --global core.autocrlf true

# Mostrar el nombre del usuario actual
git config user.name

# Mostrar email del usuario actual
git config user.email
```

## Inicializar repositorio Git

```bash
# Inicializar un proyecto Git
git init

# Ver el estado del proyecto Git
git status

# Agregar un archivo al proyecto Git
git add <nombre-archivo>

# Agregar todos los archivos al proyecto Git
git add .

# Crear un commit para guardar los cambios al proyecto Git
git commit -m "Mensaje del commit"

# Agregar todos los archivos al proyecto de Git y crear un commit para guardar los cambios. 
git commit -a -m "Mensaje del commit"
```

## Archivo .gitignore

* Crear un archivo con el nombre ``.gitignore``
* Dentro del archivo ``.gitignore`` escribiras los archivos o ficheros que serán ignorados por Git

## Ver historial de cambios

```bash
# Mostrar el historial (lista de commits)
git log

# Mostrar la primera línea del historial
git log --oneline

# Mostrar el historial completo
git log --all

# Mostrar la primera línea del historial completo
git log --all --oneline

# Mostrar la primera línea del historial completo, mostrando el nombre de la rama, y el gráfico del historial
git log --all --oneline --decorate --graph

# Ir a un cambio especifico del historial
git checkout <nombre-id>

# Ir a los cambios de la rama master
git checkout master
```

## Ramas en Git

```bash
# Muestra las ramas de tu repositorio
git branch

# Crear una nueva rama
git branch <nombre-rama>

# Cambiar a una rama especifíca
git checkout <nombre-rama>

# Llevar los cambios de una rama a la rama donde te encuentras
git merge <nombre-rama>

# Eliminar una rama, si no se hizo un merge git dará un aviso
git branch -d <nombre-rama>

# Forzar la eliminar de una rama
git branch -D
```

## Repositorio remoto con Github

```bash
git remote add origin https://github.com/<nombre-usuario>/<nombre-repositorio>.git
git push -u origin master

git push origin master
git pull origin master

git remote -v
git branch -a
```