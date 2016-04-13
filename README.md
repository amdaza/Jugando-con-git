# Jugando-con-git
Ejercicio 1 de prácticas de Git

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
$ git reset --hard HEAD~1
Reset para mover tanto el puntero HEAD como la rama styled.
--hard para perder los cambios realizados en el working copy

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
$ git reflog
Para ver el historial de movimientos de HEAD.

$ git reset 8bf779e
Para ir al último commit.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No, porque master es un ancestro del commit donde nos encontramos. Por tanto, nos sale un mensaje "already up to date", pues los cambios de master ya están incluidos en styled.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Sí, porque en ambas ramas hay cambios en las mismas líneas (en este caso, todas las líneas).

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
Ninguno, porque se trata de un merge fast-forward. Es decir, los cambios que contiene master ya están incluidos en styled, y por ello basta con mover la rama master al donde se encuentra la rama styled.

- ¿Qué comando o comandos utilizaste en el paso 25?
$ git log --graph --decorate

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Sí, por lo mismo que en el paso 21. la rama title contiene todos los cambios que tenía master. Por tanto, con mover las ramas habría bastado.

- ¿Qué comando o comandos utilizaste en el paso 27?
$ git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?
$ git reset --hard HEAD

- ¿Qué comando o comandos utilizaste en el paso 29?
$ git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?
$ git reflog
$ git reset --hard 131b06b

- ¿Qué comando o comandos usaste en el paso 32?
$ git reflog
$ git checkout 51249ac

- ¿Qué comando o comandos usaste en el punto 33?
$ git reflog
$ git checkout 131b06b
