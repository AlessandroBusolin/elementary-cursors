<p align="center">
<img src="https://github.com/AlessandroBusolin/elementary-cursors-for-Linux-Mint/blob/master/src/cursors/Linux_Mint_Official_Logo.png">
</p>

[![GitHub release][version-image]][version-url]

elementary Cursor Theme redesigned for Linux Mint.
==================================================
### Preview

<p align="center">
<img src="https://github.com/AlessandroBusolin/elementary-cursors-for-Linux-Mint/blob/master/preview/elementary.png">
</p>

### General informations

A cursor theme for elementary OS redesigned for Linux Mint.

These cursors are free artwork; you can redistribute them and/or modify them under the terms of the [GNU General Public License version 3](http://www.gnu.org/licenses/gpl.txt).

### Installing 

Copy the 'elementary' folder into '/usr/share/icons', then set your cursor theme using your favourite tool or:

    gsettings set org.gnome.desktop.interface cursor-theme 'elementary'

But to make a system-wide change run the following:

    sudo update-alternatives --install /usr/share/icons/default/index.theme x-cursor-theme /usr/share/icons/elementary/cursor.theme 13
    sudo update-alternatives --set x-cursor-theme /usr/share/icons/elementary/cursor.theme

Then log out and back in for the changes to take effect.

For manual installation, you may have to change the copied files' permissions (to 755) after copying in order to use the theme.

### Using the Source

There are scripts to simplify the rendering process; to run them (and edit icons) you will need:

 * inkscape
 * python

To render the cursor theme from the [source plate](src/cursors/elementary.svg) you will need to run the render script in [src/cursors](src/cursors):
	
	cd src/cursors
    python renderpngs.py elementary.svg

Then make the theme by running the make script in the [src/cursors/pngs](src/cursors/pngs) folder:

	cd src/cursors/pngs
    bash make.sh

-----------

"elementary Cursor Theme" ridisegnato per Linux Mint.
=====================================================

### Anteprima

<p align="center">
<img src="https://github.com/AlessandroBusolin/elementary-cursors-for-Linux-Mint/blob/master/src/cursors/elementary.svg">
</p>

### Informazioni generali

Un tema per il cursore di elementary OS ridisegnato per Linux Mint.

Questi cursori sono opere d'arte gratuite; li puoi redistribuire e/o modificare secondo i termini della [GNU General Public License version 3](http://www.gnu.org/licenses/gpl.txt).

### Installazione

Copia la cartella 'elementary' dentro '/usr/share/icons', quindi imposta il cursore usando il tuo programma/strumento preferito oppure:

    gsettings set org.gnome.desktop.interface cursor-theme 'elementary'

Per impostare il pacchetto di cursori come il predefinito di sistema, esegui i seguenti comandi:

    sudo update-alternatives --install /usr/share/icons/default/index.theme x-cursor-theme /usr/share/icons/elementary/cursor.theme 13
    sudo update-alternatives --set x-cursor-theme /usr/share/icons/elementary/cursor.theme

Quindi effettua il log out per rendere effettivi i cambiamenti.

Per l'installazione manuale, potrebbe essere necessario modificare le autorizzazioni dei file copiati (impostando il valore a 755) dopo la copia, per poter utilizzare il tema.

### Usare il sorgente

Ci sono degli script che semplificano il processo di rendering; per avviarli (e modificare le icone) ti servono:

 * inkscape
 * python

Per fare il render del tema del cursore da [source plate](src/cursors/elementary.svg) ti serve eseguire lo script di render in [src/cursors](src/cursors):

	cd src/cursors
    python renderpngs.py elementary.svg

Quindi crea il tema attraverso l'esecuzione dello script "make" nella cartella [src/cursors/pngs](src/cursors/pngs): 

	cd src/cursors/pngs
    bash make.sh

-----------

<!-- Markdown link & img dfn's -->
[version-image]: https://img.shields.io/github/release/AlessandroBusolin/elementary-cursors-for-Linux-Mint.svg?style=flat-square

[total-image]: https://img.shields.io/github/downloads/AlessandroBusolin/elementary-cursors-for-Linux-Mint/total.svg

[version-url]: https://github.com/AlessandroBusolin/elementary-cursors-for-Linux-Mint/releases/latest
