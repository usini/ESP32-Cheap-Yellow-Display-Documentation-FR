# Modifications CYD

Voici quelques modifications matérielles qui peuvent être effectuées sur le CYD pour améliorer ou changer certaines de ses fonctionnalités.

## Améliorer la portée et les performances du LDR

La gamme de détection du LDR sur le CYD est assez limitée, de complètement étaint à complètement lumineux. Cette modification augmente cette gamme et lisse également la sortie du LDR.

Elle implique de souder à la main des composants 0603, donc probablement pas pour les débutants en soudure !

[Lien](https://github.com/hexeguitar/ESP32_TFT_PIO#1-ldr)

## Modification du gain de l'ampli audio

La configuration de l'ampli audio sur le CYD n'est pas bonne, résultant en une qualité audio médiocre. Cette modification réduit le gain ce qui conduit à une meilleure qualité audio.

Comme décrit, cela implique de souder à la main un composant 0603, mais vous pourriez également ajouter une résistance de 10k à travers les deux pattes inférieures de l'IC pour la même modification. Faites ce qui vous semble le plus facile !

![image](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/assets/1562562/04b98352-ca41-4bcc-bf77-380db4cce1da)

[Lien](https://github.com/hexeguitar/ESP32_TFT_PIO#2-audio-amp-gain-mod)

## Ajout de PSRAM

Il est possible, avec certaines modifications de la carte, d'utiliser de la PSRAM avec le CYD.
Cette modification implique de retirer la LED RVB, de couper certaines pistes et d'installer le CI PSRAM.

[Lien](https://github.com/hexeguitar/ESP32_TFT_PIO#adding-psram)