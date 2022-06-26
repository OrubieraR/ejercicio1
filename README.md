# Ejercicio1

Ejercicio 1 Git - GitHub
---

1. **¿Qué comando utilizaste en el paso 11? ¿Por qué?**
 
`Git reset --hard HEAD˜1`
Utilicé este comando porque en el paso 11 había que deshacer el último commit y que 
en el working copy estuviesen los archivos que había en el anterior commit, 
modificando el staging area.


2. **¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog` para ver todos los movimientos que ha habido y para localizar el commit 
en el que está el “git-nuestro.md” de la rama “styled”.

Luego hacer un `reset --hard` (aquí el commit al que se quiere cambiar).


3. **El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

Git devuelve “Already up to date” porque se está intentando fusionar una rama hijo 
en una rama padre.


4. **El merge del paso 19, ¿Causó algún conflicto? ¿Por qué́?**

Sí hubo un conflicto porque había 2 versiones del archivo “git-nuestro.md” 
diferentes.

Se resuelve el conflicto en el archivo, editándolo con Nano y dejando el contenido 
que se creó en la rama “styled”.

Después se continua con el merge ejecutando “git commit” y añadiendo el comentario 
tras el nombre del archivo en el texto generado automáticamente por Git que contiene 
toda la información del conflicto.


5. **El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

Al estar los commits “en lista” el puntero head avanza y el archivo “git-nuestro.md” 
tendría el contenido de hubiera en la rama “styled”.

En este punto hice una prueba. Creé un nuevo commit con una modificación en el 
archivo “git-nuestro.md” y después hice el merge.
Al unir la rama styled con master creo un conflicto porque había 2 versiones del 
archivo “git-nuestro.md”.

Hay que resolver nuevamente el conflicto sobre el archivo y hacer el commit.


6. **¿Qué comando o comandos utilizaste en el paso 25?**

Para dibujar el diagrama utilicé el comando `git log –graph –decorate – 
pretty=oneline.

Para mayor comodidad cree un atajo con git config alias.graph “git log –graph 
–decorate – pretty=oneline".


7. **El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí podría ser fast-forward porque las ramas están en lista.


8. **¿Qué comando o comandos utilizaste en el paso 27?**

Utilicé `git reset HEAD~1`


9. **¿Qué comando o comandos utilizaste en el paso 28?**

Utilicé `git status` para saber qué archivos había en stage área.
Después usé `git restore git-nuestro.md`.


10. **¿Qué comando o comandos utilizaste en el paso 29?**

Usé el comando: `git Branch -D title`


11. **¿Qué comando o comandos utilizaste en el paso 30?**

Usé `git reflog para localizar el SHA del commit y luego usé  `git reset –hard 
numero commit`.


12. **¿Qué comando o comandos usaste en el paso 32?**

Utilicé, `git log` copié el SHA del primer commit, cuando se creó el poema.
Después hice un `git reset --hard SHA del primer commit`


13. **¿Qué comando o comandos usaste en el punto 33?**

Usé `git reflog` para averiguar el SHA del commit en el que añadimos el título del 
poema.

Después `git reset --hard SHA` para volver a ese estado.
