Dagoma Sigma avec Klipper

ATTENTION:
Ces modifications nécessitent l'ouverture de la machine avec le risque de détériorer les capteur FSR.
Si vous envisager ces modifications vous perdez la garantie sur votre machine


Le projet à pour objectif de convertir une imprimante Dagoma Sigma utilisant comme firmware Marlin, en une imprimante utilisant comme firmeware Klipper.
afin de gagner en précision et diminuer les bruits de déplacement des chariots
Particularité de cette imprimante utilisation de 3 capteurs de force (FSR) positionnés sous le plateau afin de réaliser le bed leveling, ou Bed-mesk chez Klipper
avec utilisation d'une entrée analogique code adapté de Marlin.

4 étapes envisagé :

1- Electronique et mécanique d'origine, avec utilisation de cale de rappel afin de faire fonctionner les FSR dans la plage de commutation de l'entrée numérique.

2- Electronique et mécanique d'origine, avec ajout d'une carte pour la gestion des FSR qui produit en sortir un signal numérique tout ou rien.
Carte addtionelle utilisé : https://github.com/JohnSL/FSR_Endstop

le 1 et 2 sont des preuve de concepte, pas ou peux de gain attendu coté bruit

3- Mécanique d'origine, pour l'électronique utilisation de la dernière carte D6 avec driver TMC 2209 de chez Dagoma afin de rester dans l'echo système.
gain attendu sur le bruit en augmentant le nombre de micro-step, augmentation limité par la chip 8 bit ATMEGA2560 utiliser sur la carte

4- Mécanique d'origine, pour l'électronique utilisation de la dernière carte Fystec R4 avec la carte additionnelle pour les FSR
Gain attendu plus important sur le bruit, carte optimisé pour embarquer Klipper, form factor plus compact

Eng :
Dagoma Sigma with Klipper

WARNING:
These modifications require opening the machine with the risk of damaging the FSR sensors.
If you consider these modifications you will lose the warranty on your machine.


The project aims to convert a Dagoma Sigma printer using Marlin as firmware, into a printer using Klipper as firmware.
in order to gain precision and reduce carriage movement noise
Particularity of this printer use of 3 force sensors (FSR) positioned under the plate in order to carry out bed leveling, or Bed-mesk at Klipper
with use of an analog input code adapted from Marlin.

4 steps envisaged:

1- Original electronics and mechanics, with use of return wedge in order to operate the FSRs in the switching range of the digital input.

2- Original electronics and mechanics, with the addition of a card for managing the FSR which produces an all or nothing digital signal.
Additional card used: https://github.com/JohnSL/FSR_Endstop

1 and 2 are proof of concept, no or little gain expected in terms of noise

3- Original mechanics, for electronics use of the latest D6 card with TMC 2209 driver from Dagoma in order to remain in the echo system.
expected gain on noise by increasing the number of micro-steps, increase limited by the 8 bit ATMEGA2560 chip used on the card

4- Original mechanics, for electronics use of the latest Fystec R4 card with the additional card for FSR
Greater expected gain on noise, card optimized to embed Klipper, more compact form factor
