# Consignes pour le déploiement LoRa en environnement urbain de petite taille (TaillePetiteUrbExt)

## Objectif

Ce guide vise à fournir des instructions détaillées pour le déploiement d'un réseau LoRa en maillage dans un environnement urbain de petite taille. L'objectif est d'assurer une communication résiliente sans relais, même en cas de catastrophe naturelle.

## Matériel recommandé

- **Fréquence** : 433 MHz (pour une meilleure pénétration des obstacles en milieu urbain dense).
- **Endpoints** : 4x T-BEAM Supreme (Lyligo).

## Configuration des antennes

- **Hauteur des antennes** : Installer les antennes à une hauteur de 10 mètres (environ 3 étages) pour maximiser la portée et la qualité du signal.
- **Topologie du réseau** : Placer les endpoints de manière à créer un réseau maillé, où chaque nœud peut communiquer avec plusieurs autres nœuds, assurant ainsi une redondance naturelle.


## Protocole et firmware

- **Protocole** : Utiliser le protocole Meshtastic, qui est un protocole de maillage automatique fonctionnant avec la technologie LoRa.
- **Flashage des cartes** : Utiliser le web flasher pour mettre à jour les T-BEAM Supreme avec la version la plus récente de Meshtastic.

## Tests et validation

- **Tests de portée** : Effectuer des tests de portée pour vérifier que les antennes à 10 mètres offrent une couverture suffisante dans les zones urbaines denses sans nécessiter de relais.
- **Tests de pénétration** : Vérifier que le signal à 433 MHz traverse efficacement les obstacles urbains.
- **Tests de redondance** : Simuler des pannes de certains nœuds pour s'assurer que le réseau maillé reste fonctionnel grâce à la redondance.


## Conclusion

En suivant ces consignes, vous pourrez déployer un réseau LoRa résilient et maillé dans un environnement urbain de petite taille, capable de maintenir la communication même en cas de catastrophe naturelle, sans nécessiter de relais.

---

Ce fichier de consignes est basé sur les résultats des tests et les recommandations fournies dans le rapport de projet. Pour plus de détails, consultez l'arbre de décision et les fichiers de tests associés.
