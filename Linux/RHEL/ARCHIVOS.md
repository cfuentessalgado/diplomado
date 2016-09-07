## A continuacion describire los principales archivos de configuracion de Distros basadas en RHEL

* **_/etc/host.conf_** : Este archivo se encarga de configurar como se buscan los nombres de dominio, basicamente el orden de busqueda.
```bash
#indica el orden de busqueda
#en este ejemplo primero busca en /etc/hosts y luego en el nameserver o DNS
order hosts,bind

#este parametro indica si algun host tiene permitido multiples ip en /etc/hosts puede ser on/off
multi on

```

* **_/etc/hosts_** : Este archivo se encarga de mapear los hostnames a direcciones IP antes que el DNS (si asi se especifica en /etc/host.conf) o en el caso que no exista un DNS.
```bash
#          IPAddress		FQDN                   	 ALIAS
           127.0.0.1		localhost	 	 deep.example.ex
           208.164.186.1	deep.example.ex		 deep
           208.164.186.2	mail.example.ex		 mail
           208.164.186.3	web.example.ex		 web
```

