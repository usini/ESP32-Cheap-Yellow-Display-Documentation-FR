# Add-ons

Voici une liste d'extensions matérielles supplémentaires qui peuvent augmenter les fonctionnalités de votre CYD.

## Sniffer Carte SD

Si vous souhaitez utiliser les broches de la carte SD pour brancher autre chose, le moyen le plus simple est d'utiliser un "SD Card Sniffer", qui se branche dans l'emplacement pour carte SD et rend les broches accessibles. C'est particulièrement utile pour les appareils qui se connecte en SPI.

## Brochage de la carte Sniffer

| Étiquette sur la carte | Broche ESP32 | Utilisation SPI |
| ---------------------- | ------------ | --------------- |
| DAT2                   | -            | -               |
| CD                     | IO5          | CS              |
| CMD                    | IO23         | DI / MOSI       |
| GND                    | GND          | -               |
| VCC                    | 3.3V         | -               |
| CLK                    | IO18         | SCLK            |
| DAT0                   | IO19         | DO / MISO       |
| DAT1                   | -            | -               |

### Liens

- [Micro SD Card Sniffer - Aliexpress\*](https://s.click.aliexpress.com/e/_Ddwcy9h)

## Nunchuck Nintendo Wii

Un contrôleur Nunchuck d'une Nintendo Wii est un excellent dispositif de contrôle pour les projets CYD car ils sont peu coûteux et, puisqu'ils utilisent l'i2c pour la communication, ils ne requièrent que 2 broches GPIO pour la connexion.

Avec ces deux broches, vous obtenez :

- Un joystick analogique
- 2 Boutons
- Un accéléromètre

## Matériel Requis

### Contrôleurs Nunchuck

Ceux officiels de Nintendo sont généralement de meilleure qualité (peut-être essayer les options d'occasion), mais les copies fonctionnent aussi bien.

- [Recherche sur Amazon.co.uk\*](https://amzn.to/3nQrXcE)
- [Recherche sur Amazon.com\*](https://amzn.to/3nRJTUd)
- [Aliexpress (Tiers)\*](https://s.click.aliexpress.com/e/_AaQbXh)

### Contrôleurs Nunchuck

Il y a de nombreuses options disponibles pour ceux-ci, même les moins chers d'Aliexpress fonctionnent parfaitement.

- [Aliexpress](https://s.click.aliexpress.com/e/_AEEtc3)
- [Mon modèle open source de Oshpark](https://oshpark.com/shared_projects/RcIxSx2D)
- [Adafruit](https://www.adafruit.com/product/4836)

## Câblage

Le moyen le plus simple de réaliser ce câblage est d'utiliser le câble fourni avec le CYD et le connecteur JST **CN1** (celui le plus proche de l'emplacement de la carte Micro SD)

Connectez le câble à votre carte d'adaptation comme suit :

| CN1 CYD | Adaptateur | Note                      |
| ------- | ---------- | ------------------------- |
| GND     | - (GND)    | Fil noir pour moi         |
| 3.3V    | + (3V)     | Fil rouge pour moi        |
| IO22    | d (SDA)    | Fil bleu pour moi         |
| IO27    | c (SCL)    | Fil jaune pour moi        |

Note : J'ai constaté que les résistances de pull-up ne sont pas nécessaires sur SDA et SCL.

## Exemple

Consultez l'exemple [NunchuckTest](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/InputTests/NunchuckTest) pour voir comment l'utiliser.

## Haut-parleurs

Un haut-parleur peut être connecté à l'affichage avec un connecteur JST de 1,25 mm au connecteur étiqueté "SPEAK" (ou soudé).

Consultez l'exemple [HelloRadio](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/Basics/7-HelloRadio) pour voir comment l'utiliser.

La plupart des petits haut-parleurs de 8 Ohms devraient fonctionner. Il peut être judicieux d'ajouter un connecteur JST de 1,25 mm pour simplifier le branchement, débranchement.

### Liens

- [Haut-parleur avec connecteur JST 1.25mm (2pcs) - Aliexpress\*](https://s.click.aliexpress.com/e/_DBOJoh7) - Testé, fonctionne directement.
- [Connecteurs JST 2 broches 1.25mm - Aliexpress\*](https://s.click.aliexpress.com/e/_DlbPkWH) - Pas acheté par moi, mais devrait fonctionner.

\* = Lien affilié - Cela ne vous coûte rien de plus, mais je reçois une petite partie de la vente.