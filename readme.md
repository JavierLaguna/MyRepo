# Práctica Git

### Javier Laguna

#### ¿Qué comando utilizaste en el paso 11? ¿Por qué?

> git reset --hard HEAD~1

Con el comando `reset` al lugar que le indicamos, en este caso `HEAD~1` que es el commit padre. Y con `--hard` descartamos los cambios del working copy

#### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

> git reflog

> git reset --hard 54c4e67

Primero hacemos `reflog` para buscar el identificador del commit al que queremos volver, una vez localizado lo copiamos y hacemos `git reset --hard [commitID]` en este caso el id del commit es `54c4e67` y con ello volvemos a ese commit

#### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

> git merge master

No se produce ningún conflicto ni cambio porque la rama `styled` ya tiene todos los cambios de `master`

#### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

> git merge htmlify

Si hay conflicto debido a que ambas ramas han modificado las mismas líneas del archivo `git-nuestro.md`

#### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

> git merge styled

En la rama `styled` solo tiene añadidos sobre `master` y por lo tanto se produce un merge fast-forward sin ningún conflicto

#### ¿Qué comando o comandos utilizaste en el paso 25?

> git log --graph


#### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

> git merge --no-ff title

Podría ser fast-forward porque en la rama `title` solo hay añadidos sobre `master`

#### ¿Qué comando o comandos utilizaste en el paso 27?

> git reset HEAD~1

Con el comando `reset` al lugar que le indicamos, en este caso `HEAD~1` que es el commit padre.

#### ¿Qué comando o comandos utilizaste en el paso 28?

> git checkout -- .

Para descartar todos los cambios del working copy

#### ¿Qué comando o comandos utilizaste en el paso 29?

> git branch -D title

Aplicamos `-D` al comando para indicarle que es un borrado

#### ¿Qué comando o comandos utilizaste en el paso 30?

> git reset --hard HEAD@{1}

Ya que deshacer el commit ha sido la última operación que hemos realizado y nos hemos movido de commit

#### ¿Qué comando o comandos usaste en el paso 32?

> git reflog
> 
> git reset 7140c14

Primero hacemos `reflog` para buscar el identificador del commit al que queremos volver, una vez localizado lo copiamos y hacemos `git reset [commitID]` en este caso el id del commit es `7140c14 ` y con ello volvemos a ese commit

#### ¿Qué comando o comandos usaste en el punto 33?

> git reset HEAD@{1}

Ya que el estado final, cuando pusimos título al poema fue el último commit en el que estuvimos previamente