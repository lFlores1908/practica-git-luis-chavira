\# Práctica de Git y GitHub



\## Datos del estudiante



\*\*Nombre:\*\* Luis Angel Chavira Flores  

\*\*Matrícula:\*\* 2630008  



\## Nombre de la práctica



Creación y administración de un repositorio local con Git y sincronización con GitHub.



\## Objetivo de la práctica



El objetivo de esta práctica fue reforzar el uso de Git y GitHub mediante la creación de un repositorio local, el registro de cambios utilizando el área de preparación o Staging Area, la creación de commits y la vinculación del repositorio local con un repositorio remoto en GitHub.



También se practicó la sincronización de cambios en ambas direcciones, es decir, desde el repositorio local hacia GitHub mediante `git push` y desde GitHub hacia el repositorio local mediante `git pull`.



\## Procedimiento realizado



Primero se creó una carpeta llamada `practica-git-luis-chavira`, la cual se utilizó como directorio principal para la práctica.



Después se abrió PowerShell dentro de esta carpeta y se inicializó un repositorio local utilizando el comando:



```bash

git init

```



Posteriormente se configuró la rama principal con el nombre `main` mediante:



```bash

git branch -M main

```



Se crearon los archivos `README.md` y `datos.txt`. El archivo `datos.txt` se utilizó para realizar diferentes modificaciones durante la práctica.



Una vez creados los archivos, se verificó el estado del repositorio con:



```bash

git status

```



Después se agregaron los archivos al área de preparación utilizando:



```bash

git add .

```



Una vez preparados los archivos, se realizó el primer commit del repositorio con:



```bash

git commit -m "Primer commit"

```



Posteriormente se creó un repositorio público en GitHub con el mismo nombre del repositorio local.



El repositorio remoto se vinculó con el repositorio local utilizando:



```bash

git remote add origin URL\_DEL\_REPOSITORIO

```



Después se verificó la configuración del repositorio remoto mediante:



```bash

git remote -v

```



Una vez establecida la conexión, se enviaron los archivos del repositorio local a GitHub por primera vez con:



```bash

git push -u origin main

```



Después se modificó directamente el archivo `datos.txt` desde la página de GitHub, agregando una nueva línea al archivo.



Para descargar ese cambio al repositorio local se utilizó:



```bash

git pull origin main

```



Posteriormente se modificó nuevamente el archivo `datos.txt`, pero esta vez desde la computadora local.



El cambio se agregó al área de preparación, se creó un nuevo commit y finalmente se envió nuevamente a GitHub mediante:



```bash

git add .

git commit -m "modificado localmente"

git push

```



De esta manera se comprobó que los cambios podían sincronizarse correctamente tanto desde GitHub hacia el repositorio local como desde el repositorio local hacia GitHub.



\## Comandos de Git utilizados



\### `git init`



Inicializa un repositorio de Git dentro de la carpeta actual. Este comando crea la estructura necesaria para que Git pueda comenzar a registrar los cambios realizados en los archivos.



\### `git branch -M main`



Cambia el nombre de la rama principal a `main`.



\### `git status`



Permite revisar el estado actual del repositorio y muestra qué archivos han sido modificados, cuáles están preparados para un commit y cuáles todavía no están siendo rastreados por Git.



\### `git add .`



Agrega todos los archivos modificados o nuevos al área de preparación o Staging Area.



\### `git commit -m "mensaje"`



Guarda una versión de los cambios preparados en el historial local del repositorio. El mensaje permite describir brevemente qué cambios se realizaron.



\### `git remote add origin URL`



Vincula el repositorio local con un repositorio remoto, en este caso alojado en GitHub.



\### `git remote -v`



Muestra las direcciones de los repositorios remotos configurados.



\### `git push -u origin main`



Envía por primera vez los commits de la rama `main` del repositorio local al repositorio remoto en GitHub.



La opción `-u` permite establecer una relación entre la rama local `main` y la rama remota `origin/main`.



\### `git push`



Envía al repositorio remoto los commits realizados localmente que todavía no se encuentran en GitHub.



\### `git pull origin main`



Descarga los cambios existentes en la rama `main` del repositorio remoto y los integra en el repositorio local.



\## Creación del repositorio local



El repositorio local fue creado dentro de una carpeta en la computadora. Después de abrir PowerShell dentro de esa carpeta, se ejecutó `git init`, lo que permitió convertirla en un repositorio administrado por Git.



A partir de ese momento Git comenzó a detectar los archivos y cambios realizados dentro de la carpeta.



\## Vinculación del repositorio local con GitHub



Después de crear el repositorio local se creó un repositorio público en GitHub.



La dirección HTTPS del repositorio de GitHub se agregó como repositorio remoto utilizando `git remote add origin`.



Esto permitió establecer una conexión entre el repositorio local de la computadora y el repositorio remoto almacenado en GitHub.



\## Sincronización Local → GitHub



Para enviar cambios desde la computadora hacia GitHub se utilizó el siguiente flujo:



```text

Working Directory

&#x20;      ↓

git add .

&#x20;      ↓

Staging Area

&#x20;      ↓

git commit

&#x20;      ↓

Repositorio local

&#x20;      ↓

git push

&#x20;      ↓

GitHub

```



Primero se modificaron los archivos, después se agregaron al Staging Area, posteriormente se creó un commit y finalmente se enviaron los cambios a GitHub utilizando `git push`.



\## Sincronización GitHub → Local



También se realizó una modificación directamente desde la página de GitHub.



Para descargar ese cambio al repositorio local se utilizó:



```bash

git pull origin main

```



Este comando permitió actualizar los archivos de la computadora con la versión más reciente almacenada en GitHub.



\## Archivos contenidos en el repositorio



\### `README.md`



Contiene la documentación de la práctica, incluyendo el objetivo, el procedimiento realizado, los comandos utilizados y la explicación del funcionamiento de Git y GitHub.



\### `datos.txt`



Archivo utilizado para comprobar la sincronización de cambios entre el repositorio local y GitHub.



Durante la práctica este archivo fue modificado tanto desde GitHub como desde el repositorio local.



\## Conclusión



Esta práctica me permitió recordar y reforzar el funcionamiento básico de Git y GitHub.



Comprendí nuevamente la diferencia entre el directorio de trabajo, el área de preparación y el repositorio local, así como la importancia de realizar commits para mantener un historial ordenado de los cambios realizados.



También pude comprobar cómo se vincula un repositorio local con GitHub y cómo utilizar `git push` para enviar cambios al repositorio remoto y `git pull` para descargar modificaciones realizadas desde GitHub.



El uso de Git permite mantener un mejor control de versiones de los archivos y facilita el seguimiento de los cambios realizados durante el desarrollo de un proyecto.

