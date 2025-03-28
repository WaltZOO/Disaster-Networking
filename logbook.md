# Projet 18 Disaster Network : Journal de bord (aka fiche de suivi)

## 2025-03-28
* [x] finir arbre de decision
* [x] deseign des test
* [x] Documentation LoRa dev e5 
    - carte stm32 non compatible avec Meshtastic (pas assez de mémoire)

## 2025-03-25
* [x] Carte Wio Tracker WM1110 flashé en tant que relai Meshtastic

## 2025-03-24
* [x] Carte Heltec Lora 32 flashé en tant que relai Meshtastic
* [x] Test de portée des T-beam supreme 686 MHz 

## 2025-03-17
A faire: 
* [ ] FLasher les Wyres

## 2025-03-11
A faire : 

* [ ] Trouver la documentation des castes à disposition (WIO Wyres, ST Link, T-Beam Supreme, ...)
 - On a trouver pour la WIO Wyres (mais pas comlète) et la STLink 
* [x] Faires le cablage pour connecter la Wyres à la STLink 
* [ ] Trouver le bon IDE pour flasher nos Wyres
* [ ] Trouver le programme à mettre sur les Wyres
* [x] Trouver le programme à mettre sur les T-Beam Supreme
* [ ] Flasher les Wyres
* [x] Flasher les T-Bean Supreme



## 2025-03-10 Soutenance mi-parcours

A faire

* [ ] aller emprunter le [Wisblock RAK11310](https://store.rakwireless.com/products/rak11310-wisblock-lpwan-module) [build file](https://github.com/meshtastic/firmware/blob/master/boards/wiscore_rak11300.json) au fablab.
* [ ] voir https://github.com/EWSS-CAMF/camf/blob/main/README.md
* [ ] voir https://github.com/thingsat/riot_modules/tree/main/modules/camf

## 2025-02-25

A faire

* [x] aller emprunter le [WM1110](https://meshtastic.org/docs/hardware/devices/seeed-studio/wm1110/) au fablab.

## 2025-02-24

Finition du cahier des charges.

## 2025-02-20

* [ ] DD --> Team : à lire : [How SenseCAP T1000-E Becomes a Game-Changing Dog Tracker](https://www.etsy.com/fr/listing/1867271135/houdini-m1-traceur-de-chien-open-source?etsrc=sdt)
 
In the video, Data Slayer showcases the Houdini M1 Dog tracker, a DIY solution designed with SenseCAP T1000-E. It's open-source and free from subscriptions. In a personal story, he shares how losing a dog in the wild led him to create this tracker. Unlike AirTag or GPS collars, the Houdini M1 uses Meshtastic technology for real-time, decentralized tracking—perfect for off-grid adventures. Get your T1000-E on [Seeed's official store](https://www.seeedstudio.com/SenseCAP-Card-Tracker-T1000-E-for-Meshtastic-p-5913.html) or Amazon here(10% off coupon code RWL5D6ZS).


## 2025-02-18

Commencement du cahier des charges.

## 2025-02-10

Reunion Gestion de Projet pour mieux definir le livrable. 

* [ ] rédiger le [who is who](./whoiswho.md) (et les rôles)
* [ ] rédiger un pacte d'équipe (~pacte d'associé)
* [x] rédiger le cahier des charges (markdown bien sur) avec les diagrammes
* [x] faire le [point matériel récupéré](./matos.md) au fablab (emprunt depuis https://matos.univ-grenoble-alpes.fr/#
* [ ] créer une structure arborescente de dossiers pour organiser le dépôt

Exemple de structure arborescente
* [./README.md](./README.md) --> un description et des liens pour naviguer dans la structure
* [./logbook.md](./logbook.md)
* [./whoiswho.md](./whoiswho.md)
* [./CONTRIBUTORS.md](./CONTRIBUTORS.md)
* [./pacte.md](./pacte.md)
* [./matos.md](./matos.md)
* [./LICENSE.md](./LICENSE.md)
* ./presentations
* ./presentations/README.md
* ./presentations/2024-02-10/
* ./presentations/2024-02-17/
* ./presentations/2024-03-XX_mid-project/
* ./presentations/2024-04-XX_final/
* ./reports
* ./reports/bib.tex
* ./reports/bib.md
* ./docs
* ./docs/user
* ./docs/admin
* ./media
* ./externals
* ./sandbox

**Instructions et bonnes pratiques**

* utilisez Markdown :  Rien d'autres n'est accepté
* utilisez [PlantUML](https://github.com/donsez/bd/tree/main/plantuml#readme) pour les diagrammes :  Rien d'autres n'est accepté (ie éditeurs en ligne and co)
* préférez SVG pour les schémas vectoriels à PNG et JPEG (pire HEIC)
* PDF, DOCX, PPT, ODT, ODP proscrits (sinon `git rm *.pdf, *.pptx *.docx ...`)
* utilisez Markdown et [reveal.js](https://github.com/webpro/reveal-md) pour vos présentations (dans un dossier dans le dossier `./presentations`)
* pour les thèmes dans les slides, pensez aux daltoniens (le [NB](https://fr.wikipedia.org/wiki/Bienvenue_%C3%A0_Gattaca) est indémodable)
* tout ce qui n'est pas écrit n'a pas été fait
* tout ce qui temporaire est définitif (on nettoiera plus tard, vite fait ...)
* plus tard == jamais
* redigez plutôt en anglais --> vos projets seront visibles de vos employeurs, vos maîtres de stage ...
* docker, docker, docker
* git, git, git
* dans vos interactions orales (présentations, clients) : évitez wesh wesh, vite fait, rapide, carré ... vous n'êtes pas sur la scène RAP française !
* [intelligence contextuelle](https://www.wikiberal.org/wiki/Intelligence_contextuelle)
* [Pandoc](https://pandoc.org/) est votre ami

## 2025-02-03

Prise de connaissance du sujet. Documentation sur Meshtastic et Clusterduck

## 2025-02-11



