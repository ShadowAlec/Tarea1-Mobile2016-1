## Tarea 1
## Luis Trinidad Ortiz Cisneros
## Diferencia entre reset --soft y reset --mixed

---

**git reset --soft <commit> **

Este tipo de reset no modifica el archivo índice, o el árbol de trabajo para nada, simplemente regresa a ese nodo y los archivos modificados, pasan al stage area. Entonces, si en este punto, hacemos un commit, habremos regresado al nodo original que se "eliminó".



**git reset --mixed <commit> **

 Si se aplica este tipo de reset, el nodo head apuntará al nodo indicado, pero esta vez el índice será también ese nodo, así pues, si hacemos un commit, no pasará nada, pues el índice es el mismo que el nodo head, aún así, los cambios hechos siguen guardados, los cuales están en el área unstaged. Para que se cree un commit con estos nuevos cambios se debe hacer git add (Para los archivos nuevos) y luego git commit, como usualmente se hace.
