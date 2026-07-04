#wpp-auto

PT-BR
Script simples pra alternar wallpapers no KDE Plasma com base no horario do dia. Compativel com diversas telas.

## Requisitos
- KDE Plasma
- qdbus6 ou qdbus
- Bash

#Estrutura das pastas

-Por padrão, o script espera que os wallpapers estejam dentro de:

~/Imagens/wpp

A organização basica usa duas pastas:

~/Imagens/wpp/
|- d/ #Wallpaper para o periodo do dia
|- n/ #Wallpaper para o periodo da noite

Exemplo:

~/Imagens/wpp/
|- d/
|  |- wallpaper-dia-1.png
|  |- wallpaper-dia-2.jpg
|
|
|- n/
|  |- wallpaper-noite-1.png
   |- wallpaper-noite-2.jpg


Também é possivel usar wallpapers diferentes para cada tela.

A estrutura de pastas então seria:
~/Imagens/wpp/
|---t1/ # Primeira tela
|   |-d/
|   |-n/
|
|---t2/ # Segunda tela
|   |-d/
|   |-n/


## Uso

Dê permissão de execução do script:

 " chmod +x wpp-auto "

e então execute
 " ./wpp-auto "


#Inicialização Automática
 Adicione o script á inicialização automática do KDE PLasma ou crie um serviço de usuário com o "systemd"

OBS: O script não inclui wallpapers. Ele apenas procura na pasta configurada e escolhe qual aplicar dependendo da hora.


ENG

Simple script to switch wallpapers on KDE Plasma based on the time of day. Currently made for dual  screens. (Soon will have single and multiple setup, else you could add a new folder structure to the script)

#Requirements
KDE Plasma
qdbus6 or qdbus
Bash

#Folder structure

-By default, the script expects the wallpapers to be inside:

~/Imagens/wpp

The basic organization uses two folders:

~/Imagens/wpp/
|- d/ #Wallpaper for the daytime period
|- n/ #Wallpaper for the nighttime period

Example:

~/Imagens/wpp/
|- d/
| |- wallpaper-day-1.png
| |- wallpaper-day-2.jpg
|
|
|- n/
| |- wallpaper-night-1.png
|- wallpaper-night-2.jpg

It is also CURRENTLY MADE TO USE WITH DUAL MONITOR SETUPS!. Later will be added support for single-monitors, or else you could just follow the following folder structure, even without a second monitor:

The folder structure would then be:
~/Imagens/wpp/
|---t1/ # First screen
| |-d/
| |-n/
|
|---t2/ # Second screen
| |-d/
| |-n/

Usage

Give the script execution permission:

" chmod +x wpp-auto "

and then run
" ./wpp-auto "

#Automatic Startup
Add the script to KDE Plasma automatic startup or create a user service with the command "systemd"

NOTE: The script does not include wallpapers. It only searches the configured folder and chooses which one to apply depending on the time.

## License

No license added yet...

Thank you/Obrigado
