#Comandos Utiles en Linux

##Comandos Basicos
Comando | Uso
--------|-----
 **|**    "_Pipe_" | Redirije la salida estandar
 **sudo** _[comando]_ | Ejecuta _[comando]_ en modo super usuario
 **man** _[comando]_ | Muestra la entrada de manual del _[comando]_
 _[comando]_ **&** | Ejecuta el comando y envia el proceso a background (2do plano)
 **>>** _[archivo]_ | Adjunta a _[archivo]_ conservando el contenido anterior
 **>** _[archivo]_ | Escribe a _[archivo]_ sobreescribiendo el contenido anterior
 **echo -n** | Muestra una linea de texto
 **xargs** | Construye una linea de comando usando la salida del comando anterior

##Manejo de Archivos y permisos

Comando | Uso
--------|----
**chmod** <opciones> _[archivo]_ | Modifica los permisos de _[archivo]_ `chmod ug+x script.sh`
**find** |  Busca archivo Ej: `find . -name script.sh`
**rm -rf** _[carpeta]_ | Borra _[carpeta]_ y sus archivos
**cat** _[archivo]_ | Imprime en pantalla todo el contenido de un archivo
**more** _[archivo]_ | Muestra el contenido de un archivo en forma paginada
**less** _[archivo]_ | Mejor que **more**
**wc** _[archivo]_ | Cuenta las palabras en un archivo
**wc -l** _[archivo]_ | Cuenta las lineas en un archivo
**tail** _[archivo]_ | Muestra las ultimas lineas de un archivo
**tail** -f _[archivo]_ | Muestra las ultimas lineas de un archivo interactivamente, muy bueno para monitorear logs
**head** _[archivo]_ | Muestra las primereas lineas de un archivo
**file** _[archivo]_ | Muestra informacion de un archivo (tipo)
**cp** _[archivo1]_ _[archivo2]_ | Copia el archivo1 al archivo 2 Ej: `cp script.sh script.bkp`
**cp -R** _[carpeta1]/*_ _[carpeta2]/_ | Copia **_todo_** el contenido dentro de carpeta1 a carpeta2 Ej: `cp -R scripts/* respaldo_scripts/`
**mv** _[archivo1]_ _[archivo2]_ | Mueve/Renombra el archivo1 a archivo 2 Ej: `mv script.sh script_old.sh`
**mv** _[carpeta1]_ _[carpeta2]_ | Mueve/Renombra carpeta1 y  **_todo_** su contenido a carpeta2 Ej: `mv scripts respaldo_scripts`

