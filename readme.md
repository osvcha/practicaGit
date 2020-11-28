11. 
git reset --hard HEAD~1
reset para mover el puntero HEAD, hard porque quiero descartar los cambios del working copy y HEAD~1 porque quiero deshacer el anterior

12. 
git reflog: para buscar el identificador del commit deshecho
git reset --hard 7933ecd: para moverme al commit identificado recuperando el trabajo con hard

13. 
git merge master
Styled ya incluye los cambios de master, por lo tanto ni hace el merge ni genera conflictos: Already up to date.

19.
git checkout styled: para moverme a la rama styled
git merge htmlify: styled absorbe htmlify
Si hay conflictos ya que en ambas ramas se modificó el mismo archivo en las mismas lineas

21.
git checkout master: para moverme a la rama master
git merge styled: master absorbe a styled (resistance is futile)
No hay conflictos, es un merge FF, master incluye ahora los cambios hechos por styled

25.
git log --graph --oneline

26.
git merge --no-ff title
Si podría haber sido FF, ya que title está en la misma "linea" de commits. Si no hubieramos puesto el modificador, habría sido FF por defecto.

27.
git reset HEAD~1

28.
git restore git-nuestro.md

29.
git branch -D title

30.
git reflog: para buscar el identificador del commit del merge con title
git checkout 74ee0d1: para mover el puntero HEAD al commit correspondiente

32.
git reflog: para buscar el identificador del commit del merge con title
git checkout adbe9fe: para mover el puntero HEAD al commit correspondiente

33.
git reflog: para buscar el identificador del commit del merge con title
git checkout 74ee0d1: para mover el puntero HEAD al commit correspondiente

También he borrado la rama master y la he creado en el commit donde se creó el título

Después de crear ls etiquetas y moverme entre ellas he vuelto a master antes de subirlo a github
