<h1 align="center"> MONITORIZACIÓN DE PROCESOS </h1>
 
<br>

## DIRECTORIOS ENLAZADOS  
[![INICIO](https://img.shields.io/badge/VOLVER%20A%20INICIO-RED?style=for-the-badge&color=%237289da)](./README.md)  
[![ALMACENAMIENTO](https://img.shields.io/badge/IR%20A%20MONITORIZACION%20DE%20ALMACENAMIENTO-RED?style=for-the-badge&color=%237289da)](./monitorizacionAlmacenamiento.md)  
[![RED](https://img.shields.io/badge/IR%20A%20MONITORIZACION%20DE%20RED-RED?style=for-the-badge&color=%237289da)](./monitorizacionRed.md) 
<br>
<br>

*En este repositorio mostraré cuatro comandos que me parecieron interesantes a la hora de monitorear procesos*  
<br>  

## COMANDO PS

El comando *"__ps__"* proporciona una instantánea de los procesos en ejecución en el sistema. Los ejemplos que pongo son los siguientes:  
<br>
> ps -e
>

![Resultado del comandoo ps -e](./img/monitorizacion_procesos/ps-e.png)  
*__Este comando lista todos los procesos en ejecución__*  
<br>
> ps aux
>
![Resultado del comandoo ps aux](./img/monitorizacion_procesos/ps_aux.png)  
*__Este comando muestra detalles de todos los procesos, incluyendo el uso de memoria y el de la CPU__*  
<br>
> ps -u
>
![Resultado del comandoo ps -u](./img/monitorizacion_procesos/ps-u.png)  
*__Este comando lista los procesos específicos de un usuario__*  
<br>
## COMANDO TOP  

El comando *__"top"__* muestra información dinámica sobre los procesos en ejecución y el uso del sistema como CPU, memoria y el tiempo de actividad. A continuación muestro los ejemplos que he seleccionado:  
<br>
> top
>
![Resultado del comandoo top](./img/monitorizacion_procesos/top.png)  
*__Este comando inicia el monitoreo en tiempo real de procesos__*
<br>
> top -u
>
![Resultado del comandoo top -u](./img/monitorizacion_procesos/top-u.png)  
*__Este comando filtra la lista para mostrar solo los procesos de un usuario específico__*  
<br>
> htop
>
![Resultado del comandoo htop](./img/monitorizacion_procesos/htop.png)  
*__Este comando es una alternativa más avanzada y más amigable que el "top", eso si, requiere de una instalación__*  
<br>
## COMANDO PIDSTAT  

El comando *__"pidstat"__* muestra estadísticas sobre el uso de recursos por procesos específicos. Los ejemplos que elegí fueron estos:  
<br>
> pidstat
>
![Resultado del comandoo pidstat](./img/monitorizacion_procesos/pidstat.png)  
*__Este comando muestra las estadísticas generales de CPU por proceso__*  
<br>
> pidstat -r
>
![Resultado del comandoo pidstat -r](./img/monitorizacion_procesos/pidstat-r.png)  
*__Este comando monitorea el uso de memoria de los procesos__*   
<br>
> pidstat -u -p
>
![Resultado del comandoo pidstat -u -p](./img/monitorizacion_procesos/pidstat-u-p.png)  
*__Este comando muestra estadísticas específicas de CPU para un proceso en concreto__*
<br>
## COMANDO PGREP  

El comando *__"pgrep"__* permite buscar procesos por nombre y devuelve sus PIDs. Los que seleccioné fueron:  
<br>
> pgrep
>
![Resultado del comandoo pgrep](./img/monitorizacion_procesos/pgrep.png)  
*__Este comando encuentra los procesos relacionados con el servicio que desees, en este caso Apache__*  
<br>
> pgrep -u
>
![Resultado del comandoo pgrep -u](./img/monitorizacion_procesos/pgrep-u.png)  
*__Este comando busca procesos ejecutados por un usuario en concreto__*  
<br>
> pgrep -fl
>
![Resultado del comandoo pgrep -fl](./img/monitorizacion_procesos/pgrep-fl.png)  
*__Este comando muestra el nombre coompleto del proceso junto con su PID__*  
<br>
<br>

