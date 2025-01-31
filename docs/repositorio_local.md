# ¿Cómo crear un repositorio local con comandos de git?

Lo primero que se debe hacer es ubicar una carpeta en el computador donde se va a almacenar el repositorio. Es recomendable elegir la carpeta de `documentos`.

Hay varias formas de empezar a crear repositorios, por ejemplo, se abre la aplicación de `Git Bash`, y se ejecuta el comando:

```bash
cd documents
```
![Ubicarse en la carpeta de Documentos](/images/cd_documents.png)

Una vez en la carpeta deseada, se procede a crear la carpeta que va a contener el o los repositorios. Para ellos se usa:

```bash
mkdir repositorios
```

Ingresamos a la carpeta que se acaba de crear con:

```bash
cd repositorios
```

Aquí se crearán todos los repositorios que se requiera. No se puede crear uno dentro de otro.

Para crear el primer repositorio, acceder a él e inicializarlo, se usan los siguientes comandos:

```bash
mkdir ejemplo
cd ejemplo
git init
```
El repositorio creado en este caso, se llama `ejemplo`. Nótese que ahora en la consola aparece una marca a la derecha, `main`, la cual identifica que el directorio ahora es un repositorio.

![Ejemplo de como se ve Main](/images/init3.png)

En el repositorio se pueden aplicar los mismos comandos usados explicados en [Uso Consola](docs/uso_consola.md). Adicional a ello, hay comandos propios de git, los cuales servirán para el control de las versiones de los archivos y el buen gestionamiento de la información. Algunos comandos son: 

```bash
git status
```

Este comando nos da información sobre los cambios en nuestro respositorio hasta ese momento. Por ejemplo, si se ham modificado, eliminado, cambios sin guardar o para saber si hay algo que no se ha subido o descargado del servidor (más detalles acerca de la nube en [Repositorio Remoto](docs/repositorio_remoto.md)).

Si no se ha realizado ningún cambio, aparecerá que no hay nada a lo qué hacer `commit`.

### Que es un commit?
Un commit es una acción en los sistemas de control de versiones que guarda los cambios hechos en un proyecto. Permite guardar el estado del código en un momento específico y facilita ver el historial de cambios. Cada commit tiene una breve descripción de lo que se modificó.

Cuando se quiera guardar los cambios importantes de forma segura y que mas adelante se puedan deshacer o recuperar sin problemas de que se pierdan o se dañen, se debe agregar los archivos modificados o eliminados al área de preparación con el comando `add`, por ejemplo:

```bash
git add archivo1.py
```
Luego de eso se debe hacer el commit y agregar una breve descripción que informe acerca de los cambios realizados. Se puede hacer un solo commit con varios archivos o se puede hacer individualmente, algo útil por si se quiere revertir un commit. El commit se hace con el comando: 

```bash
git commit m- "Breve descripción de los cambios realizados"
```
En cualquier momento de los pasos es posible y recomendable ver el `status`. De esa forma se asegura que los cambios que se hayan hechos, queden efectivamente guardados.

Si se quiere ver el historial de commits se usa el comando:


```bash
git log
```

Si se quiere ver la información de lo commits más compacta, es posible usando:

```bash
git log --oneline
```
![Commit_oneline](/images/commit_oneline.png)

