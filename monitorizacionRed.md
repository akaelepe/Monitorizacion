<h1 align="center"> MONITORIZACIÓN DE RED </h1>
 
<br>

## DIRECTORIOS ENLAZADOS  
[![INICIO](https://img.shields.io/badge/VOLVER%20A%20INICIO-RED?style=for-the-badge&color=%237289da)](./README.md)  
[![PROCESOS](https://img.shields.io/badge/IR%20A%20MONITORIZACION%20DE%20PROCESOS-RED?style=for-the-badge&color=%237289da)](./monitorizacionProcesos.md)  
[![ALMACENAMIENTO](https://img.shields.io/badge/IR%20A%20MONITORIZACION%20DE%20ALMACENAMIENTO-RED?style=for-the-badge&color=%237289da)](./monitorizacionAlmacenamiento.md)  
<br>
<br>

*En este repositorio traigo los comandos que más me llamaron la atención en cuanto a monitoreo de la red*
<br>
<br>

## COMANDO IFCONFIG  

El comando *__"ifconfig"__* muestra la configuración de la red de las interfaces. Aunque está en desuso en algunas distribuciones sigue siendo importante. Los más remarcables son:  
<br>
> ifconfig
>
![Resultado del comandoo ifconfig](./img/monitorizacion_red/ifconfig.png)  
*__Este comando muestra todas las interfaces de red activas__*
<br>
> ip a
>
![Resultado del comandoo ip a](./img/monitorizacion_red/ip-a.png)  
*__Alternativa moderna y, actualmente la que se usa, para mostrar las interfaces de red__*
<br>
> ip -s link
>
![Resultado del comandoo ip -s](./img/monitorizacion_red/ip-s.png)  
*__Este comando muestra las estadísticas de las interfaces de red__*
<br>

## COMANDO NETSTAT  

El comando *__"netstat"__* proporciona información sobre conexiones de red, tablas de enrutamiento y estadísticas de tráfico. A mi criterio los que más usos tendrían son:  
<br>
> netstat -tuln
>
![Resultado del comandoo netstat -tuln](./img/monitorizacion_red/netstat-tuln.png)  
*__Este comando lista las conexiones activas y puertos en escucha__*  
<br>
> netstat -i
>
![Resultado del comandoo netstat -i](./img/monitorizacion_red/netstat-i.png)  
*__Este comando muestra las estadísticas de las interfaces de red__*
<br>
> ss -tuln
>
![Resultado del comandoo ss -tuln](./img/monitorizacion_red/ss-tuln.png)  
*__Este comando es la alternativa moderna para listar sockets en escucha__*
<br>

## COMANDO PING  

El comando *__"pìng"__* verifica la conectividad de red con otro host mediante el envío de paquetes ICMP. Los más usados son:  
<br>
> ping "dirección"
>
![Resultado del comandoo ping](./img/monitorizacion_red/ping.png)  
*__Este comando envía paquetes ICMP al host especificado__*  
<br>
> ping -c 4 "dirección"
>
![Resultado del comandoo ping -c](./img/monitorizacion_red/ping-c.png)  
*__Este comando limita el numero de paquetes enviados, en este caso 4__*  
<br>
> ping -i 2 "dirección"
>
![Resultado del comandoo ping -i](./img/monitorizacion_red/ping-i.png)  
*__Este comando ajusta el intervalo entre paquetes a 2 segundos__*  
<br>

## COMANDO TRACEROUTE  

El comando *__"traceroute"__* muestra la ruta que siguen los paquetes para llegar a un host. Dentro del manual de Linux, los más usados son:  
<br>
> traceroute "dirección"
>
![Resultado del comandoo traceroute](./img/monitorizacion_red/traceroute.png)  
*__Este comando muestra la ruta por defecto hacia la dirección introducida__*
<br>
> traceroute -I "dirección"
>
![Resultado del comandoo traceroute -I](./img/monitorizacion_red/traceroute-I.png)  
*__Este comando usa paquetes ICMP en lugar de UDP__*  
<br>
> traceroute -m 5 "dirección"
>
![Resultado del comandoo traceroute -m](./img/monitorizacion_red/traceroute-m.png)  
*__Este comando limita el número de saltos a 5__*
<br>
