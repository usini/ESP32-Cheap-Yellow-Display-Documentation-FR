# Dépannage

## Premièrement, assurez-vous que c'est un CYD !

Si vous rencontrez des problèmes, c'est la première chose à vérifier !

Les exemples et informations contenus dans ce dépôt sont uniquement pour l'affichage **ESP32-2432S028**. Le numéro de modèle est écrit au dos de l'affichage en lettres dorées, à côté du connecteur du haut-parleur.

## L'écran ne s'allume pas

Si vous avez des problèmes pour faire fonctionner l'affichage, la première chose que je tenterais est de [webflasher un projet existant](PROJECTS.md#projects-1). Ce seront des codes connus pour fonctionner, et si cela fonctionne correctement, cela indique un problème logiciel, pas matériel.

### Si le projet webflash affiche quelque chose à l'écran

- Assurez-vous d'avoir mis le fichier [User_Setup.h](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/DisplayConfig/User_Setup.h) au bon endroit [comme décrit ici](/SETUP.md#library-configuration)
- La broche 21 est la broche de rétroéclairage, assurez-vous de ne pas l'utiliser pour autre chose dans votre croquis.

### Le projet webflash n'affiche rien à l'écran

- Assurez-vous de ne rien connecter sur la broche 21. Elle est déportée sur le connecteur étiqueté `P3`
- Essayez une autre alimentation USB et/ou un autre câble
- Si rien d'autre n'a fonctionné, votre CYD pourrait être défectueux. Contactez le vendeur.

## L'écran scintille

- Essayez une autre alimentation USB et/ou un autre câble
- Suivez les étapes de la section [L'écran ne s'allume pas](#L'écran-ne-s'allume-pas)
- Si rien d'autre n'a fonctionné, votre CYD pourrait être défectueux. Contactez le vendeur.