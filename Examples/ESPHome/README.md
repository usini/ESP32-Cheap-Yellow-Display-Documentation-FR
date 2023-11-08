# Exemples ESPHome

[Lien vers les examples](https://github.com/witnessmenow/ESP32-Cheap-Yellow-Display/tree/main/Examples/ESPHome)

Ces exemples montrent le code yaml pour faire fonctionner l'affichage ESP32-2432S028R avec ESPHome.

Pour que le yaml fonctionne, vous devez ajouter les paramètres suivants dans votre fichier secrets.yaml :
 - api_key
 - ota_password
 - wifi_ssid
 - wifi_password
 - ap_password

Pour certains des exemples, vous devrez copier des fichiers de polices ou d'images dans votre dossier ESPHome. Ces exemples contiennent les instructions dans le fichier yaml lui-même.

## 1-HelloWorld

Ce yaml affiche le texte "Hello World" centré sur l'écran.

## 2-ESPHomeClock

Ce yaml affiche le logo ESPHome et la date et l'heure actuelles.

## 3-RGBLED

Ce yaml publie la LED RVB située au dos de l'affichage dans Home Assistant.

## 4-TouchDemo

Ce yaml affiche deux rectangles agissant comme des capteurs tactiles binaires au sein de Home Assistant.

## 5-TemperatureGraph

Ce yaml affiche un graphique d'un capteur de température de Home Assistant.

