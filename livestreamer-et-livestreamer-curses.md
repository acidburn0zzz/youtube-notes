
![Twitch streame darks souls 3 semaines avant sa sortie](images/2016-03-23-livestreamer-twitch.jpeg)

# Livestreamer

Permet de streamer divers sites via votre lecteur video tels que Twitch, Crunchyroll, Dailymotion, Livestream, UStream, YouTube Live pour ne citer que les plus connus. 

- Site officiel: https://github.com/chrippa/livestreamer
- Doc: http://docs.livestreamer.io/

### Installation

		$ sudo pip install livestreamer

### Configuration

Fichier a editer: ~/.config/livestreamer/config
	
		default-stream best
		player=mpv
### Options

- Changer la quality du flux video:

		$ livestreamer twitch.tv/day9tv source
		audio, high, low, medium, mobile (worst), source (best)

# Livestreamer-curses

TUI (text user interface) pour livestreamer.

- Site officiel: https://github.com/gapato/livestreamer-curses

### Installation

		$ sudo pip install livestreamer-curses

### Configuration

- Fichier a editer: ~/.config/livestreamer-curses/livestreamer-cursesrc
- Reference: https://raw.githubusercontent.com/gapato/livestreamer-curses/master/livestreamer-cursesrc.sample

		CHECK_ONLINE_ON_START = True

		# 0 pour desactiver
		CHECK_ONLINE_INTERVAL = 60

- Fichier base de donnees: ~/.local/share/livestreamer-curses/livestreamer-curses.db

### Commandes

		? aide
		j/k bas/haut pour se deplacer
		entrer pour lancer la video

		a ajout
		r qualite
		
		o voir/cacher les streams hors lignes


