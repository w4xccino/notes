
# The most useful commands for me
- `cd` para moverse entre carpetas
- `chmod` cambia los permisos de archivos `-R` para que sea recursivo.
- `mount` ,`umount`,`remount` para montar y desmontar unidades
- `blkid` para ver las unidades  montadas. 
- `ls` para ver archivos `-la` para archivos escondidos.
- `top` para mostrar procesos.
- `flatpak` es un gestor de paquetes multi-distribucion.
- `mv` para mover archivos.
- `cp` copiar archivos
- `rmdir` elimina carpetas
- `rm -rf` comando de eliminacion
- `pwd` muestra la ubicacion actual
- `wget <url>` descargar archivos. 
- `screen` instancias separadas de terminal 
- `find . -name <name>` Buscar en la carpeta actual por nombre
	- `service <process_name> status` ver si un proceso está siendo ejecutado
	- `ps aux | grep <process_name>` ver si un proceso está siendo ejecutado
- `which` para obtener la locacion de otro comando 
- `du -h` . ver peso de la carpeta actal.
# Locaciones importantes
- `/etc/fstab` es un archivo para modificar las particiones y discos.
- `/boot/grub/grub.conf` archivo para modificar el grub.
- `/etc/apt/sources.list.d/` carpeta para repositorios


## PATH
### PATH TEMPORAL
- `echo $PATH` Ver al path
- `export PATH="$PATH:<location>"` Agregar al path
### PATH PERMATENTE
Editar cualquiera de estos dos archivos con los comandos de arriba:
- `source ~/.bashrc`
- `source ~/.profile`
## shortcuts
- `shift` + `CAPS LOCK` cambiar el layout del teclado. Muy util


# GIT
- `git config credential.helper store`Guardar credenciales de github

# Alacritty
`alacritty-themes` configura los colorcitos del alacritty

