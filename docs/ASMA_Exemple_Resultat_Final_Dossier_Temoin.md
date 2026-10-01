# 1. Ce que montre ce dossier

Ce dossier est un **exemple fictif** produit pour montrer à quoi ressemblera le résultat du programme de standardisation, une fois la phase 1 terminée. Il porte sur une opération inventée, le lotissement Tafoukt, et ne reprend aucun marché, aucun prix adjugé et aucune donnée réelle d'ASMA.

Il suit la chaîne complète du standard, de la saisie des paramètres jusqu'à l'estimation confidentielle :

| Étape | Qui la fait | Ce qu'il produit | Section |
| 1. Renseigner les paramètres | Le bureau d'études | Une fiche de 14 valeurs, sans rédiger une ligne de texte | 2 |
| 2. Générer le CPS type | Le standard | Les prescriptions techniques des lots retenus, déjà référencées | 3 |
| 3. Générer le bordereau | Le standard | Les prix codés des lots retenus, avec leur libellé et leur unité | 4 |
| 4. Chiffrer l'estimation | Le maître d'ouvrage | L'estimation confidentielle et sa fourchette, à partir de la base de prix | 5 |

> Les montants de la section 5 sont **inventés pour la démonstration**. Ils ne proviennent pas de la base de prix d'ASMA et n'ont aucune valeur de référence.

**L'opération fictive.** Lotissement Tafoukt, 4,2 hectares, 180 lots d'habitat économique. Trois lots du corps d'état VRD sont retenus pour l'exemple : VRD03 assainissement eaux usées, VRD11 bordures et caniveaux, VRD12 revêtements des trottoirs. Un DCE réel en compterait une quinzaine.

# 2. La fiche de paramètres — le seul travail du bureau d'études

C'est tout ce que le bureau d'études remplit. Le reste est produit par le standard.

| Paramètre | Valeur retenue | Valeurs admissibles |
| {MAITRE_OUVRAGE} | ASMA | Liste fermée |
| {OPERATION} | Lotissement Tafoukt — 4,2 ha, 180 lots | Texte libre |
| {REGIME_JURIDIQUE} | Compte propre | Compte propre / MOD |
| {LOTS_TRAITES} | VRD03, VRD11, VRD12 | Codes de la taxonomie v3.2 |
| {NATURE_TERRAIN} | TOUT_TERRAIN | TOUT_TERRAIN / ROCHEUX |
| {MATERIAU_CANALISATION} | Béton armé série 135 A | Béton armé / PVC-U / PEHD / fonte ductile |
| {DIAMETRE_COLLECTEUR} | DN 400 et DN 500 | DN 200 à DN 1000 |
| {PROFONDEUR_MOYENNE} | 2,20 m | 1,00 m à 4,00 m |
| {COMPACTAGE_TRANCHEE} | 95 % de l'OPM | 95 % OPM / 95 % OPN / 92 % OPM |
| {CLASSE_TAMPON} | D 400 en chaussée, C 250 en caniveau | A 15 à F 900 |
| {TYPE_BORDURE} | T2 béton préfabriqué | T1 / T2 / T3 / A2 / CS1 |
| {LARGEUR_TROTTOIR} | 2,00 m | 1,50 m à 2,00 m |
| {REVETEMENT_TROTTOIR} | Pavés autobloquants 8 cm | Pavés / dalles / béton balayé / enrobé |
| {TYPE_TRAVERSEE} | Bateau, raccordements latéraux ≤ 12 % | Bateau / abaissée / plateau |

Quatre de ces valeurs sont contraintes par un texte obligatoire : le standard refuse une largeur de trottoir inférieure à 1,50 m, une classe de tampon inférieure à D 400 en chaussée, une pente de bateau supérieure à 5 % et un compactage inférieur à celui du CCTG de l'opérateur. Le bureau d'études ne peut pas les contourner sans justification écrite.

# 3. Extrait du CPS type — Chapitre 3, prescriptions techniques

Texte produit par le standard à partir des paramètres ci-dessus. Les valeurs issues de la fiche sont soulignées par **les caractères gras**.

## Article 3.4 — Lot VRD03 : assainissement des eaux usées

**3.4.1 Canalisations.** Les collecteurs sont en **béton armé de série 135 A**, de diamètre nominal **DN 400 et DN 500**, conformes à la norme NM 10.1.027 (REF-046). Les tuyaux portent le marquage de la série, du diamètre et du fabricant. Les joints sont souples préfabriqués, à bague d'étanchéité en élastomère conforme à la NM 05.02.018.

**3.4.2 Lit de pose et enrobage.** Le lit de pose a une épaisseur minimale de 10 cm et est constitué de sable propre 0/10 contenant moins de 12 % de fines, d'équivalent de sable au moins égal à 50. L'enrobage est réalisé avec le même matériau, jusqu'à 20 cm au-dessus de la génératrice supérieure de la conduite. Ces dispositions sont celles du CCTG d'assainissement liquide urbain de l'ONEE — Branche Eau, tome 2, article 205.4 (REF-049).

