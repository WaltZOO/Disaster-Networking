# Projet 18 - Réseau de catastrophe (disaster network) avec LoRa

Après le passage du cyclone Chido sur Mayotte, les 51 antennes sur 54 du réseau mobile ont été rendues hors service, notamment faute de courant, privant ainsi les autorités et la population de communiquer pour organiser les secours.

Les Disaster Networks (ou réseaux de communication en cas de catastrophe) sont des infrastructures ou systèmes de communication conçus pour assurer la connectivité et les communications critiques lors de situations d’urgence ou de catastrophes naturelles, technologiques ou humaines. Ces réseaux jouent un rôle vital dans la coordination des secours, l’alerte des populations et le rétablissement des communications dans des environnements fortement perturbés.

Dans ce projet, vous mettrez en oeuvre et vous comparerez 2 technologies de réseaux maillés avec des endpoints LoRa :

* le protocole [ClusterDuck](https://clusterduckprotocol.org/)
* le protocole [Meshtastic](https://meshtastic.org/)

Vous essayerez d'implémenter le protocole [Bundle](https://datatracker.ietf.org/doc/rfc9171/) (pour les DTN) au dessus de LoRa si vous avez le temps.

Vos développements pourront être contribués à ces deux communautés oepn-source.

## Tests terrain

Des tests seront réalisés au moyen de ballons captifs gonflés à l'hélium sur le campus de SMH au printemps 2025.

Des tests pourront être également réalisés à bord de ballons stratosphériques du CNES au Printemps 2025 : https://gricad-gitlab.univ-grenoble-alpes.fr/thingsat/public/-/blob/master/balloons/README.md 


![Infra 4G de Mayotte](https://air.imag.fr/images/4/42/Cartoradio-mayotte-01.jpg)
