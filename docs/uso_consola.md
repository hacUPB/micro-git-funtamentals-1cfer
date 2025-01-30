# ¿Cómo crear y navegar por directorios y archivos desde la consola de Git Bash?

## Crear un Directorio

Lo primero que debemos hacer es crear un **directorio** o una **carpeta** para poder agregar archivos y navegar entre ellos. Para ello, usamos el comando en la consola:

``` Bash
mkdir Nombre_directorio
```

Esto crea una carpeta con el nombre que se requiera. Si el nombre contiene espacios, se debe usar:

``` Bash
mkdir "Nombre directorio"
```

Para saber la dirección de la carpeta que se acaba de crear, se puede usar el comando:

``` Bash
pwd
```
Lo que conseguimos con esto, es que nos muestre la dirección donde actualmente se está creando carpetas o archivos.

![Ejemplo del uso del comando pwd](/images/pwd.png)

Para listar las el contenido que podemos encontrar en la dirección en la que estamos, se usa el comando:

``` Bash
ls
```

Si queremos una lista detallada de los archivos y directorios, proporcionando más información, se usa el comando

``` Bash
ls -l
```
![Ejemplo del uso del comando pwd](/images/ls.png)


Una vez se reconozca la carpeta a la cual se requiera **acceder** y ver su contenido, se puede usar el comando:

``` Bash
cd carpeta_requerida
```

Si es necesario volver a la carpeta anterior, se usa el comando:

``` Bash
cd ..
```
Al estar en el directorio deseado, es posible crear un archivo de cualquier formato, agregando la extensión correspondiente después del punto en el nombre del archivo (por ejemplo, .py para archivos de Python o .txt para archivos de texto), utilizando el comando:

``` Bash
touch nombre_del_archivo.txt
```
De igual forma que las carpetas, si se usa espacios entre las palabras, es necesario usar las comillas ("nombre del archivo".txt), de lo 

De ser necesario, se puede eliminar un archivo o una carpeta (depende si contiene o no información dentro). Para ello existen 2 comandos:

``` Bash
rm nombre_del_archivo.txt
```
Es el mismo para una carpeta. Sin embargo, si la carpeta contiene información, como archivos o subcarpetas, se usa:

``` Bash
rm -r carpeta_requerida
```
Lo que indica `-r` es que el comando debe recorrer la carpeta y eliminar todos los archivos y subdirectorios dentro de ella.

