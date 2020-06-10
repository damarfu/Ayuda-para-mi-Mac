# Puestas a punto del Mac - mantenimiento
 #Ayuda/MacOS

## Semanal
1. Limpiar caché del Mac con estos comandos de terminal. 
``` 
sudo dscacheutil -flushcache
sudo killall -HUP mDNSResponder
```
2. Ejecutar Clean My Mac con la limpieza automática

## Mensual 
1. Ejecutar Clean My Mac con además eliminar aplicaciones que no uso y opciones avanzadas
2. Purgar la caché desde el terminal. 
``` 
sudo rm -rf ~/Library/Caches/             //Borra las caches del usuario. 
sudo update_dyld_shared_cache -debug      //Borra las cachés dinámicas
sudo update_dyld_shared_cache -force
```

## Semestral
1. Limpiar todas las caches: Apagas el Mac, al encender y empezar a sonar el chime de arranque pulsar Mayúsculas hasta que salga el logotipo de la manzana. Esperar que arranque del todo (arrancará en modo seguro). Una vez terminado el arranque, reiniciar. 

## Anual
1. Limpiar ventiladores
	- 15-11-2019
	- 02-06-2020
## Comandos después de instalar el sistema
1. Suavizado redondeado De Fuentes en pantallas no retina. Abre un terminal y escribe el siguiente comando:
defaults -currentHost write -globalDomain AppleFontSmoothing -int 1
El comando va del 0 al 3 (2 es el que tengo activado para el monitor de 24”) 0 apagado 3 máximo. 
(Con Catalina de momento no me hace falta)

