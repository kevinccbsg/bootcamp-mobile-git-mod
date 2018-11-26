
# Bootcamp mobile git module

### ¿Qué comando utilizaste en el paso 11? ¿Por qué?

`git reset HEAD~1 --hard`

Porque con `git reset HEAD~1` movemos el putero de la rama styled y el puntero HEAD un commit atras en el grafo. Además, al añadir el flag --hard descartamos los cambios que quedarían en el working copy.

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

`git reflog`

Este comando lo uso para recuperar el identificador del commit que en mi caso es b4404a8. Con lo que luego puedo hacer:

`git reset b4404a8 --hard`

Es decir muevo el puntero de mi rama styled además de head a dicho commit recuperandolo. El --hard para añadirlo al repo sin tener que hacer el proceso de añadirlo al staging area y luego al repo.

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, se produce un Already up-to-date ya que el commit de styled es posterior y el contenido de master ya lo tenia en su primer commit por lo que al estar más avanzado en el grafo está ya actualizado.

### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

Si, hay conflictos. Porque en ambas ramas se modificaron las mismas lineas del archivo git-nuestro.md provocando conflicto. Unas con los caracteres de markdown y la otra con los de html

### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

No, no ha habido conflicto ya que el puntero de la rama master está contenido en la rama styled y por lo tanto solo avanzamos el de la rama master al final del styled haciendo un merge fast forward sin causar ningún conflicto solo actualizando el contenido de master.


### ¿Qué comando o comandos utilizaste en el paso 25?

`git log --graph`

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si, porque la rama title contiene el contenido de master y master no tiene ningun commit que no tenga title por lo que solo se actualizaria el puntero master moviendose a title.

### ¿Qué comando o comandos utilizaste en el paso 27?

`git reset HEAD~1`

### ¿Qué comando o comandos utilizaste en el paso 28?

`git checkout -- git-nuestro.md` o `git reset --hard`

### ¿Qué comando o comandos utilizaste en el paso 29?

`git branch -D title` ya que no esta mergeada sino se podría hacer con el -d.

### ¿Qué comando o comandos utilizaste en el paso 30?

`git reflog`

`git reset 8cba1c1 --hard`

### ¿Qué comando o comandos usaste en el paso 32?


`git log` para localizar el primer commit

 y `git checkout 2ec07c92cb16f9991b2385c782e7451d55499a44` para ir a ese commit

### ¿Qué comando o comandos usaste en el punto 33?

`git checkout master`

