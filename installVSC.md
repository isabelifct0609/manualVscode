

### INSTALACION DE VSC


El editor de texto VSCode ha sido creado y es mantenido por Microsoft. Lo distribuye con licencia Open Source y por lo tanto en forma gratuita. Lo debemos descargar del sitio code.visualstudio.com, como podemos comprobar está disponible tanto para Windows, Mac y Linux.

##### INSTALACION EN LINUX

Paso 1
Descargar el editor de su página Web: https://code.visualstudio.com/Download

Paso 2
Descomprimir el contenido del archivo comprimido y almacenarlo en una carpeta determinada:
sudo unzip VSCode-linux-x64.zip -d /opt/vscode
Lo que hace este comando es descomprimir el contenido del archivo VSCode-linux-x64.zip en la carpeta /opt/vscode. Con el parámetro -d le indicamos que cree la carpeta en caso de que no exista.

Paso 3
Ahora toca crear el acceso directo para no tener que ejecutar siempre la expresión ./Code. Tal y como he mencionado antes, vamos a seguir este tutorial y, en el archivo con extensión .desktop añadimos el siguiente contenido:
[Desktop Entry]
Name=Visual Studio Code
Comment=Editor de código Visual Studio Linux
Exec=/opt/vscode/Code
Icon=/opt/vscode/resources/app/vso.png
Terminal=false
Type=Application.

Una vez hecho esto, ya podremos ejecutar Visual Studio Code desde un acceso directo.

Para los usuarios más novatos de Gnu/linux, os escribimos a continuación el código que hay que ejecutar para instalar el paquete dependiendo de la distribución que tengamos:

Debian / Ubuntu:

``` sh
$ sudo dpkg -i file.deb
```

```sh
$ sudo apt-get install
```

OpenSUSE/ Fedora/ Red Hat Linux:

```sh
$ sudo yum install file.rpm
```

Paquete tar.gz:

```sh
$ cd /bin
```
```sh
$ sudo code
```

Estos comandos sobre la terminal de nuestra distribución nos permitirá instalar Visual Studio Code en nuestra distribución Gnu/Linux o al menos utilizarlo de manera funcional.