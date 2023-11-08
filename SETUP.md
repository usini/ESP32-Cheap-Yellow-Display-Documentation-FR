# Configuration et paramétrage

Cette page couvrira les bases de la configuration du CYD.

## Installation matérielle

Il n'y a vraiment rien à configurer ici, il suffit de connecter le CYD à un ordinateur à l'aide d'un câble micro USB (fourni avec la carte).

## Installation logicielle

Le pilote doit être configuré pour téléverser vers le CYD, y compris pour flasher à partir d'une page web les projets.

### Pilote

Le CYD utilise la puce CH340 USB vers UART. Si vous n'avez pas déjà installé de pilote pour cette puce, vous devrez peut-être en installer un. Consultez [le guide d'installation de Sparkfun](https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all) pour obtenir les instructions.

## Configuration pour la programmation

Suivez ces instructions si vous souhaitez écrire du nouveau code pour le CYD.

### Définition de la carte

Vous aurez besoin de configurer l'ESP32 pour votre IDE Arduino, [les instructions peuvent être trouvées ici](https://docs.espressif.com/projects/arduino-esp32/en/latest/installing.html).

Vous pouvez ensuite sélectionner pratiquement n'importe quelle carte ESP32 dans le menu des cartes. (J'utilise généralement "ESP32 Dev Module", mais cela n'a pas vraiment d'importance)

Si vous rencontrez des erreurs lors du téléchargement d'un sketch, essayez de régler la vitesse de téléchargement de la carte à `115200`.

### Configuration de la bibliothèque

Le CYD peut fonctionner avec une sélection de différentes bibliothèques, mais la principale sur laquelle ce dépôt se concentre est [TFT_eSPI](https://github.com/Bodmer/TFT_eSPI) car c'est une bibliothèque assez populaire pour travailler avec ce type d'affichages et il y a beaucoup d'exemples.

Cela peut être installé depuis le gestionnaire de bibliothèques en cherchant "TFT_eSPI".

 > Note : Après l'installation de la bibliothèque, copiez le fichier [User_Setup.h](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/blob/main/DisplayConfig/User_Setup.h) dans le dossier Arduino `libraries\TFT_eSPI`. Cela configure la bibliothèque pour être utilisée avec cet affichage.

### Exemples

J'ai fourni des exemples pour que vous puissiez les essayer afin d'obtenir des idées ou de l'inspiration. [Consultez-les ici.](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/)