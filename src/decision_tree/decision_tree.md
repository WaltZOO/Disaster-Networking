```mermaid
graph TD
    Milieu["Type de Milieu"] 

    Urbain{"Milieu Urbain"}
    Rural{"Milieu Rural"}
    Montagneux{"Milieu Montagneux"}
    
    Milieu --> Urbain
    Milieu --> Rural
    Milieu --> Montagneux

    ExtPossible["Extérieur possible ?"]
    HauteurPossibleRural["Hauteur disponible ?"]
    HauteurPossibleMont["Hauteur disponible ?"]

    Urbain --> ExtPossible
    Rural --> HauteurPossibleRural
    Montagneux --> HauteurPossibleMont

    ExtOui{"OUI"}
    ExtNon{"NON"}
    HautRuralOui{"OUI"}
    HautRuralNon{"NON"}
    HautMontOui{"OUI"}
    HautMontNon{"NON"}

    ExtPossible --> ExtOui
    ExtPossible --> ExtNon
    HauteurPossibleRural --> HautRuralOui
    HauteurPossibleRural --> HautRuralNon
    HauteurPossibleMont --> HautMontOui
    HauteurPossibleMont --> HautMontNon

    SuperficieUrbExt["Superficie à couvrir"]
    SuperficieUrbInt["Superficie à couvrir"]
    SuperficieRuralExt["Superficie à couvrir"]
    SuperficieRuralInt["Superficie à couvrir"]
    SuperficieMontExt["Superficie à couvrir"]

    ExtOui --> SuperficieUrbExt
    ExtNon --> SuperficieUrbInt
    HautRuralOui --> SuperficieRuralExt
    HautRuralNon --> SuperficieRuralInt
    HautMontOui --> SuperficieMontExt

    TaillePetiteUrbExt{"<'7000m²"}
    TailleGrandeUrbExt{">=7000m²"}
    TaillePetiteUrbInt{"<'2000m²"}
    TailleGrandeUrbInt{">=2000m²"}
    TaillePetiteRuralExt{"<'4.9km²"}
    TailleGrandeRuralExt{">=4.9km²"}
    TaillePetiteRuralInt{"<'3.1km²"}
    TailleGrandeRuralInt{">=3.1km²"}
    TaillePetiteMontExt{"<'3.1km²"}
    TailleGrandeMontExt{">=3.1km²"}

    SuperficieUrbExt --> TaillePetiteUrbExt
    SuperficieUrbExt --> TailleGrandeUrbExt
    SuperficieUrbInt --> TaillePetiteUrbInt
    SuperficieUrbInt --> TailleGrandeUrbInt
    SuperficieRuralExt --> TaillePetiteRuralExt
    SuperficieRuralExt --> TailleGrandeRuralExt
    SuperficieRuralInt --> TaillePetiteRuralInt
    SuperficieRuralInt --> TailleGrandeRuralInt
    SuperficieMontExt --> TaillePetiteMontExt
    SuperficieMontExt --> TailleGrandeMontExt

    TaillePetiteUrbExt --> Consignes1["consignes_1.md"]
    TailleGrandeUrbExt --> Consignes2["consignes_2.md"]
    TaillePetiteUrbInt --> Consignes3["consignes_3.md"]
    TailleGrandeUrbInt --> Consignes4["consignes_4.md"]
    TaillePetiteRuralExt --> Consignes5["consignes_5.md"]
    TailleGrandeRuralExt --> Consignes6["consignes_6.md"]
    TaillePetiteRuralInt --> Consignes7["consignes_7.md"]
    TailleGrandeRuralInt --> Consignes8["consignes_8.md"]
    TaillePetiteMontExt --> Consignes9["consignes_9.md"]
    TailleGrandeMontExt --> Consignes10["consignes_10.md"]
    HautMontNon --> Consignes11["consignes_11.md"]




```