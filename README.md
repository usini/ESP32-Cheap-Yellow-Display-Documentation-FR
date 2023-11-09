# ESP32-Cheap-Yellow-Display

[Lien vers le projet (Anglais)](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display)

Il existe un ESP32 avec un écran LCD intégré de 320 x 240 tactile, appelé "ESP32-2432S028R", mais comme ce n'est pas très facile à prononcer, je propose de le renommer "Cheap Yellow Display" ou CYD pour faire court. Cet afficheur coûte seulement dans les 15$ avec la livraison, donc je pense qu'il représente une très bonne affaire.

![image](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/assets/1562562/76c3d481-2523-4b6f-881c-2e29f9368cd0)

## Caractéristiques

Le CYD a les caractéristiques suivantes :

- ESP32 (Avec Wifi et Bluetooth)
- Écran LCD de 320 x 240 (2.8")
- Écran tactile (résistif)
- USB pour l'alimentation et la programmation
- Un lecteur de carte microSD, une LED RGB et quelques broches supplémentaires sont disponibles

## Pour qui est-ce utile ?

Je pense qu'il est utile pour les types de personnes suivants :

- **Les débutants en carte de développement électronique** - tout est déjà connecté, il n'y a pas besoin de souder ni de composants supplémentaires
- **Les personnes qui ont l'habitude de travailler avec du matériel informatique, mais qui ont la flemme** - (comme moi) Parfois, on veut juste construire un projet sans avoir à assembler du matériel
- **Les personnes qui ne cherchent pas vraiment à apprendre, mais qui veulent juste créer des choses cool** - Plus à ce sujet plus tard.

## Quel est le but de cette page ?

C'est un matériel plutôt sympa et à bon prix, mais les instructions/logiciels qui l'accompagnent sont assez pauvres. Juste un lien vers un fichier zip sur un site internet random.

Il y a quelques années, j'ai sorti [ESP32 Trinity](https://github.com/witnessmenow/ESP32-Trinity), qui est une carte ESP32 open source pour contrôler des matrices de LED. Je pense que le principal avantage du travail que j'ai fait sur le Trinity n'est pas le matériel, mais la documentation, les exemples de code et les projets prêts à l'emploi.

Je ne crée plus de produits matériels, mais je pense qu'il serait intéressant de créer le même type de communauté autour de cet afficheur, où les gens peuvent partager des exemples et des projets réalisés pour cet afficheur.

## Où l'acheter ?

Voici quelques liens pour acheter la carte, choissisez celui qui vous revient le moins cher :

- [Aliexpress\*](https://s.click.aliexpress.com/e/_DkSpIjB)
- [Aliexpress\*](https://s.click.aliexpress.com/e/_DkcmuCh)
- [Aliexpress](https://www.aliexpress.com/item/1005004502250619.html)
- [Makerfabs](https://www.makerfabs.com/sunton-esp32-2-8-inch-tft-with-touch.html) - Il semble être vendu avec une carte SD de 16GB. Makerfabs stocke aussi mon [ESP32 Trinity](https://github.com/witnessmenow/ESP32-Trinity) (NOTEZ qu'il y aura des droits d'importation dans l'UE pour makerfabs)

\* = Lien d'affiliation

## Commencer avec votre CYD

Pour plus de détails sur la façon de commencer avec votre CYD, veuillez consulter la page [Configuration et Installation](SETUP.md)

## Exemples de Code

### Les Bases

Une collection d'exemples montrant comment utiliser les différentes fonctionnalités du CYD, c'est un bon point de départ. [Consultez-les ici.](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/Basics)

### Bibliothèques d'Affichage Alternatives

Les exemples de bases sont basés sur la bibliothèque d'affichage TFT_eSPI, mais le CYD fonctionne également avec d'autres bibliothèques d'affichage. Voici un code d'exemple si vous préférez utiliser une bibliothèque Arduino alternative. [Consultez-les ici.](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/AlternativeLibraries)

### ESPHome

Des exemples pour utiliser le CYD dans ESPHome. [Consultez-les ici.](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/ESPHome)

## Informations et Liens Supplémentaires

### Discord

Rejoignez la discussion sur l'AYE dans [mon canal Discord](https://discord.gg/nnezpvq)

### Impression 3D

Des exemples de supports et de boîtiers imprimés en 3D. [Consultez-les ici.](/3dModels)

### Informations sur les Pins

[Cette page](PINS.md) contient des informations sur les broches utilisées, et celles qui sont libres d'utilisation.

### Add-ons

[Cette page](ADDONS.md) contient des informations sur les add-ons matériels supplémentaires qui peuvent augmenter les fonctionnalités de votre CYD

### Dépannage

[Cette page](TROUBLESHOOTING.md) contient des informations sur comment dépanner le CYD

### Modifications Matérielles

[Cette page](Mods/README.md) contient des informations sur certaines modifications matérielles qui peuvent être réalisées sur le CYD pour améliorer ou changer certaines de ses fonctionnalités.

### Médias et Mentions Vidéo

[Cette page](MEDIA.md) répertorie toutes les fois où le projet CYD a été mentionné quelque part !

## Informations sur la Licence

Ce projet est sous licence MIT comme indiqué dans le [fichier de licence](/LICENSE)

La seule exception à cela est le dossier [OriginalDocumentation](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/OriginalDocumentation/) pour lequel je n'ai pas le droit d'accorder une licence

## Aidez à Soutenir ce que je fais !

[Si vous appréciez mon travail, vous pouvez me sponsoriser sur Github !](https://github.com/sponsors/witnessmenow/)
