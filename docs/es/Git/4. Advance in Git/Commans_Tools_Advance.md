# Conoce algunas funciones avanzadas de Git

Familiarizarse con herramientas y comandos avanzados de Git es crucial para tener un control más profundo y eficiente sobre tu flujo de trabajo. Aquí hay algunas herramientas y comandos avanzados que pueden resultar útiles:

### 1. **Stash:**
La herramienta `git stash` te permite guardar temporalmente cambios sin realizar un commit. Esto es útil cuando necesitas cambiar de rama o lidiar con cambios emergentes.

```bash
# Guardar cambios en el stash
git stash save "Descripción opcional"

# Listar los stashes
git stash list

# Aplicar cambios del stash
git stash apply stash@{n}
```

### 2. **Cherry Pick:**
El comando `git cherry-pick` te permite aplicar un commit específico de una rama a otra.

```bash
git cherry-pick id_del_commit
```

### 3. **Rebase:**
El rebase es útil para reescribir la historia del proyecto, colocando commits en la punta de otra rama.

```bash
# Cambiar a la rama de destino
git checkout rama_destino

# Realizar el rebase
git rebase rama_fuente
```

### 4. **Interactive Rebase:**
El rebase interactivo te permite modificar, eliminar o combinar commits durante el rebase.

```bash
git rebase -i rama_fuente
```

### 5. **Bisect:**
La herramienta `git bisect` es útil para encontrar el commit que introdujo un problema en tu código.

```bash
# Iniciar el proceso de bisect
git bisect start

# Indicar un commit bueno
git bisect good id_del_commit_bueno

# Indicar un commit malo
git bisect bad id_del_commit_malo
```

### 6. **Submódulos:**
Los submódulos permiten incluir otros repositorios Git dentro de tu propio repositorio.

```bash
# Agregar un submódulo
git submodule add url_del_repositorio

# Clonar un repositorio con submódulos
git clone --recursive url_del_repositorio
```

### 7. **Filtrar Contenidos:**
Puedes utilizar `git filter-branch` o `git filter-repo` para filtrar o reescribir el historial del repositorio.

### 8. **Reflog:**
`git reflog` te muestra el historial de referencia, incluyendo cambios de ramas y otras acciones.

```bash
git reflog
```

### 9. **Hooks:**
[Git hooks](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) te permiten ejecutar scripts en ciertos eventos del ciclo de vida de Git.

### 10. **Log Decorado:**
El log decorado (`git log --graph --decorate --oneline --all`) proporciona una vista gráfica más compacta del historial.

### 11. **Alias:**
Crea alias para comandos largos y frecuentemente utilizados.

```bash
# Crear alias
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.st status
```

### 12. **Grep:**
`git grep` busca patrones en el contenido del repositorio.

```bash
git grep "patrón_a_buscar"
```

### 13. **Autocorrección:**
Configura Git para corregir automáticamente errores tipográficos.

```bash
git config --global help.autocorrect 1
```

### 14. **Trabajo con Refspec:**
Las refspecs en Git se utilizan para especificar el mapeo de referencias entre repositorios remotos y locales.

```bash
# Crear refspec
git config remote.origin.fetch "+refs/heads/*:refs/remotes/origin/*"
```

<br><br>

Estas herramientas y comandos avanzados te brindarán mayor flexibilidad y control sobre tu flujo de trabajo en Git. Es recomendable aprenderlos gradualmente y utilizarlos según sea necesario para optimizar tu eficiencia y gestión del proyecto.