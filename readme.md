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

- El merge del paso 26, ¿Podría ser fast forward?

¿Por qué?

- ¿Qué comando o comandos utilizaste en el paso 27?

- ¿Qué comando o comandos utilizaste en el paso 28?

- ¿Qué comando o comandos utilizaste en el paso 29?

- ¿Qué comando o comandos utilizaste en el paso 30?

- ¿Qué comando o comandos utilizaste en el paso 32?

- ¿Qué comando o comandos utilizaste en el paso 33?
