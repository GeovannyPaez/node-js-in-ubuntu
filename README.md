
## Primero descargamos la la ultima version de node en la pagina principal

 - [Node Js](https://nodejs.org/es)

## Instalacion

Vamos a la carpeta de descargas y descomprimimos el archivo con tar

```bash
  1. $ cd ~/Descargas
  2. $ tar -xf node-v18.16.0-linux-x64.tar.xz
```
Movemos el archivo descomprimido al home y lo renombramos como "nodejs"
```bash 
    $ mv node-v18.16.0-linux-x64 ~/nodejs
```    
nos ubicamos donde esta la carpeta de nodejs que es en el home ejecutamos pwd para saber donde queda la ruta del ejecutable de node.
```bash 
   1. $ cd ..
   2. $ cd nodejs/bin
   3. $ pwd
    // /home/[user]/nodejs/bin
```
  

guardamos la ruta y volvemos al home.
```bash 
   4. $ cd ..
   5. $ cd .. 
   6. paez@paez-Nitro-AN515-44:~$ pwd
      /home/paez

```   
 ejecutamos el comando nano para editar el archivo .bashrc
```bash 
   4. $ nano .bashrc

```   
Una vez ejecutado el comando nano, nos abrira un archivo en cosola y simplemente hacemos scroll hasta el final del archivo. 

Ahi lo que hay que hacer es exportar una variable PATH que contenga la ruta de node js y asi poder ejecutarlo desde cualquier lugar en la consola. 

En la varible PATH colocamos la ruta del archivo de nodejs y la exportamos.
```bash 
 # enable programmable completion features (you don't need to enable
# this, if it's already enabled in /etc/bash.bashrc and /etc/profile
# sources /etc/bash.bashrc).
if ! shopt -oq posix; then
  if [ -f /usr/share/bash-completion/bash_completion ]; then
    . /usr/share/bash-completion/bash_completion
  elif [ -f /etc/bash_completion ]; then
    . /etc/bash_completion
  fi
fi
export PATH=$PATH:/home/paez/nodejs/bin

``` 
Despues damos guardamos los cambios con Control X, aceptar y Enter para salir de la consola.

Cerramos la consola y ejecutamos.
```bash 
   paez@paez-Nitro-AN515-44:~$ node -v
   v18.16.0


```   
