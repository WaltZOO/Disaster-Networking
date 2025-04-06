# Flashage Meshtastic sur Heltec V1 et Wio WM1110A

### Méthode :
Utilisation de Gitpod pour compiler des versions antérieures compatibles.

### Commandes de compilation :

**Heltec V1 et Wio WM1110A** :
Flasher à partir des binaries récupérer sur Gitpod
```bash
pio run -e heltec-v1
pio run -e wio-tracker
python3 -m esptool --port /dev/ttyUSB1 --chip esp32 write_flash 0x0 firmware.factory.bin
```

# Problématiques rencontrées avec les cartes STM32

## Cartes concernées

- Wyres V2  
- Seeed LoRa-E5 

Nous disposons également d'autres cartes telles que les **Wyres V2** et les **LoRa-E5**, que nous souhaiterions flasher. Ces cartes sont basées sur des **STM32** et ne sont pas directement compatibles avec **Meshtastic**.
Meshtastic est conçu pour **FreeRTOS** et nos cartes utilisent **RIOT-OS**.

Pour les rendre compatibles, il serait nécessaire de :

- Prendre un firmware Meshtastic existant  
- L'adapter pour qu'il fonctionne sur des cartes STM32 tournant sous **RIOT-OS**  
- Développer une **API de compatibilité** entre les modules **RadioLib** utilisés par Meshtastic et l’environnement RIOT-OS  
- Les flasher en utilisant une carte **Nucleo F334R8** via ST-Link sur un IDE comme **ArduinoIDE** ou encore **STM32CubeProgrammer**.

Cette tâche, que nous pensions initialement faisable rapidement, s’est révélée beaucoup plus complexe que prévu. N’ayant pas anticipé cette difficulté, nous avons fait le choix de nous concentrer sur les tests radio, que nous jugions prioritaires à ce stade du projet.

Au final, la compatibilité Meshtastic/STM32/RIOT-OS n’a pas pu être finalisée dans le temps imparti.
