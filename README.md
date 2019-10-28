# Registre des Navires Professionnels Français

Les données proviennent de la Direction des Affaires Maritimes, au sein du Ministère de la Transition Ecologique et Solidaire.

## Modèle de données

|Nom|Titre|Type|Description|Exemple|Propriétés|
|-|-|-|-|-|-|
|num_immat_francais|Numéro Immatriculation Française|text|6 chiffres d'immatriculation professionnelle française 1 lettre et cinq chiffres pour les navires immatriculés en plaisance. Si le navire de plaisance vient à passer en professionnel, il prend un 
|nom_navire|Nom du Navire|text|Nom utilisé pour identifier un navire. Ce champ n'est pas unique et peut changer (notamment lors d'un changemement de propriétaire|Houba Houba|Valeur obligatoire|
|chantier_construction|Chantier construction|text| - |CHANTIER NAVAL TARIN|Valeur optionnelle|
|genre_navigation|Genre Navigation|text||CI-CABOTAGE INTERNATIONAL|Valeur obligatoire|
|centre_secu_gestion|Centre sécurité gestionnaire|text|Un centre de sécurité est un service régional de la prévention des risques professionnels maritimes. Il a pour tâche principale la visite de navires professionnels français qui doivent être titulaires d’un permis de navigation (titre de sécurité).|CSN Caen|Valeur obligatoire|
|puissance_propulsive|Puissance Propulsive|double precision|Puissance propulsive en kW| - | Valeur optionnelle|
|longueur_hors_tout|Longueur Hors Tout|double precision|Distance entre les points extrêmes avant et arrière de la structure permanente du bateau|11.9|Valeur obligatoire|
|annee_construction|Année de Construction|double precision| -  |1989|Valeur obligatoire|
