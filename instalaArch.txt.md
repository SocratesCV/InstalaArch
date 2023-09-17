** Alagunas configuraciones sencillas al instalar de nuevo ArchLinux u otras distribuciones. **

# Iso
# dd #ISO #pendrive
https://archlinux.org/download
wget http://mirror.librelabucm.org/archlinux/iso/2023.04.01/archlinux-2023.04.01-x86_64.iso
lsblk
sudo dd bs=4M if=archlinux-2023.04.01-x86_64.iso of=/dev/sdb conv=fsync oflag=direct status=progress


# Aplicaciones consola:
sudo pacman -S imagemagick neofecth

## Neofetch
Temas:https://github.com/Chick2D/neofetch-themes
Fuente:https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/NerdFontsSymbolsOnly.zip
~/.local/share/Font
## imagemagick 
aplicación para automatizar acciones con imagenes (imstagram)
## Terminal
Tengo que escoger una consoloa definitiva, seguiré probando.
Opacidad 90%
Tecla de acceso rápido ctrl+alt+t o sup+Enter

# Notas
sudo pacman -S obsidian dropbox 

## Dropbox
Al configurar te pedirá un código numerico que te envía al movil en un mensaje.
Sincronizar algunas carpetas con dropbox, solo marcar las necesarias.
La carpeta notas la utilizará obsidian.
## Obsidian
Aplicacion para tomar notas.
Sincronizarla con la carpeta notas de dropbox.


# Programacion
sudo pacman -S neovim git pycharm

## neovim 
Editor de texto para consola.
Añadir configuraciones...
## git
Gestor de versiones
## pycharm 
Para programar en python, también habrá que haber instalado python.


# Ofimatica
sudo pacman -S calibre libreoffice

## calibre
Gestión de bibliotecas.
Añadir la base de datos de los libros del backup, y hacer un backup de vez en cuando.
## libreOffice
ofimatica, sin más.


# Seguridad
sudo pacman -S bitwarden
## bitwarden
gestor de contraseñas, se guardan online.

# Redes sociales
sudo pacman -S telegram-desktop
## telegram
Cofigurarlo leyendo un codigo qr con el movil.

# Multimedia
sudo pacman -S vlc
## vlc
Reproductor audio y video


# AMD # Drivers # AMDGPU
sudo pacman -S xf86-video-amdgpu vulkan-radeon lib32-vulkan-radeon opencl-mesa libva-mesa-driver lib32-libva-mesa-driver mesa-vdpau lib32-mesa-vdpau --needed

# Intel # Drivers # IntelGPU
sudo pacman -S xf86-video-intel vulkan-intel lib32-vulkan-intel opencl-mesa libva-mesa-driver lib32-libva-mesa-driver mesa-vdpau lib32-mesa-vdpau --needed

# Nvidia # Drivers # NvidiaGPU
sudo pacman -S nvidia nvidia-settings nvidia-utils lib32-nvidia-utils cuda opencl-nvidia  lib32-opencl-nvidia vdpauinfo clinfo  --needed


# imInstagram
Script para modificar las fotos para instagram, tengo el scrip en github
mkdir ./Imágenes/iminstagram
git https://github.com/SocratesCV/ImagenInstagram.git ./imágenes/iminstagram/




# VARIOS

## Pacman
sudo pacman -Syyu
sudo pacman -S
sudo pacman -R
sudo pacman -Ss
sudo pacman -Scc
--needed --noconfirm

