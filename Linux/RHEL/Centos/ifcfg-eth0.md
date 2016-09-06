Ubicacion del Archivo: **/etc/sysconfig/network-scripts/ifcfg-eth0**

**El nombre de este archivo dependera exclusivamente del nombre de la interfaz de red que se pretenda modificar. Estas pueden variar, algunos ejemplos son: _eth0,enp0s3,wlan0,em0. etc..._**

**La siguiente es la estructura de lo que debemos escribir en este archivo:**

```bash
BOOTPROTO="static"
DEVICE="[Escribir el nombre de la interfaz de Red]"
ONBOOT="yes"
IPADDR = "[Escribir la IP que se desea asignar aqui]"
NETMASK="[Escribir la mascara de red]"
GATEWAY = "[Escribir la Pasarela Predeterminada Aqui]"
DNS1 = "[Servidor DNS principal]"
DNS2 = "[Servidor DNS secundario]"

```

Digamos por ejemplo que queremos configurar nuestro servidor con la siguiente configuracion estatica para la interfaz de red **enp0s3**:

* ip **192.168.0.200**
* mascara de red **255.255.255.0**
* pasarela **192.168.0.1**
* dns principal **8.8.8.8**
* dns secundario **8.8.4.4**

### El archivo de configuracion (**/etc/sysconfig/network-scripts/ifcfg-enp0s3**)entonces deberia quedar asi:

```bash
BOOTPROTO="static"
DEVICE="enp0s3"
ONBOOT="yes"
IPADDR = "192.168.0.200"
NETMASK="255.255.255.0"
GATEWAY = "192.168.0.1"
DNS1 = "8.8.8.8"
DNS2 = "8.8.4.4"

```
