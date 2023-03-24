# GIT
- Un sistema de control de versiones

### COMANDOS DE GIT

```
git --version

git config --global user.name "jefry"
git config --global user.email "jefrydep@gmail.com"
git config --global -e (comando para configurar) - wq!
git help
git config
git init 
git status
git add .
git reset nombreDelarchivoa_resetear
git config core.autocrlf true (para eliminar el warnig CRLF)
git checkout -- . (reconstruye los proyectos hasta el ultimo commit)
git branch (ver las ramas)
git config --global init.defaultBranch main(para cambiar la rama master por main de manera global)
git commit -am "readme actualizado" (da seguimiento a los archivos añadidos)
git log (para ver todos los commits)
git reset (poner nombre de los archivos para bajarlos del stage)
git add *.html (agrega todos los archivo html al stage del root)
git add js/*.js (agrega todos las extensiones js de la carpeta js)   
git add css/ (agrega todos los archivos que se encuentren dentro de css)
git config --global alias.s "status --short"(para ponerle un alias a nuestro comando )
git log --oneline
git diff
git commit --amend -m (actualizando el ultimo commit)
git reset --soft HEAD^
git reset --soft (AQUI COLOCAMOS EL ID DEL COMMIT PARA MODIFICARLO)
git reset --mixed (id del commit)
git reflog (muestra todos los comandos de git ulitlzados par volver en el tiempo)
git reset --hard (id del commit)
git rm (nombre del archivo a elimianr)

git pull
git push


```
1. para configurar nuestro alias de log
```
git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"
```

## Trabajando con ramas en git

```
git ckeckout -b "nombre dela rama"
git branch
git merge (nombre de la rama de donde se va hacer el merge)
git branch -d (eliminar las ramas que ya no necesitamos) -f
git branch -a (para ver las ramas remotas)
git remote prune origin(para elminar ramas del local)
```
## Tags

- hace referencia de un commit en un punto especifico y luego descargarlo 
```
git tag super-release
git tag -d (nombre del tag a eliminar)
git tag -a v1.0.0 -m "new vwersion read"
git tag -a v1.0.0 -m jf12kds "un tag con el id commit"
git show v0.1.0 (para ver el tag)
git push --tags (para subir los tags al repositorio)
crear un release
```

#### git Stash
1. separa un espacio en memoria con todos los archivos 
```
git stash
git stash list
git stash drop 
git stash show stash@{1}
git stash save "aqui el nmbre del stash"
git stash pop (recupera el ultimo stash y lo elimina)
git stash clear 

```
##### Git rebase

```
git rebase main
git rebase -i HEAD-4
squash 
reword
git checkout -- README.MD 
```


## Git hup


```                                                                                                                                                                                                                                                                                                                                                                     
git remote add origin "link"
git push -u origin master
git pull 



```
### Forks 


* este comando nos sirven para crear un repositorio princi
```
git remote add upstream (aqui ponemos el link del respisitorio)
git remote -v
git pull upstream (nombre de la rama que deseas pulear)
```