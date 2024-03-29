# **Comandos de la terminal**

## **Listado de archivos**

Muestra información acerca del comando

```
<comando> --help 
```

Limpia la terminal

```
clear
```

Muestra el directorio en el que uno se encuentra actualmente

```
pwd
``` 
list (muestra el contenido de un direcotrio o carpeta)

```
ls
```

muestra una lista del contenido del directorio pero de una manera más elegante.

```
ls -l 
```

muestra una lista del contenido del directorio pero de una manera más elegante en forma de lista, el parámetro -h permite ver el tamaño de cada archivo, ejemplo: 120MB, 202GB, 23849K, 93284213b.
alias ls='ls -l -h --color=auto' Se puede crear un alias que ejecute un comando con varios parámetros que usamos habitualmente de una manera más corta, entonces al escribir ls en realidad se eejuctará el comando ls -l -h --color=auto

```
ls -l -h 
```

## **Moverse por la terminal**

Change directorie, sirve para cambiar de directorios

```
cd <nombre del directorio> 
```

Vuelve un directorio atrás
```
cd ..  
```
Vuelve un direcotrio, pero es menos rápido que hacer cd ..
```
cd /<nombre del directorio> 
```
Directorio actual
```
cd . 
```
Cambia de directorio según la ruta especificada.
```
cd <ruta>
```
Vuelve al último directorio en el que estábamos, como si se tratará de cambiar de una carpeta anteriormente seleccionada.
```
cd - 
```
Sin importar donde uno se encuentre cambiar al directorio /home.
```
cd ~ 
```

## **Como saber el contenido del un archivo** 

Muestra un archivo
```
cat <nombre del archivo> 
```
Muestra el archivo con número de lineas
```
cat -n <nombre del archvivo> 
```
Muestra el archivo cada 30 líneas teniendo que tocar enter para seguir viendo el resto del archivo, para terminar de ver el archivo se debe tocar la letra q para poder salir de este modo de lectura.
```
cat -n <nombre del archivo> | less 
```
## **Permisos de administrador**

Significa Super user do. Al comando que se le agrega `sudo` hará que el mismo se ejecute en modo de administrador con todos los priviliejos que esto consiste.
```
sudo <comando>
```
## **Creando archivos y directorios**

Crea un archivo vacio sin nigún contenido
```
touch <nombre del archivo> 
```
El contenido escrito emtre comillas dobles se colocarmá en el archivo especificado
```
echo "Contenido" > <nombre del archivo> 
```
Modifica el contenido del archivo manteniendo el contenido del archivo (es decir, sin reeeplazarlo).
```
echo "Contenido2" >> <nombre del archivo> -
```
 Crea una carpeta
```
mkdir <nombre de la carpeat> 
```
Crea una carpeta dentro de otra de una manera más sencillas, esto mediante el comando -p
```
mkdir -p <nombre de la carpeta1> 
```
Copia un archivo y lo copia en una ruta especificada como segundo parámetro.
```
cp <ruta origen> <ruta destino> 
```
Copia un directorio con todos sus archivos y subdirectorios internos a la carpeta de destino
```
cp -r <nombre del directorio de origen> <nombre del directorio de destino> 
```
borra un archivo
```
rm <nombre del archivo> 
```
Pregunta antes de eliminar un archivo
```
rm -i 
```
Pregunta antes de eliminar un archivo, uno, por uno con todos los archivos
```
rm -i * 
```
elimina un directorio con todo su contenido
```
rm -r <nombre del archivo> 
```
-> Mueve un archivo o directorio
```
mv <origen> <destino> -
```
```
find <direcotiro en el que quieres buscar> -name "<nombre del archivo>"
```
buscara el archivo sin importar si su nombre tiene mayúsculas y minúsculas
```
find . -iname <nombre del archivo> 
```
-type d especifica que solo se quiere buscar directorios y no archivos
```
find . -type d -iname "<nombre del directorio>" 
```

# **Trabajo con archivos**


