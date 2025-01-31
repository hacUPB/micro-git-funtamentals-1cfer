## ¿Cómo crear un repositorio remoto en GitHub y sincronizarlo con un repositorio local?

Primeramente se debe acceder a la página de [GitHub](https://github.com/) y crear una cuenta o iniciar sesión. A continuación, se debe crear un repositorio con el nombre de nuestra elección:

![Repositorio](/images/crear_rep.png)

Ahora para conectarlo con el repositorio creado localmente, se ejecuta el siguiente comando: 

``` bash
git remote add origin https://github.com/1cfer.repositorio_ejemplo.git
```

El link del repositorio lo podemos encontrar en el botón de `Code`

![Code](/images/code.png)

Cuando se comience editar archivos desde nuestro directorio local y se hagan commits, éstos estarán "adelantados" no se podrán encontrar en la nube hasta que se use el comando:

``` bash
git push
```
Lo que hace es enviar todos los commits que se hayan realizado en el local y que aún no estén en el remoto. 

Cuando se trabaje desde otro dispositivo o computador el cual tiene el repositorio local `desactualizado` del remoto, es decir tenga menos información, se debe usar el comando:

``` bash
git pull
```
De esta forma se evitan errores y se asegura de estar trabajando con la versión más actualizada.