# Registre des Navires Professionnels Français

Les données proviennent de la Direction des Affaires Maritimes, au sein du Ministère de la Transition Ecologique et Solidaire.

## Modèle de données
- Clé primaire : 'num_immat_francais'

|Nom|Titre|Type|Description|Exemple|Propriétés|
|-|-|-|-|-|-|
|num_imo|Identifiant OMI|double precision|Identifiant des navires, associé à une coque. Il est invariant quels que soient les changements de propriétaire, de pavillon ou de nom du navire. Il est attribué aux navires de commerce de jauge brute égale ou supérieure à 100 à leur construction. [ref wikipédia](https://fr.wikipedia.org/wiki/Num%C3%A9ro_IMO) |IMO 1234567|Valeur optionnelle|
|num_mmsi|identifiant MMSI|double precision|Maritime Mobile Service Identity (MMSI) : Indentifiant radiophonique unique d'un navire| 227150000|Valeur optionnelle|
|num_immat_francais|Numéro Immatriculation Française|text|6 chiffres d'immatriculation professionnelle française 1 lettre et cinq chiffres pour les navires immatriculés en plaisance. Si le navire de plaisance vient à passer en professionnel, il prend un numéro définitif à 6 chiffres.|762413 (Navigation Professionnelle) A62413 (Plaisance)|Valeur obligatoire|
|armateur_exploitant| Armateur exploitant|text|Armateur responsable de l'exploitation du navire|Bourbon|Valeur opérationnelle| 
|nom_navire|Nom du Navire|text|Nom utilisé pour identifier un navire. Ce champ n'est pas unique et peut changer (notamment lors d'un changemement de propriétaire|Houba Houba|Valeur obligatoire|
|chantier_construction|Chantier construction|text| - |CHANTIER NAVAL TARIN|Valeur optionnelle|
|genre_navigation|Genre Navigation|text|Donnée réglementant le temps de de navigation|CI-CABOTAGE INTERNATIONAL|Valeur obligatoire|
|effectif_minimum|Effectif Minimum|int| Nombre minimum de personnel navigants à bord| 3 | Valeur obligatoire |
|centre_secu_gestion|Centre sécurité gestionnaire|text|Un centre de sécurité est un service régional de la prévention des risques professionnels maritimes. Il a pour tâche principale la visite de navires professionnels français qui doivent être titulaires d’un permis de navigation (titre de sécurité).|CSN Caen|Valeur obligatoire|
|puissance_propulsive|Puissance Propulsive|double precision|Puissance propulsive en kW| - | Valeur optionnelle|
|longueur_hors_tout|Longueur Hors Tout|double precision|Distance entre les points extrêmes avant et arrière de la structure permanente du bateau|11.9|Valeur obligatoire|
|annee_construction|Année de Construction|int| -  |1989|Valeur obligatoire|
|type_carburant| Type de carburant|text| Carburant utilisé pour la propulsion du navire |Diesel| Valeur optionnelle|
|jauge| Jauge | double precision | Mesure de la capacité de transport d'un navire. Unité en UMS | 260 | Valeur obligatoire | 
|nombre_moteur| Nombre de moteurs | int |-|2| Valeur optionnelle | 
|quartier| Quartier |text| Si RI => Registre International Français| Brest| Valeur optionnelle|
|date_francisation| Date Francisation |date| Date à laquelle le navire porte la pvaillons français | 12/12/2012 | Valeur optionelle|
|date_derniere_emission_ais| Date Dernière Emission AIS| date | Date de la dernière émission de position via AIS, dont la vitesse est non nulle | 12/12/2012 | Valeur optionelle |
|moyenne_vitesse_ais|Moyenne Vitesse AIS| int| Moyenne de la vitesse du navire relevé via AIS | 12 knts | Vitesse optionnelle|





