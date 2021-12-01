# Qué es SSH?

Significa `Secure Shell` que es un protocolo que permite el acceso remoto a una terminal, de un [[Servidor]] o computadora con [[Linux]].

## Creación de cables SSH
Para crear claves SSH, estas normalmente vienen en formato `.pub` que incluyen la informacion. 
En windows se crean mediante programas como *PUTTY*.

#### Linux
En estaciones de trabajo de Linux y macOS, usa la herramienta ssh-keygen para crear un nuevo par de claves SSH. En el siguiente ejemplo, se crea un par de claves RSA.

Abre una terminal y usa el comando ssh-keygen con la marca -C para crear un nuevo par de claves SSH.

```bash
ssh-keygen -t rsa -f ~/.ssh/KEY_FILENAME -C USER -b 2048
```

Reemplaza lo siguiente:

`KEY_FILENAME`: el nombre de tu archivo de claves SSH.

Por ejemplo, un nombre de archivo de `my-ssh-key` genera un archivo de clave privada llamado `my-ssh-key` y un archivo de clave pública llamado `my-ssh-key.pub`.

`USER`: tu nombre de usuario. Por ejemplo, `cloudysanfrancisco@gmail.com` o `cloudysanfrancisco`.

Nota: `USER` no puede ser `root`, a menos que configures tu VM para permitir el acceso raíz. Para obtener más información, consulta Conéctate a instancias como usuario raíz.

`ssh-keygen` guarda el archivo de claves privadas en `~/.ssh/KEY_FILENAME` y el archivo de claves públicas en `~/.ssh/KEY_FILENAME.pub`

## Conexión por medio SSH usando una clave

```bash
ssh -i PATH_TO_PRIVATE_KEY EXTERNAL_IP
```