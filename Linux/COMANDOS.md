#Comandos Utiles en Linux

##Comandos Basicos
Comando | Uso
------------------------------------------------------------------------------------------------
 **|**    "_Pipe_" | Redirije la salida estandar
 **sudo** _[comando]_ | Ejecuta _[comando]_ en modo super usuario
 **man** _[comando]_ | Muestra la entrada de manual del _[comando]_
 _[comando]_ **&** | Ejecuta el comando y envia el proceso a background (2do plano)
 **>>** _[archivo]_ | Adjunta a _[archivo]_ conservando el contenido anterior
 **>** _[archivo]_ | Escribe a _[archivo]_ sobreescribiendo el contenido anterior
 **echo -n** | Muestra una linea de texto
 **xargs** | Construye una linea de comando usando la salida del comando anterior

##Manejo de Archivos y permisos

* **chmod** <opciones> _[archivo]_   Modifica los permisos de _[archivo]_
```bash
#ejemplo de uso agrega permiso de ejecucion a script.sh para el dueño y el grupo 
chmod ug+x script.sh
```

* **find**    Busca archivo Ej:
```bash
find . -name script.sh
```

* **rm -rf** _[carpeta]_    Borra _[carpeta]_ y sus archivos
