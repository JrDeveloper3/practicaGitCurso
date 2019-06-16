Ejercicio 1
- - - - - - - - - - - -- - - 
1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?
  >He utilizado el comango git reset --hard HEAD~1, con esto deshago el commit realizado y lo elimino de Working Copy
  >debido al --hard.
  
2.  ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
>Con el git reflog vemos todas las operaciones que hemos realizado y asi obtenemos el SHA del commit que queremos rehacer.
>Realizo un commit reset --hard **SHA** para modificar el contenido del Working COpy, volviendo a antes de deshacer el último commit.

3.El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
>Sí , hay conflictos ya que el archivo git-nuestro.md tiene contenidos diferentes, por lo que debemos elegir con que contenido quedarnos
>y volver hacer git add git-nuestro.md cuando esten solucionados los conflictos.

4.El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
> Utilizamos el comando git log --graph y otro que resume mas el diagrama que sera git log --pretty=oneline --graph.

5.El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
> Si ya que la rama title esta creada a partir del ultimo commit realizado en la rama master, por lo que el puntero HEAD-> MASTER PUEDE IR >DIRECTAMENTE HASTA EL DE TITLE.

6. Qué comando o comandos utilizaste en el paso 27?
>git reset HEAD~1 sin el --hard ya que no queremos eliminar los cambios del Working Copy.

7. ¿Qué comando o comandos utilizaste en el paso 28?
> git checkout git-nuestro.md para descartar los cambios unicamnete de ese archivo.

8. ¿Qué comando o comandos utilizaste en el paso 29?
> git branch -D title para eliminar la rama title

9. ¿Qué comando o comandos utilizaste en el paso 30?
> Primero ejecuto git reflog para ver las operaciones realizadas y localizar el merge a rehacer. Cuando lo localito hafgo git reset --hard **SHA** para ctualizar el Working Copy y volver al estado deseado.

10. ¿Qué comando o comandos usaste en el paso 32?
>Como en el paso anterior lanzo git reflog y git reset **SHA** para situarme en el commit que deseo, sin --hard ya que no quiero actualizar el Working Copy.

11. ¿Qué comando o comandos usaste en el punto 33?
>Hago lo mismo que en el paso anterior.
