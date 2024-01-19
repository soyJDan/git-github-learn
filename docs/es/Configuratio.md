Configuración inicial
===

1. Antes de configurar Git, asegúrate de tenerlo instalado en tu sistema. Puedes descargar la última versión de Git desde https://git-scm.com/.

<br>

2. **Configuración del nombre de usuario y correo electrónico:**
    - Abre tu terminal o consola y ejecuta los siguientes comandos para configurar tu nombre de usuario y correo electrónico, que se utilizarán para identificar tus cambios en el historial.

    ```shell
        $ git config --global user.name "JDan"
        $ git config --global user.email "jdan@git-scm.com"
    ```

<br>

3. **Configuración del editor de texto predeterminado:**
    - Puedes configurar tu editor de texto preferido para las operaciones que requieren mensajes, como los commits. Por ejemplo, si prefieres usar Visual Studio Code:

    ```shell
        $ git config --global core.editor "code --wait"
    ```
    > Esto configura Git para que utilice Visual Studio Code como editor.

<br>

4. **Verificación de configuración:**
    - Puedes verificar la configuración global de Git en cualquier momento utilizando el siguiente comando:

    ```shell
        $ git config --global --list
    ```
    > Esto mostrará todas las configuraciones globales que has establecido.

<br>

5. **Configuración de autocorrección (Opcional):**
    - Puedes configurar Git para corregir automáticamente ciertos errores tipográficos o comandos mal escritos

    ```shell
        $ git config --global help.autocorrect 1
    ```
    > Esto hará que Git intente corregir automáticamente errores tipográficos en los comandos.

<br>

6. **Configuración de alias para comandos (Opcional):**
    - Puedes crear alias para comandos Git largos y frecuentemente utilizados.

    ```shell
        $ git config --global alias.co checkout
        $ git config --global alias.ci commit
        $ git config --global alias.st status
    ```
    > Ahora puedes usar `git co` en lugar de git checkout, `git ci` en lugar de git commit, y así sucesivamente.

<br>

Con estos pasos, has realizado la configuración inicial de Git en tu sistema. Ahora estás listo para iniciar un repositorio, realizar commits y colaborar en proyectos utilizando Git
