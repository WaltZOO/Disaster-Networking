# Cahier des Charges : Disaster Networking

**Février 2025**  
Bossant Maxime, Ivanova Antonia, Maury Maxence et Poncin Erwan  

---

## Table des matières  
1. [Présentation du projet](#présentation-du-projet)  
2. [Cible du projet](#cible-du-projet)  
3. [Notre enveloppe budgétaire](#notre-enveloppe-budgétaire)  
4. [Délais de réalisation](#délais-de-réalisation)  
5. [Spécifications fonctionnelles](#spécifications-fonctionnelles)  
   - [Communication avec ClusterDuck](#communication-à-distance-avec-clusterduck)  
   - [Communication avec Meshtastic](#communication-à-distance-avec-meshtastic)  
6. [Spécifications techniques](#spécifications-techniques)  
   - [Infrastructure et matériel](#infrastructure-et-matériel)  
   - [Mise en réseau et protocoles](#mise-en-réseau-et-protocoles)  
   - [Performances et portée](#performances-et-portée)  
   - [Consommation et autonomie](#consommation-et-autonomie)  
   - [Robustesse](#robustesse)  
   - [Déploiement et maintenance](#déploiement-et-maintenance)  

---

## Présentation du projet  

L’intitulé de notre projet est **Disaster Networking**.  

Nous devons utiliser la technologie **LoRa** pour mettre en place un réseau de communication d’urgence permettant l’échange de messages lors d’une catastrophe naturelle, lorsque les antennes 4G sont hors service.  

Notre cas d’étude de base est le cyclone **Chido** sur Mayotte qui, survenu en décembre 2024, a rendu hors service **51 des 54 antennes** du réseau mobile (entre autres faute de courant). Notre objectif est de mettre en place un réseau assurant la communication entre les **secouristes** et les **habitants** pour coordonner les secours et alerter les populations.  

---

## Cible du projet  

Nous avons pour objectif de mettre en place et comparer deux technologies : le protocole **ClusterDuck** et le protocole **Meshtastic**.  

Les livrables du projet sont :  
- **Arbre de décision pour la communication** : critère de choix entre ClusterDuck et Meshtastic.  
- **Guide de déploiement rapide** : étapes d'installation et de configuration, résultats des tests terrains.  

---

## Notre enveloppe budgétaire  

Nous disposons de **54 heures** de travail à 4.  
Sachant qu’une journée de travail a une durée de 8 heures, nous disposons d’une enveloppe de **27 jours-homme** pour le projet.  

---

## Délais de réalisation  

- **Soutenance finale** : 7 avril 2025.  
- **Soutenance de mi-parcours** : lundi 10 mars 2025 à 14h30.  

---

## Spécifications fonctionnelles  

### Communication à distance avec ClusterDuck  
**Objectif** : Assurer une communication entre deux antennes à plusieurs kilomètres de distance :  
- Milieu urbain : ≥ 10 km  
- Milieu dégagé : ≥ 30 km  

### Communication à distance avec Meshtastic  
**Objectif** : Assurer une communication entre deux antennes à plusieurs kilomètres de distance :  
- Milieu urbain : ≥ 10 km  
- Milieu dégagé : ≥ 30 km  

---

## Spécifications techniques  

### Infrastructure et matériel  
- **Technologie utilisée** : LoRa (Long Range)  
- **Fréquences supportées** : 868 MHz et 433 MHz  
- **Matériel disponible** :  
  - TBeam Supreme 433 x4  
  - TBeam Supreme 868 x2  
  - 4x TinyGS 2G4 + ESP32 Dev Kit + 1x LoRa 2.4 GHz + 1x Wyres  
  - Wyres x5  
  - LoRa E5 Mini x5  
  - Minitel (reste dans le Fablab)  
  - MXCHIP (car écran OLED)  

### Mise en réseau et protocoles  

**ClusterDuck Protocol** :  
- Mise en place d’un réseau maillé avec des nœuds relais.  
- Utilisation du protocole LoRa ou d’une couche réseau propriétaire.  
- Auto-configuration et adaptation du maillage.  

**Meshtastic** :  
- Réseau maillé décentralisé avec routage dynamique.  
- Utilisation du protocole LoRa point-à-point avec échange de messages.  
- Compatibilité avec les smartphones via Bluetooth/Wi-Fi.  

### Performances et portée  
- **Portée cible** :  
  - Milieu urbain : ≥ 10 km  
  - Milieu dégagé : ≥ 30 km  
- **Débit de données** : Messages courts (inférieurs à 256 octets).  
- **Latence maximale** :  
  - ≤ 10 secondes en conditions normales  
  - ≤ 60 secondes en forte charge  

### Consommation et autonomie  
- Autonomie ≥ 48 heures en conditions normales.  
- Système de veille et d’activation à la demande.  
- Option d’alimentation solaire pour prolonger l’autonomie.  

### Robustesse  
- Résistance à l’humidité et aux températures extrêmes.  
- Antennes et boîtiers renforcés pour l’usage en extérieur.  

### Déploiement et maintenance  
- **Facilité d’installation** :  
  - Guide de déploiement rapide.  
  - Interface utilisateur simplifiée.  
- **Surveillance du réseau** :  
  - Outil de monitoring des relais.  
  - Logs d’activité pour l’analyse des performances.  

---
