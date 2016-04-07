![Fonds d'ecran sous i3 avec Bob Ross!](images/2016-04-06-i3-wallpapers.jpg)

# i3: terminaux transparents, gestion de fonds d'ecran

i3 wm (Gestionnaire de fenetres). Logiciels utilises: compton, feh.

### Compositeur: Compton

Cette etape est optionnelle si votre terminal gere la transparence de base (chercher dans les options).

Installez le paquet `compton` avec votre gestionnaire de paquets habituel. Par exemple, sous Mint, Ubuntu, Debian: 

		sudo apt-get install compton

Un compositeur permet de modifier l'apparence de vos fenetres, comme ajouter une ombre portee, rendre les fenetres transparents, etc.


- https://fr.wikipedia.org/wiki/Compositeur_%28logiciel%29
- https://wiki.archlinux.org/index.php/Compton

Config: `~/.config/compton.conf`

		opacity-rule = ["90:class_g = 'Termite'"];

**Demarrage automatique de Compton**
https://wiki.archlinux.org/index.php/Compton#Autostarting

Sous i3: `~/.i3/config`

		exec --no-startup-id compton

### Feh: changement du fond d'ecran

Feh: fast and light Imlib2-based image viewer. https://github.com/derf/feh

Installez le paquet `feh` avec votre gestionnaire de paquets habituel. Par exemple, sous Mint, Ubuntu, Debian: 

		sudo apt-get install feh

Mettre une image en fond d'ecran:

		feh --bg-fill image.jpg

Changer aleatoirement le fond d'ecran avec une image provenant d'un repertoire:

		feh --randomize --bg-fill ~/images/wallpapers/*

### Recuperer des fonds d'ecran

- https://www.reddit.com/r/wallpapers
- http://boards.4chan.org/wg/catalog (wallpapers general)
- http://boards.4chan.org/w/catalog (wallpapers anime)
- http://imgur.com/search?q=wallpapers

