# Cosas basicas de VIM

En este caso, siempre prefiero usar neovim. Es mas genial para mi gusto y mas personalizable.
Normalmente esto se usa en [[Linux]]

## Ubicación del archivo de cnf

`~/.config/nvim/init.vim`

## Comando basicos de VIM

- `gg` ir a comienzo de documento
- `e` para ir final de palabra
- `0` comienzo de linea
- `$` final de lineak
- `CTRL+W <teclas de direccion>` para moverse entre buffers.
- `G` final de documento
- `CTRL +n` Abre NERDTREE
- `,ff` ABre buscador
- `,s` abre navegacion por palabras
- `o` agregar nueva linea
- `s` nerd tree open split windows****

# Instalar Lunar Vim
### Primero instalar NeoVim 0.6 en adelante con:
1. Descargar el AppImage de neovim 0.6 desed github.
2. Crear una clave simbólica con el comando: 
	1. `ln -s <full path to nvim.appimage> /home/<username>/.local/bin/nvim ` 
3. Probar si neovim funciona.
4. Instalar la version de NodeJS. Esto se hace con el siguiente comando.
5. `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash`
	`source ~/.bashrc`
	`nvm install 16`
	`npm install -g npm  # update npm`
	
7. Instalar Nerdfonts. 
8. Ya esta :v

links: https://stackoverflow.com/questions/10081293/install-npm-into-home-directory-with-distribution-nodejs-package-ubuntu

https://github.com/neovim/neovim/wiki/Installing-Neovim

https://www.lunarvim.org/01-installing.html#prerequisites
https://github.com/LunarVim/LunarVim




	
	