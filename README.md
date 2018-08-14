English: 
Hello, to start speaking in Spanish, that's why I apologize for my bad dialect in English.
I want to show you a Script that I did recently, it has a single fault. When you restart the script you have to change the name of the mkdir since this is the folder creation command, if someone can solve it, I would appreciate it.
I hope you like it, the instructions are in Spanish within the script but I will do a translation in English translated.
My email is b1nary01@outlook.com
Español:
hola,
Les quiero mostrar un Script que hice hace poco, tiene una unica falla. Cuando reinicias el script tienes que cambiarle el nombre de el mkdir ya que este es el comando de creacion de carpetas, si alguien lo puede solucionar les agradeceria.
mi email es b1nary01@outlook.com

Es Solo para LINUX y debes tener estas herramientas instaladas
youtube-dl, install: sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-
y luego
-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-
sudo chmod a+rx /usr/local/bin/youtube-dl
---------------------------------------------------------------
ffmpeg, install: sudo apt-get install ffmpeg 
-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-
y luego
-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-.-
sudo youtube-dl -U
--------------------------------------------------------------
copiar y pergar en el terminal de LINUX para instalar Youtube-dl y ffmpeg
--------------------------------------------------------------

----------------------Copiar y pegar en Sublime text------------------------------------
#1/bin/bash
clear;
cd Escritorio;
cd musica_descargada;
echo "---------------------------------------------------------------------------"
echo -e ' $$$$$$$$\        $$\                 $$\      $$\            $$$$$$\   '
echo -e ' \__$$  __|       $$ |                $$$\    $$$ |          $$ ___$$\  '
echo -e '    $$ |$$\   $$\ $$$$$$$\   $$$$$$\  $$$$\  $$$$ | $$$$$$\  \_/   $$ | '
echo -e '    $$ |$$ |  $$ |$$  __$$\ $$  __$$\ $$\$$\$$ $$ |$$  __$$\   $$$$$ /  '
echo -e '    $$ |$$ |  $$ |$$ |  $$ |$$$$$$$$ |$$ \$$$  $$ |$$ /  $$ |  \___$$\  '
echo -e '    $$ |$$ |  $$ |$$ |  $$ |$$   ____|$$ |\$  /$$ |$$ |  $$ |$$\   $$ | '
echo -e '    $$ |\$$$$$$  |$$$$$$$  |\$$$$$$$\ $$ | \_/ $$ |$$$$$$$  |\$$$$$$  | '
echo -e '    \__| \______/ \_______/  \_______|\__|     \__|$$  ____/  \______/  '
echo -e '                                                  $$ |                  '
echo -e '                                                  $$ |                  ' 
echo -e '                                                  \__|                  '
echo "-----------------------------------NICO------------------------------------"
echo -e "\e[35m NOTA 1 : NO PONER VIDEOS DIRECTO DE UNA LISTA DE REPRODUCCION \e[0m"
echo "."
echo -e "\e[35m NOTA 2 : RECUERDA PONER NOMBRE DEL ARTISTA Y TEMA \e[0m"
echo "."
echo -e "\e[35mAHORA SE CREARA UNA CARPETA DONDE SE GUARDARA LA MUSICA - Nombre de carpeta "Musica" \e[0m"
read -p "¿ESTA DE ACUERDO CON ESTO? (y/n) : "
mkdir "Musica $carpeta"
cd "Musica $carpeta"
sleep 3
function Descarga {
	echo " "
	read -p 'INTRODUCE LINK DE YOUTUBE: ' fuente
	echo " "
	echo -e "\e[0;33mPONE EL NOMBRE DEL AUTOR Y EL TEMA (EJEMPLO : Metallica - The Unforgiven)\e[0m"
	echo " "
	read -p 'NOMBRE Y TITULO: ' nombre
	echo " "
	}

	while true
do

	Descarga

	echo " "
	echo -e "\e[33m ######################################################### "
	echo -e "\e[33m # BUSCANDO LA CANCION SELECCIONADA NO CIERRE LA VENTANA # "
    echo -e "\e[33m ######################################################### "
    echo " "
	youtube-dl -x --audio-format mp3 $fuente -o youtube.mp3
	echo " "
echo -e "\e[31mRenombrando la pista por el nombre puesto por usted\e[0m"
echo " "
sleep 4
mv youtube.mp3 "$nombre.mp3"
echo -e "\e[0;33mDESCARGA TERMINADA- INTRODUCE OTRO ZELDA O CIERRA VENTANA."
done
