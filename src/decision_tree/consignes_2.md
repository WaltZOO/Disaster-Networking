# Consignes pour le déploiement LoRa en environnement urbain de taille moyenne avec extensions (TailleMoyenneUrbExt)

## Objectif

Ce guide vise à fournir des instructions détaillées pour le déploiement d'un réseau LoRa en maillage dans un environnement urbain de taille moyenne avec extensions possibles. L'objectif est d'assurer une communication résiliente, même en cas de catastrophe naturelle.

## Matériel recommandé

- **Fréquence** : 433 MHz (pour une meilleure pénétration des obstacles en milieu urbain dense).
- **Endpoints** : 4x T-BEAM Supreme (Lyligo).
- **Relais** : 1x WiFi LoRa 32 (Heltec) ou 1x Wio-WM1110 (si la superficie est supérieure à 7000m²).

## Configuration des antennes

- **Hauteur des antennes** : Installer les antennes à une hauteur de 10 mètres (environ 3 étages) pour maximiser la portée et la qualité du signal.
- **Positionnement** : Placer les endpoints de manière à créer un réseau maillé, où chaque nœud peut communiquer avec plusieurs autres nœuds, assurant ainsi une redondance naturelle.

## Topologie du réseau

- **Topologie maillée** : Utiliser une topologie en maillage où chaque endpoint peut communiquer directement avec plusieurs autres endpoints. Utiliser des relais pour étendre la couverture si la superficie est supérieure à 7000m².

## Protocole et firmware

- **Protocole** : Utiliser le protocole Meshtastic, qui est un protocole de maillage automatique fonctionnant avec la technologie LoRa.
- **Flashage des cartes** : Utiliser le web flasher pour mettre à jour les T-BEAM Supreme avec la version la plus récente de Meshtastic. Pour les autres cartes, suivre la documentation fournie pour flasher le firmware Meshtastic.

## Tests et validation

- **Tests de portée** : Effectuer des tests de portée pour vérifier que les antennes à 10 mètres offrent une couverture suffisante dans les zones urbaines denses.
- **Tests de pénétration** : Vérifier que le signal à 433 MHz traverse efficacement les obstacles urbains.
- **Tests de redondance** : Simuler des pannes de certains nœuds pour s'assurer que le réseau maillé reste fonctionnel grâce à la redondance.

## Conclusion

En suivant ces consignes, vous pourrez déployer un réseau LoRa résilient et maillé dans un environnement urbain de taille moyenne, capable de maintenir la communication même en cas de catastrophe naturelle.

---
