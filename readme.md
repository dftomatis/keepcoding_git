# Guía de Comandos Utilizados en los Ejercicios de Git

##  ¿Qué comando utilizaste en el paso 11? ¿Por qué?
```bash
$ git reset --hard HEAD~1
```
Deshace el último commit y lo que hay en el working y el staging area queda vacío.

---

##  ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
```bash
$ git reflog
```
Para ver los cambios en el repo y el ID al que quiero volver.

```bash
$ git reset --hard 3613d85
```
Regresa el puntero a ese ID.

---

##  ¿El merge del paso 13 causó algún conflicto? ¿Por qué?
El merge no causó conflictos porque `styled` ya incluía todos los cambios de `main`.

---

##  ¿El merge del paso 19 causó algún conflicto? ¿Por qué?
En `styled`, `git-nuestro.md` tenía formato Markdown.
En `htmlify`, `git-nuestro.md` fue modificado para usar etiquetas HTML.
Cuando Git intentó fusionar ambas versiones en `styled`, detectó que el mismo archivo había sido modificado de manera diferente en ambas ramas y no puede decidir automáticamente qué versión conservar, por lo que marca el archivo como en conflicto y te pide que elijas qué cambios mantener.

---

##  ¿El merge del paso 21 causó algún conflicto? ¿Por qué?
No hubo conflictos porque `main` no tenía cambios propios desde que `styled` se bifurcó.
Git pudo hacer un fast-forward sin necesidad de resolver diferencias manualmente.
Si `main` hubiera tenido cambios adicionales, el merge habría requerido resolución de conflictos.

---

##  ¿Qué comando o comandos utilizaste en el paso 25?
```bash
git log --graph --oneline --all
```
Muestra la información de los commits pintando un grafo. 
- `--oneline` muestra cada commit en una sola línea para facilitar la lectura.
- `--all` muestra todos los commits, incluso los de ramas que no están activas.

---

##  ¿El merge del paso 26 podría ser fast forward? ¿Por qué?
Sí, porque `main` no tenía cambios adicionales después de crear `title`.

---

##  ¿Qué comando o comandos utilizaste en el paso 27?
```bash
git reset HEAD~1
```
Deshace el último commit manteniendo el working copy.

---

##  ¿Qué comando o comandos utilizaste en el paso 28?
```bash
git restore git-nuestro.md
```

---

##  ¿Qué comando o comandos utilizaste en el paso 29?
```bash
git branch -D title
```

---

##  ¿Qué comando o comandos utilizaste en el paso 30?
```bash
$ git reflog
```
Para ver los cambios en el repo y el ID al que quiero volver.

```bash
$ git reset --hard 50b1ffd
```
Regresa el puntero a ese ID.

---

##  ¿Qué comando o comandos usaste en el paso 32?
```bash
git log --oneline --reverse
```
Muestra los commits en formato resumido e invierte el orden para que el primer commit aparezca primero.

```bash
git checkout 17f4f0c
```
Me mueve al commit con ese ID.

---

##  ¿Qué comando o comandos usaste en el punto 33?
```bash
git reflog
```
```bash
git checkout 50b1ffd


