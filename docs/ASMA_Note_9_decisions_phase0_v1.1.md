# 1. Objet et mode d'emploi

Cette note prépare l'action 0.1 de la phase 0 : obtenir une décision datée sur chacun des 9 points laissés ouverts par la section 9 du guide pratique. Ces points conditionnent le dimensionnement du classeur de prix et la robustesse de la base de référentiels ; le guide demande qu'ils soient tranchés avant le lancement du pilote.

Pour chaque point, la fiche donne la question posée, les options possibles, leurs avantages et inconvénients, la recommandation du guide et ses conséquences sur les prompts et le classeur. Les deux dernières lignes de chaque fiche sont remplies en réunion.

> Règle de séance : un point à la fois. Toute décision reportée reçoit un responsable et une date butoir. Le relevé de décisions (section 4) est rédigé le jour même et visé par la direction technique.

Les points sont classés par portée, comme le prévoit la démarche : d'abord les points structurants, puis le découpage des lots, enfin la gouvernance.

| N° | Point | Portée | Recommandation du guide |
| 1 | Une feuille de prix par lot ou par famille | Structurant | Par famille (environ 15 feuilles) |
| 2 | Périmètre du standard : défaut seul ou défaut + options | Structurant | Défaut + options activables par paramètre |
| 7 | Rôle des fascicules du CCTG français | Structurant | Supplétif uniquement, statut qualifié explicitement |
| 3 | Lots hors périmètre (barrages, stations de traitement, travaux souterrains) | Découpage | Exclure explicitement du standard |
| 4 | Protection phytosanitaire : lot propre ou volet de l'entretien | Découpage | Volet de l'entretien horticole |
| 5 | Détection incendie : fusion avec l'extinction ou séparation | Découpage | Séparer (corps de métier distinct) |
| 6 | Subdivision du lot courant faible | Découpage | Quatre lots, regroupables à la consultation |
| 8 | Correspondance lots / secteurs de qualification Q&C | Gouvernance | À vérifier sur le tableau officiel du ministère |
| 9 | Validation de la base de référentiels | Gouvernance | Version 1.0 figée + clause de réouverture obligatoire |

# 2. Points structurants

## Point 1 — Une feuille de prix par lot ou par famille

| Rubrique | Contenu |
| Question | Le classeur cible (action 0.5) contient-il une feuille de prix par famille ou une feuille par lot ? |
| Options | A : une feuille par famille, environ 15 feuilles, chaque ligne portant son code lot. B : une feuille par lot, environ 150 feuilles. |
| Avantages et inconvénients | A : classeur maniable, colonnes identiques partout, filtrage par code lot, consolidation facile pour la base de prix ; les familles les plus larges (VRD, 22 lots) donnent des feuilles longues. B : lecture directe par lot, mais classeur très fragmenté, maintenance lourde et risque d'écarts de structure entre feuilles. |
| Recommandation du guide | **Par famille (environ 15 feuilles).** |
| Conséquences | Action 0.5 : créer Prix_EVP, puis une feuille Prix par famille, avec une colonne code lot obligatoire et une liste déroulante tirée de la taxonomie. Le volet 0.5 de l'outil de suivi est déjà organisé par famille. |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 2 — Périmètre du standard : défaut seul ou défaut + options

| Rubrique | Contenu |
| Question | Le CPS type et le catalogue décrivent-ils une seule solution par défaut, ou une solution par défaut avec des options activables par paramètre ? |
| Options | A : défaut seul. B : défaut + options activables par paramètre {…}. |
| Avantages et inconvénients | A : standard plus simple et plus rapide à valider, mais les bureaux d'études réécriront les descriptifs pour chaque variante, ce qui contredit l'objectif du projet. B : couvre les variantes courantes sans réécriture (par exemple arrosage goutte-à-goutte ou par aspersion) ; en contrepartie, plus de paramètres à définir, à contrôler et à tester. |
| Recommandation du guide | **Défaut + options activables par paramètre.** |
| Conséquences | Les paquets v3 listent les paramètres et leurs valeurs admissibles ; la colonne « paramètres admissibles » des feuilles de prix devient obligatoire ; la liste des paramètres est validée lors de l'arbitrage du pilote (phase 1) et éprouvée par le test métier du BET. |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 7 — Rôle des fascicules du CCTG français dans la base de référentiels