**3.4.3 Remblai de tranchée.** Le remblai est compacté à **95 % de l'optimum Proctor modifié**, par couches élémentaires de 20 cm, selon l'essai de la NM 13.1.023 (REF-051). Les matériaux répondent aux classes A1, B2, B5, B6, D1 ou D2 du GMTR (REF-002). Les traversées de chaussée sont systématiquement remblayées en sable de concassage. La réfection définitive de la chaussée est conforme à la NM 13.1.220 (REF-041).

**3.4.4 Regards de visite.** Les regards sont conformes à la NM EN 1917 et, pour la certification, aux règles RCNM025 (REF-037). Les dispositifs de couronnement et de fermeture sont de **classe D 400 en chaussée et C 250 en caniveau**, conformes à la NM 10.9.001 (REF-045) : profondeur d'emboîtement d'au moins 50 mm pour la classe D 400 et 27 mm pour la classe C 250, masse surfacique minimale de 200 kg/m² et 100 kg/m², cote de passage d'au moins 600 mm, marquage de la classe et du fabricant.

**3.4.5 Épreuves d'étanchéité.** Les épreuves sont réalisées par tronçon, après remblai total des fouilles, selon la norme EN 1610 et l'article 327 du CCTG de l'ONEE (REF-050). La pression d'épreuve est de 0,04 MPa, soit 4 m de colonne d'eau, mesurée au radier de l'extrémité amont, sans dépasser 0,1 MPa à l'aval. Le délai d'imprégnation est de **24 heures pour les conduites en béton**. L'essai dure 30 minutes. Le volume d'eau d'appoint nécessaire pour rétablir le niveau initial ne dépasse pas **0,40 l/m² de paroi pour le DN 400 et 0,40 % du volume pour le DN 500** ; pour les regards en béton, 0,50 l/m². Tout tronçon non conforme est repris et éprouvé de nouveau aux frais de l'entrepreneur.

## Article 3.11 — Lot VRD11 : bordures et caniveaux

**3.11.1 Éléments préfabriqués.** Les bordures sont du **type T2 en béton préfabriqué**, conformes à la NM EN 1340. Les caniveaux préfabriqués sont conformes à la NM EN 1433.

**3.11.2 Pose.** Les bordures sont posées sur une fondation en béton de classe B1, avec un épaulement arrière. Les joints ont 1 cm au maximum.

**3.11.3 Accessibilité.** Aux traversées, la bordure est abaissée pour former un **bateau de 1,50 m de largeur minimale**, de pente inférieure à 5 %, avec des **raccordements latéraux de 12 % au maximum sur 0,50 m**, conformément à l'arrêté conjoint n° 2306-17 (REF-038) pris pour l'application du décret n° 2-11-246 (REF-042) et de la loi n° 10-03 (REF-043). Une bande d'éveil de vigilance de 60 cm est posée en amont de chaque traversée.

## Article 3.12 — Lot VRD12 : revêtements des trottoirs

**3.12.1 Revêtement.** Le trottoir a une **largeur libre de 2,00 m** et reçoit un revêtement en **pavés autobloquants en béton de 8 cm d'épaisseur**, conformes à la NM EN 1338, posés sur lit de sable selon la NM 13.1.279.

**3.12.2 Cheminement.** Le sol est non meuble, non glissant et sans obstacle. Le dévers transversal ne dépasse pas 2 %. Les ressauts sont limités à 2 cm, chanfreinés, et espacés d'au moins 2,50 m. Les trous et fentes des grilles d'arbres et des avaloirs sont inférieurs à 2 cm. Le mobilier urbain est implanté hors de la largeur libre.

> Toutes les références citées sont au statut « vérifié » dans la feuille Référentiels du classeur. Le standard n'affirme jamais une référence qui n'a pas été vérifiée sur sa source officielle.

# 4. Bordereau des prix — extrait

Les prix sont codés selon la règle du classeur : code du lot, point, numéro à trois chiffres. Le libellé, l'unité et la définition viennent de la bibliothèque de prix ; le bureau d'études ne les réécrit pas.

