# Consignes pour le déploiement LoRa en environnement montagneux de petite taille avec extensions (TaillePetiteMontExt)

## Objectif

Ce guide vise à fournir des instructions détaillées pour le déploiement d'un réseau LoRa en maillage dans un environnement montagneux de petite taille avec extensions possibles. L'objectif est d'assurer une communication résiliente, même en cas de catastrophe naturelle.

## Matériel recommandé

- **Fréquence** : 868 MHz (pour une meilleure portée en environnement dégagé).
- **Endpoints** : 4x T-BEAM Supreme (Lyligo).

## Configuration des antennes

- **Hauteur des antennes** : Installer les antennes en haut de la montagne pour optimiser la couverture dans un environnement montagneux.
- **Positionnement** : Placer les endpoints de manière à créer un réseau maillé, où chaque nœud peut communiquer avec plusieurs autres nœuds, assurant ainsi une redondance naturelle.

## Topologie du réseau

- **Topologie maillée** : Utiliser une topologie en maillage où chaque endpoint peut communiquer directement avec plusieurs autres endpoints.

## Protocole et firmware

- **Protocole** : Utiliser le protocole Meshtastic, qui est un protocole de maillage automatique fonctionnant avec la technologie LoRa.
- **Flashage des cartes** : Utiliser le web flasher pour mettre à jour les T-BEAM Supreme avec la version la plus récente de Meshtastic.

## Tests et validation

- **Tests de portée** : Effectuer des tests de portée pour vérifier que les antennes à 5 mètres offrent une couverture suffisante dans les zones montagneuses.
- **Tests de pénétration** : Vérifier que le signal à 868 MHz offre une portée optimale dans un environnement ouvert.
- **Tests de redondance** : Simuler des pannes de certains nœuds pour s'assurer que le réseau maillé reste fonctionnel grâce à la redondance.

## Conclusion

En suivant ces consignes, vous pourrez déployer un réseau LoRa résilient et maillé dans un environnement montagneux de petite taille, capable de maintenir la communication même en cas de catastrophe naturelle.

---
