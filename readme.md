- ¿Qué comando utilizaste en el paso 11?¿Por qué?
git reset --hard
Porque lo quería modificar todo.

- ¿Qué comando o comandos utilizaste en el paso 12?¿Por qué?
1º reflog - para encontrar el ID del commit anterior.
2º git reset --hard con el ID del commit - para restaurar todos los cambios.

- El merge del paso 13, ¿Causó algún conflicto?¿Por qué?
No. Porque "styled" ya tenía el commit de "master", de modo que no ha supuesto
 diferencia.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Si. Porque habíamos modificado las mismas líneas en git-nuestro, y al hacer 
un no-fast-forward, cuando se ha creado un nuevo archivo git-nuestro, 
no sabía cuáles eran las líneas correctas que debía utilizar.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No. Porque ha sido fast-forward, ya que el contenido de "master" ya formaba
parte de "styled".

- Qué comando o comandos utilizaste en el paso 25?
git log --graph --decorate --pretty=oneline

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si. Porque la rama "title" ya contiene lo mismo que master.

- ¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?
git restore git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?
git reflog: para buscar el commit
git show 28300fb: para asegurarme que es el commit correcto
git reset 28300fb: para volver al punto del merge
git restore .: porque no hice el reset hard, y así pasé todos los cambios al working.

- ¿Qué comando o comandos utilizaste en el paso 32?
git log: para buscar el commit
git reset --hard: para ir al commit y cambiar el working copy

- ¿Qué comando o comandos utilizaste en el paso 33?
git reset --hard HEAD@{1}