| Code | Désignation | Unité | Quantité |
| VRD03.001 | Déblais en tranchée en terrain de toute nature, profondeur jusqu'à 2,50 m, y compris blindage, épuisement et évacuation | m³ | 3 240 |
| VRD03.004 | Lit de pose en sable 0/10, épaisseur 10 cm | m³ | 162 |
| VRD03.005 | Enrobage de la conduite en sable 0/10, jusqu'à 20 cm au-dessus de la génératrice | m³ | 486 |
| VRD03.007 | Remblai de tranchée en matériau d'apport, compacté à 95 % de l'OPM par couches de 20 cm | m³ | 2 592 |
| VRD03.011 | Fourniture et pose de canalisation en béton armé série 135 A, DN 400, joint souple | ml | 820 |
| VRD03.012 | Fourniture et pose de canalisation en béton armé série 135 A, DN 500, joint souple | ml | 460 |
| VRD03.021 | Regard de visite en béton, profondeur jusqu'à 2,50 m, avec cunette et échelons | u | 42 |
| VRD03.031 | Dispositif de couronnement et de fermeture en fonte ductile, classe D 400, cote de passage 600 mm | u | 38 |
| VRD03.032 | Dispositif de couronnement et de fermeture en fonte ductile, classe C 250, cote de passage 600 mm | u | 4 |
| VRD03.041 | Épreuve d'étanchéité selon EN 1610, par tronçon de réseau | ml | 1 280 |
| VRD11.001 | Fourniture et pose de bordure de trottoir type T2 en béton préfabriqué, sur fondation béton | ml | 2 460 |
| VRD12.003 | Revêtement de trottoir en pavés autobloquants en béton de 8 cm sur lit de sable | m² | 4 920 |

Douze prix pour trois lots. Chaque prix porte un code stable : le même ouvrage reçoit le même code d'une opération à l'autre, ce qui rend les marchés comparables et alimente la base de prix.

# 5. Estimation confidentielle du maître d'ouvrage

Produite à partir des quantités ci-dessus et de la base de prix. **Montants fictifs, pour la démonstration seulement.**

| Code | Quantité | Prix unitaire médian (DH HT) | Montant (DH HT) | Observations |
| VRD03.001 | 3 240 m³ | 48,00 | 155 520 | 9 observations |
| VRD03.004 | 162 m³ | 190,00 | 30 780 | 7 observations |
| VRD03.005 | 486 m³ | 190,00 | 92 340 | 7 observations |
| VRD03.007 | 2 592 m³ | 62,00 | 160 704 | 11 observations |
| VRD03.011 | 820 ml | 610,00 | 500 200 | 8 observations |
| VRD03.012 | 460 ml | 780,00 | 358 800 | 5 observations |
| VRD03.021 | 42 u | 6 400,00 | 268 800 | 9 observations |
| VRD03.031 | 38 u | 2 950,00 | 112 100 | 6 observations |
| VRD03.032 | 4 u | 2 400,00 | 9 600 | 3 observations — peu fiable |
| VRD03.041 | 1 280 ml | 18,00 | 23 040 | 4 observations |
| VRD11.001 | 2 460 ml | 165,00 | 405 900 | 12 observations |
| VRD12.003 | 4 920 m² | 240,00 | 1 180 800 | 10 observations |
| | | **Total HT** | **3 298 584** | |

| Indicateur | Valeur | Lecture |
| Estimation médiane | 3 298 584 DH HT | Valeur retenue pour l'estimation confidentielle |
| Fourchette basse (1er quartile) | 2 969 000 DH HT | Une offre en dessous est examinée comme anormalement basse |
| Fourchette haute (3e quartile) | 3 727 000 DH HT | Une offre au-dessus demande une justification |
| Seuil de contrôle du règlement | ± 20 % de l'estimation | Article 43 du règlement de passation d'ASMA (REF-021) |
| Prix fondés sur moins de 3 observations | 0 sur 12 | Aucun prix écarté |
| Prix signalés « peu fiables » | 1 sur 12 | VRD03.032, 3 observations : à confirmer |
| Ancienneté médiane des observations | 14 mois | Prix actualisés par l'index de révision |

L'estimation se lit en une page et chaque ligne est traçable : on sait de combien de marchés adjugés vient chaque prix, et depuis quand.

# 6. Ce que cet exemple démontre

| Promesse du programme | Ce que montre le dossier |
| Le bureau d'études ne rédige plus | 14 valeurs renseignées en section 2 produisent les sections 3 et 4 en entier |
| Les références sont sûres | Chaque prescription cite un texte vérifié du classeur, avec son code REF |
| Les marchés deviennent comparables | 12 prix codés, réutilisables d'une opération à l'autre |
| L'estimation est outillée | Une estimation médiane, une fourchette et un indicateur de fiabilité par prix |
| Le maître d'ouvrage garde la main | Les valeurs imposées par un texte obligatoire ne sont pas modifiables par le BET |

**Ce qui n'est pas encore fait.** Le CPS type et la bibliothèque de prix de la famille Espaces verts sont produits pendant le pilote, validés le 25 novembre 2026 ; la VRD suit le 9 décembre. La base de prix est alimentée à partir de la mi-décembre avec les BDDE adjugés déjà rassemblés. Les montants de ce dossier ne seront remplacés par de vraies valeurs qu'à ce moment-là.

**Ce dossier n'est pas un DCE.** Il ne comporte ni chapitre administratif, ni plans, ni pièces du marché. Il sert uniquement à montrer la forme du résultat attendu.
