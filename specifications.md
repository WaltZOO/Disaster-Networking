# Cahier des Charges : Disaster Networking

**Février – Avril 2025**  
Bossant Maxime, Ivanova Antonia, Maury Maxence, Poncin Erwan  

---

## Table des matières  
1. [Présentation du projet](#présentation-du-projet)  
2. [Cible du projet](#cible-du-projet)  
3. [Notre enveloppe budgétaire](#notre-enveloppe-budgétaire)  
4. [Délais de réalisation](#délais-de-réalisation)  
5. [Spécifications fonctionnelles](#spécifications-fonctionnelles)  
6. [Spécifications techniques](#spécifications-techniques)  

---

## Présentation du projet  

L’intitulé de notre projet est **Disaster Networking**.  
Nous avons étudié l’utilisation de la technologie **LoRa** pour mettre en place un réseau de communication résilient pouvant fonctionner en cas de catastrophe naturelle, lorsque les infrastructures classiques sont hors service.  

Le cas d’étude choisi est le cyclone **Chido**, survenu à Mayotte en décembre 2024, qui a mis hors service **51 des 54 antennes** du réseau mobile. L’objectif est de **préparer** un réseau résistant à ce type d’événement, pour permettre aux **secouristes** et **habitants** de continuer à échanger des informations vitales.  

---

## Cible du projet  

Le projet repose sur une approche préventive : **anticiper la catastrophe** en déployant un réseau adapté à la topographie et à la densité de l’environnement.  

Nous avons testé deux bandes de fréquence LoRa (433 MHz et 868 MHz) en environnement urbain, périurbain et rural.  
Nous avons utilisé le protocole **Meshtastic**, un protocole de routage automatique en réseau maillé, embarqué sur différentes cartes.  

Les livrables du projet sont :  
- **Arbre de décision** pour aider à choisir la fréquence et la topologie réseau selon le terrain.  
- **Résultats des tests de portée LoRa** selon plusieurs facteurs (hauteur, densité urbaine, température, distance).  
- **Guide de déploiement** des équipements Meshtastic.  

---

## Notre enveloppe budgétaire  

Nous disposions d’une enveloppe de **54 heures de travail par personne** dans un groupe de 4, soit **216 heures** ou **27 jours-homme**.  

---

## Délais de réalisation  

- **Début du projet** : février 2025  
- **Soutenance intermédiaire** : 10 mars 2025  
- **Soutenance finale** : 7 avril 2025  

---

## Spécifications fonctionnelles  

### Objectifs fonctionnels réalisés  
- Tester et comparer les performances de **LoRa 433 MHz** et **LoRa 868 MHz**.  
- Évaluer l’influence de la **hauteur des antennes**, de la **densité urbaine**, de la **température**, et de la **distance**.  
- Déterminer les **configurations optimales** selon l’environnement.  
- Proposer un **guide de déploiement** orienté terrain, avec recommandations pratiques.  

### Livrable clé  
- Un **arbre de décision** (Appendix 1) indiquant le matériel, la fréquence, la topologie et la hauteur à utiliser selon la configuration du terrain.  

---

## Spécifications techniques  

### Infrastructure et matériel  

- **Technologie utilisée** : LoRa (Long Range), Meshtastic (firmware open-source)  
- **Fréquences testées** : 433 MHz, 868 MHz  

#### Matériel utilisé :
- **433 MHz** :  
  - 4x T-BEAM Supreme (LilyGO)  

- **868 MHz** :  
  - 2x T-BEAM Supreme (LilyGO)  
  - 1x WiFi LoRa 32 (Heltec)  
  - 1x Wio-WM1110 (Seeed Studio)  

### Mise en réseau et protocole  
- **Meshtastic** :  
  - Réseau maillé automatisé avec routage dynamique.  
  - Communication point-à-point via LoRa.  
  - Compatibilité Bluetooth/Wi-Fi pour l’interface smartphone.  

- Le **portage de Meshtastic sur d’autres cartes** a été partiellement tenté (via flashing manuel) mais abandonné au profit des tests terrain, jugés prioritaires.  

### Performances et portée (résultats réels)  
- **Portée observée** :  
  - **433 MHz** :  
    - Urbain dense : jusqu’à 500 m  
    - Rural dégagé : jusqu’à 1,5 km  
  - **868 MHz** :  
    - Urbain : jusqu’à 1,5 km  
    - Rural dégagé : jusqu’à 5 km  

- **Hauteur optimale** :  
  - Urbain : antenne à ~10 m (équivalent 3e étage)  
  - Rural : ~5 m suffisent  

### Consommation et autonomie  
- **Estimation théorique** : >48 h d’autonomie en mode basse consommation  
- **Pas de mesures exactes** réalisées sur l'autonomie  

### Robustesse  
- Tests limités aux environnements extérieurs en conditions normales  
- Sensibilité à l’alimentation externe et au boîtier non étudiée  


### Déploiement et maintenance  
- **Documentation du flashage Meshtastic** pour les T-BEAM et autres cartes (voir Appendix 3)  
- **Guide de déploiement simplifié** selon terrain  
- Pas de système de supervision ou de monitoring intégré au projet  
