<h1 align="center"> MONITORIZACIÓN DE ALMACENAMIENTO </h1>
 
<br>

## DIRECTORIOS ENLAZADOS  
[![INICIO](https://img.shields.io/badge/VOLVER%20A%20INICIO-RED?style=for-the-badge&color=%237289da)](./README.md)  
[![PROCESOS](https://img.shields.io/badge/IR%20A%20MONITORIZACION%20DE%20PROCESOS-RED?style=for-the-badge&color=%237289da)](./monitorizacionProcesos.md)  
[![RED](https://img.shields.io/badge/IR%20A%20MONITORIZACION%20DE%20RED-RED?style=for-the-badge&color=%237289da)](./monitorizacionRed.md) 
<br>
<br>
*En este repositorio muestro cuatro comandos útiles a la hora de monitorear el almacenamiento*
<br>

## COMANDO DF  

El comando *__"df"__* informa sobre el uso del espacio en disco de los sitemas de archivos montados. Los ejemplos que elegí son los siguientes:  
<br>
> df -h
>
![Resultado del comandoo df -h](./img/monitorizacion_almacenamiento/df-h.png)  
*__Este comando muestra el uso del espacio en disco en formato legible__*
<br>
> df -T
>
![Resultado del comandoo df -T](./img/monitorizacion_almacenamiento/df-T.png)  
*__Este comando indica el tipo de sistema de archivos junto con el espacio utilizado__*
<br>
> df "directorio"
>
![Resultado del comandoo df /home](./img/monitorizacion_almacenamiento/df-home.png)  
*__Este comando detalla el uso de disco del sistema de archivos donde está montado el directorio indicado__*
<br>

## COMANDO DU  

El comando *__"du"__* muestra el uso del espacio en disco por archivos y directorios. Las diferentes variantes del comando que elegí fueron:  
<br>
> du -h
>
![Resultado del comandoo du -h](./img/monitorizacion_almacenamiento/du-h.png)  
*__Este comando muestra el tamaño de los directorios en un formato legíble__*
<br>
> du -sh "ruta"
>
![Resultado del comandoo du -sh](./img/monitorizacion_almacenamiento/du-sh.png)  
*__Este comando resume el uso de espacio de un archivo oo directorio específico__*  
<br>
> du --max-depth=1
>
![Resultado del comandoo du --max-depth](./img/monitorizacion_almacenamiento/du--max-depth.png)  
*__Este comando muestra el tamaño de directorios en el nivel superior de una jerarquía__*  
<br>

## COMANDO LSBLK  

El comando *__"lsblk"__* lista la información de dispositivos de bloques, como discos y particiones. Los que me parecieron más interesantes fueron:  
<br>
> lsblk
>
![Resultado del comandoo lsblk](./img/monitorizacion_almacenamiento/lsblk.png)  
*__Este comando lista todos los dispositivos de bloques y su jerarquía__*  
<br>
> lsblk -f
>
![Resultado del comandoo lsblk -f](./img/monitorizacion_almacenamiento/lsblk-f.png)  
*__Este comando incluye información del sistema de archivos__*  
<br>
> lsblk -o NAME,SIZE,TYPE,MOUNTPOINT
>
![Resultado del comandoo lsblk -o](./img/monitorizacion_almacenamiento/lsblk-o.png)  
*__Este comando personaliza las columnas en la salida__*  
<br>


## COMANDO MOUNT  

El comando *__"mount"__* muestra sistemas de archivos montados y permite montarlos o desmontarlos. A mi parecer los mejores son:  
<br>
> mount
>
![Resultado del comandoo mount](./img/monitorizacion_almacenamiento/mount.png)  
*__Este comando lista todos los sistemas de archivos actualmente montados__*  
<br>
> mount | grep "disco deseado/partición deseada"
>
![Resultado del comandoo mount+grep](./img/monitorizacion_almacenamiento/mount-grep.png)  
*__Este comando te filtra el resultado de una partición específica__*  
<br>
> mount -o remount,rw /
>
![Resultado del comandoo mount -o](./img/monitorizacion_almacenamiento/mount-o.png)  
*__Este comando remonta el sistema de archivos raíz como lectura-escritura__*  
<br>


