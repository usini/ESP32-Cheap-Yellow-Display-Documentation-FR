# Broches

Cette page parle des broches sur le CYD.

## Quelles broches sont disponibles sur le CYD ?

Il y a 3 broches GPIO facilement accessibles.

|Broche|Emplacement|Note|
|---|---|----|
|IO35|Connecteur JST **P3**|Broche d'entrée uniquement, pas de résistances de tirage internes disponibles|
|IO22|Connecteur JST **P3** et **CN1**||
|IO27|Connecteur JST **CN1**||

Si vous avez besoin de plus de broches, vous devrez aller les chercher sur d'autres composants. Le SD Card Sniffer comme mentionné dans les [Add-ons](ADDONS.md) est probablement la méthode la plus facile.

Si vous avez besoin de plus de broches, vous devrez désouder des composants.

## Broches disponibles

Il y a trois connecteurs JST 4P de 1,25 mm sur la carte.

### P3
|Broche|Utilisation|Note|
|---|---|----|
|GND|||
|IO35||Broche d'entrée uniquement, pas de résistances de tirage internes disponibles|
|IO22||Aussi sur le connecteur **CN1**|
|IO21||Utilisé pour le rétroéclairage TFT, donc pas vraiment utilisable|

### CN1
C'est un excellent candidat pour les dispositifs I2C.

|Broche|Utilisation|Note|
|---|---|----|
|GND|||
|IO22||Aussi sur le connecteur **P3**|
|IO27|||
|3.3V|||

### P1
|Broche|Utilisation|Note|
|---|---|----|
|VIN|||
|IO1(?)|TX|Peut-être possible d'utiliser comme GPIO ?|
|IO3(?)|RX|Peut-être possible d'utiliser comme GPIO ?|
|GND|||

## Boutons

Le CYD a deux boutons, reset et boot.

|Broche|Utilisation|Note|
|---|---|----|
|IO0|BOOT|Peut être utilisé comme entrée dans les croquis|

## Haut-parleur

Le connecteur du haut-parleur est un connecteur JST 2P de 1,25 mm qui est connecté à l'amplificateur, donc pas utilisable en tant que GPIO au connecteur du haut-parleur

|Broche|Utilisation|Note|
|---|---|----|
|IO26|Connecté à l'ampli|`i2s_set_dac_mode(I2S_DAC_CHANNEL_LEFT_EN);`|

## LED RGB

Si votre projet nécessite des broches supplémentaires à ce qui est disponible ailleurs, vous pouvez récupérer cette broche.

Note : Les LED sont "actives à bas", signifiant que HIGH == off, LOW == on

|Broche|Utilisation|Note|
|---|---|----|
|IO4|LED Rouge||
|IO16|LED Verte||
|IO17|LED Bleue||

## Carte SD

|Broche|Utilisation|Note|
|---|---|----|
|IO5|SD_CS||
|IO18|SD_SCK||
|IO19|SD_MISO||
|IO23|SD_MOSI||

## Écran Tactile

|Broche|Utilisation|Note|
|---|---|----|
|IO25|XPT2046_CLK||
|IO32|XPT2046_MOSI||
|IO33|XPT2046_CS||
|IO36|XPT2046_IRQ||
|IO39|XPT2046_MISO||

## Capteur de Luminosité (LDR)

|Broche|Utilisation|Note|
|---|---|----|
|IO34|||

## Affichage

|Broche|Utilisation|Note|
|---|---|----|
|IO2|TFT_RS|Aussi connu sous le nom : TFT_DC|
|IO12|TFT_SDO|Aussi connu sous le nom : TFT_MISO|
|IO13|TFT_SDI|Aussi connu sous le nom : TFT_MOSI|
|IO14|TFT_SCK||
|IO15|TFT_CS||
|IO21|TFT_BL|Aussi sur le connecteur P3, pour une raison quelconque|

## Points de test
|Patte|Utilisation|Note|
|---|---|----|
|S1|GND|près de USB-SERIAL|
|S2|3.3v|pour ESP32|
|S3|5v|près de USB-SERIAL|
|S4|GND|pour ESP32|
|S5|3.3v|pour TFT|
|JP0 (patte la plus proche de la prise USB)|5v|LDO TFT|
|JP0|3.3v|LDO TFT|
|JP3 (patte la plus proche de la prise USB)|5v|LDO ESP32|
|JP3|3.3v|LDO ESP32|