| Rubrique | Contenu |
| Question | Quelle valeur donner aux fascicules du CCTG français, souvent cités par les CPS sources ? |
| Options | A : supplétif uniquement, avec un statut qualifié explicitement. B : contractuel par renvoi systématique dans le CPS type. C : exclus de la base. |
| Avantages et inconvénients | A : conserve un repère technique utile sans l'imposer, cohérent avec la règle de qualification de chaque référence (guide, section 2.1). B : simple à rédiger, mais rend opposables des textes étrangers, parfois non disponibles pour les entreprises. C : perte d'un repère utile là où aucun texte marocain n'existe. |
| Recommandation du guide | **Supplétif uniquement, statut qualifié explicitement.** |
| Conséquences | Feuille Référentiels : statut « supplétif » pour chaque fascicule, avec numéro et édition vérifiés (V21, E26, EP25, BT24 des listes de collecte). Le CPS type ne rend un fascicule contractuel que par un renvoi explicite, décidé au cas par cas. À faire relire par le juriste (action 0.2). |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

# 3. Découpage des lots et gouvernance

## Point 3 — Lots hors périmètre proposé

| Rubrique | Contenu |
| Question | Les barrages, stations de traitement et travaux souterrains font-ils partie du standard ? |
| Options | A : exclusion explicite du standard. B : intégration comme lots d'extension. C : aucune mention (exclusion implicite). |
| Avantages et inconvénients | A : périmètre clair, aucun CPS type produit sans sources ni référent compétent ; ces ouvrages restent traités au cas par cas. B : couverture plus large, mais sans sources ASMA ni expertise interne pour les valider. C : risque de confusion avec la famille OAH (ouvrages d'art et hydraulique) et avec la VRD. |
| Recommandation du guide | **Exclure explicitement du standard.** |
| Conséquences | Liste d'exclusions inscrite dans la taxonomie v3 validée le 23/09/2026 (action 0.4) et dans la rubrique B2 des paquets concernés ; limite à préciser avec les familles VRD et OAH. |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 4 — Protection phytosanitaire : lot propre ou volet de l'entretien horticole

| Rubrique | Contenu |
| Question | Dans la famille EVP, la protection phytosanitaire est-elle un lot à part ou un volet du lot d'entretien horticole ? |
| Options | A : volet de l'entretien horticole. B : lot propre. |
| Avantages et inconvénients | A : conforme à la pratique courante des marchés d'entretien, évite les doublons de prix et les interfaces entre entreprises. B : meilleure visibilité et traçabilité des traitements, mais lot souvent trop petit pour être consulté seul. |
| Recommandation du guide | **Volet de l'entretien horticole.** |
| Conséquences | Taxonomie EVP sans lot phytosanitaire distinct ; les prescriptions d'usage des produits (références E17 et E18 de la collecte Espaces verts) sont rattachées au lot d'entretien dans le paquet K. |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 5 — Détection incendie : fusionner avec l'extinction ou séparer

| Rubrique | Contenu |
| Question | Dans les lots techniques du bâtiment, la détection incendie et l'extinction forment-elles un seul lot ou deux ? |
| Options | A : deux lots séparés. B : un lot unique « sécurité incendie ». |
| Avantages et inconvénients | A : correspond à deux corps de métier distincts (courant faible pour la détection, fluides pour l'extinction), prix plus précis ; une interface est à décrire (asservissements, essais coordonnés). B : un seul interlocuteur, mais un lot hétérogène que peu d'entreprises couvrent entièrement. |
| Recommandation du guide | **Séparer (corps de métier distinct).** |
| Conséquences | Deux lots distincts dans les familles du Bâtiment (FLU02 extinction et ELB06 détection dans la taxonomie v3), avec une interface explicite dans le paquet Bâtiment. |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 6 — Subdivision du lot courant faible

| Rubrique | Contenu |
| Question | Le courant faible du bâtiment (câblage, sonorisation, contrôle d'accès, vidéo) forme-t-il un lot unique ou plusieurs lots ? |
| Options | A : quatre lots, regroupables au moment de la consultation. B : un lot unique. C : deux lots (réseaux, sûreté). |
| Avantages et inconvénients | A : bibliothèque de prix plus précise et réutilisable, regroupement possible selon la taille du projet ; plus de lots à tenir à jour. B : simple, mais descriptifs hétérogènes et prix moins comparables. C : compromis, moins souple que A. |
| Recommandation du guide | **Quatre lots, regroupables à la consultation.** |
| Conséquences | Famille ELB : quatre lots courant faible (ELB02 à ELB05). Limite à préciser avec la vidéoprotection urbaine de la famille ECL (vidéo du bâtiment ou vidéo de l'espace public). |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 8 — Correspondance entre les lots et les secteurs de qualification Q&C

| Rubrique | Contenu |
| Question | Chaque lot de la taxonomie est-il rattaché à un secteur de qualification et de classification (Q&C) des entreprises ? |
| Options | A : rattachement établi après vérification sur le tableau officiel du ministère. B : rattachement proposé dès maintenant, sans vérification. C : pas de rattachement. |
| Avantages et inconvénients | A : fiable et opposable, mais demande une vérification préalable. B : rapide, mais risque d'exiger une qualification erronée dans le règlement de consultation. C : perte d'une aide utile à la rédaction des dossiers. |
| Recommandation du guide | **À vérifier sur le tableau officiel du ministère ; non confirmé à ce stade.** |
| Conséquences | Désigner qui vérifie et pour quand. En attendant, la colonne Q&C de la taxonomie reste au statut « à vérifier » et le CPS type n'affirme aucune qualification. |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Point 9 — Validation de la base de référentiels : unique ou avec clause de réouverture

| Rubrique | Contenu |
| Question | La base de référentiels est-elle validée une fois pour toutes, ou figée avec une obligation de réouverture ? |
| Options | A : version 1.0 figée, avec clause de réouverture obligatoire à chaque évolution d'un texte source. B : validation unique. |
| Avantages et inconvénients | A : base stable pour le pilote et toujours à jour ; demande une veille réglementaire désignée. B : plus simple, mais la base vieillit et finit par citer des textes abrogés. |
| Recommandation du guide | **Version 1.0 figée, plus clause de réouverture obligatoire à chaque évolution d'un texte source.** |
| Conséquences | Action 0.8 : désigner le responsable de la veille réglementaire, revue complète annuelle et réouverture à chaque publication ou abrogation. Cycle brouillon → vérifié → validé pour chaque entrée (guide, section 5.3). |
| Décision retenue | ☐ Recommandation   ☐ Autre option : …………………………… |
| Décideur et date | …………………………………………… |

## Points complémentaires issus des tableaux B8

La démarche prévoit d'ajouter à la réunion les points des tableaux B8 qui touchent plusieurs familles. Le guide ne fixe pas de recommandation pour ces points ; le plan d'action retient un principe commun : une interface explicite dans chaque paquet concerné, et une mise à jour conjointe des paquets quand elle change.

| Point | Familles | Question à trancher |
| Limite de l'eau d'irrigation | EVP / VRD | Où s'arrête la VRD et où commence le réseau d'arrosage (point de livraison, regard, vanne de sectionnement) ? Décidé le 23/09/2026 (décision I-1) : point de livraison = vanne de tête ou regard de comptage. |
| Génie civil de l'éclairage | ECL / VRD | Les tranchées, fourreaux et massifs d'éclairage relèvent-ils de la VRD ou de l'éclairage public ? Décidé le 23/09/2026 (décision I-2) : famille ECL, option d'intégration à la VRD. |
| VRD dans le Bâtiment | Bâtiment / VRD | Les réseaux extérieurs et voiries d'une opération de bâtiment relèvent-ils du paquet Bâtiment ou de la famille VRD ? |

# 4. Relevé de décisions

| N° | Point | Décision retenue | Décideur | Date |
| 1 | Feuille de prix par lot ou par famille | | | |
| 2 | Périmètre du standard | | | |
| 3 | Lots hors périmètre | | | |
| 4 | Protection phytosanitaire | | | |
| 5 | Détection incendie | | | |
| 6 | Subdivision du courant faible | | | |
| 7 | Rôle des fascicules du CCTG | | | |
| 8 | Correspondance lots / Q&C | | | |
| 9 | Validation de la base de référentiels | | | |

Décisions reportées : responsable et date butoir pour chacune. Après la réunion, les décisions sont reportées dans les tableaux B8 des prompts (nouvelle version numérotée) et dans le plan d'action, puis consignées dans le journal de l'outil de suivi.

Visa de la direction technique : ……………………………………   Date : ……………………
