# 1. Vue d'ensemble de la phase 0

La phase 0 prépare le pilote Espaces verts en huit actions, sur environ trois semaines. Chaque action a un porteur, un livrable et un critère de fin : la phase 0 n'est close que lorsque les huit critères sont remplis.

| N° | Action | Porteur | Durée | Dépend de |
| 0.1 | Trancher les 9 points de décision du guide | Direction technique | 1 semaine | — |
| 0.2 | Relecture juridique du noyau v3 | Service marchés / juriste | 1 semaine | 0.3 |
| 0.3 | Règlement des achats d'ASMA en donnée d'entrée | Service marchés | 1 semaine | — |
| 0.4 | Figer la taxonomie et les codes lots (fait le 23/09/2026) | Chef de projet | 1 semaine | 0.1 |
| 0.5 | Créer le classeur cible | Chef de projet | 3 jours | 0.4 |
| 0.6 | Feuille Référentiels de la famille EVP | Ingénieur EV + juriste | 1 à 2 semaines | 0.5 |
| 0.7 | Rassembler les sources du pilote | Chef de projet | 2 à 3 semaines | — |
| 0.8 | Désigner les responsables et la périodicité de revue | Direction | 3 jours | — |

Enchaînement conseillé :

| Semaine | Actions |
| Semaine 1 | Lancer 0.1, 0.3, 0.7 et 0.8 (sans prérequis) |
| Semaine 2 | 0.2 (dès que la fiche 0.3 est prête), 0.4 puis 0.5 |
| Semaine 3 | 0.6, fin de 0.7, revue de sortie de phase 0 |

La collecte des sources (0.7) est lancée dès le premier jour : c'est l'action la plus longue et celle qui dépend le plus de tiers.

# 2. Démarche détaillée par action

## Action 0.1 — Trancher les 9 points de décision du guide

@@O|Obtenir une décision datée sur chacun des 9 points ouverts de la section 9 du guide, pour figer le découpage des lots, la forme du classeur et le rôle des référentiels.
@@A|Porteur : direction technique. Contributeurs : service marchés, chef de projet.
@@D|1 semaine (préparation 3 jours, réunion 1 h 30, relevé 1 jour).
@@P|Guide pratique (section 9) ; tableaux B8 des quatre prompts v3.
@@L|Relevé de décisions signé ; prompts et plan d'action mis à jour.
@@C|Chacun des 9 points porte une décision datée et un décideur identifié.

1. **Recenser les points.** Reprendre les 9 points de la section 9 du guide. Y ajouter les points apparus dans les tableaux B8 des prompts v3 qui touchent plusieurs familles (limite de l'eau d'irrigation, génie civil de l'éclairage, VRD dans le Bâtiment).
2. **Préparer une fiche par point.** Question posée, options possibles, avantages et inconvénients, recommandation du guide, conséquence de chaque option sur les prompts et le classeur.
3. **Classer les points par portée.** Traiter en premier les points structurants (forme du classeur, périmètre du standard, rôle des référentiels étrangers), puis les points de découpage des lots, puis la gouvernance.
4. **Diffuser le dossier** aux participants trois jours avant la réunion.
5. **Tenir la réunion de décision.** Un point à la fois ; toute décision reportée reçoit un responsable et une date butoir.
6. **Rédiger le relevé de décisions** le jour même et le faire viser.
7. **Reporter les décisions** dans les tableaux B8 des prompts (nouvelle version numérotée) et dans le plan d'action.

## Action 0.2 — Relecture juridique du noyau v3

@@O|Faire valider par un juriste marchés les règles juridiques du noyau : verrou de qualification, place du CCAG-T, trame du Chapitre 1 et références réglementaires.
@@A|Porteur : service marchés ou juriste désigné. Contributeur : chef de projet.
@@D|1 semaine.
@@P|Fiche de synthèse du règlement des achats d'ASMA (action 0.3) ; noyau v3.
@@L|Noyau annoté, puis noyau validé en nouvelle version (A-v3.x).
@@C|Chaque question de la grille de relecture a reçu une réponse ; les corrections sont intégrées.

1. **Extraire les sections à relire** : section 3 (verrou juridique), section 4 (statut des références), section 7.1 (trame du Chapitre 1), contrôles C7 et C8 de la section 14.
2. **Remettre au juriste une grille de relecture** : le tableau des régimes par nature de maître d'ouvrage est-il exact ? Le cas d'ASMA (société de développement local) et le cas de la maîtrise d'ouvrage déléguée sont-ils bien traités ? Le CCAG-T est-il applicable par renvoi du règlement d'ASMA ? La trame du Chapitre 1 couvre-t-elle toutes les clauses obligatoires du règlement ? Les références (décret n° 2-22-431, CCAG-T) sont-elles exactes et en vigueur ?
3. **Recueillir les annotations** directement dans le document (commentaires ou modifications suivies).
4. **Intégrer les corrections** dans le noyau et le faire passer en nouvelle version, appliquée aux quatre prompts en même temps.
5. **Faire viser la version finale** par le juriste.

## Action 0.3 — Règlement des achats d'ASMA en donnée d'entrée

@@O|Disposer du texte qui régit les marchés d'ASMA et le traduire en données exploitables par le prompt (valeurs de {REGIME_JURIDIQUE}, clauses du Chapitre 1, champs à compléter).
@@A|Porteur : service marchés. Contributeur : chef de projet.
@@D|1 semaine.
@@P|Aucun.
@@L|Dossier « régime juridique ASMA » et fiche de synthèse visée ; entrées dans la feuille Référentiels.
@@C|La fiche de synthèse répond à toutes les questions de la grille et est visée par le service marchés.

1. **Identifier les deux régimes à couvrir** : marchés passés par ASMA pour son propre compte (règlement des achats d'ASMA) et marchés passés en maîtrise d'ouvrage déléguée pour un tiers (régime du délégant, souvent le décret n° 2-22-431, sauf stipulation contraire de la convention).
2. **Collecter les documents** :
    - le règlement des achats ou des marchés en vigueur et ses modificatifs ;
    - la délibération du conseil d'administration qui l'approuve ;
    - toute clause de renvoi au CCAG-T ou au décret n° 2-22-431 ;
    - le CPS administratif et le règlement de consultation types utilisés actuellement ;
    - deux ou trois conventions de maîtrise d'ouvrage déléguée types ;
    - les notes internes sur les seuils, les commissions et les délégations de signature.
3. **Analyser avec une grille de lecture**, en relevant l'article exact pour chaque question : champ d'application ; modes de passation et seuils ; cautionnements et retenue de garantie ; avances ; révision des prix ; délais de paiement et intérêts moratoires ; pénalités et plafond ; réceptions et délai de garantie ; sous-traitance ; assurances ; résiliation ; litiges et juridiction ; préférence nationale ; renvoi au CCAG-T.
4. **Rédiger la fiche de synthèse** du régime ASMA (une à deux pages), jointe ensuite à chaque exécution du prompt.
5. **Créer les entrées correspondantes** dans la feuille Référentiels (règlement d'ASMA, CCAG-T s'il y a renvoi), avec leur statut.
6. **Faire viser la fiche** par le service marchés. Elle sert ensuite de base à la relecture 0.2.

## Action 0.4 — Figer la taxonomie et les codes lots

@@O|Arrêter la liste définitive des familles et des lots, avec des codes stables, pour que chaque prix du futur catalogue ait un code qui ne changera plus.
@@A|Porteur : chef de projet. Contributeurs : référents techniques par famille.
@@D|1 semaine.
@@P|Taxonomie des corps d'état (guide pratique, section 4) ; décisions de l'action 0.1.
@@L|Taxonomie v3 validée le 23/09/2026 ; tableaux B2 des quatre paquets mis à jour.
@@C|Chaque lot a un code définitif ; les paquets utilisent ces codes ; la famille EVP est complète.

1. **Partir de la taxonomie du guide** (150 lots prévus, 15 familles) et vérifier qu'il est cohérent avec les décisions de l'action 0.1 (lots séparés ou fusionnés, exclusions).
2. **Arrêter la règle de codification** : code famille en trigramme + numéro de lot sur deux chiffres (exemple EVP04), avec la règle qu'un code attribué n'est jamais réutilisé.
3. **Faire la correspondance** entre les codes provisoires des paquets (K01 à K12, I01 à I10, etc.) et les codes définitifs (EVP01 à EVP14, VRD01 à VRD19, etc.).
4. **Statuer sur les lots d'extension** (non issus des prompts sources) : actifs dès le pilote ou activés plus tard.
5. **Compléter les colonnes utiles** : famille, statut du lot (source ou extension), lots en interface, exclusions.
6. **Mettre à jour les tableaux B2** des quatre paquets, en commençant par la famille EVP.
7. **Faire valider la taxonomie** par les référents techniques et l'enregistrer comme version de référence.

> Réalisée le 23/09/2026 : taxonomie v3 validée (107 lots, 13 familles, codes trigramme). Familles REH et TRA retirées du projet actuel ; codes reportés dans les paquets EVP, VRD, ECL (v3.2) et Bâtiment (v3.1).

## Action 0.5 — Créer le classeur cible

@@O|Mettre en place le modèle Excel vide qui recevra le référentiel et les prix, avec une structure identique pour toutes les familles.
@@A|Porteur : chef de projet.
@@D|3 jours.
@@P|Taxonomie v3 validée (action 0.4) ; section 12.3 du noyau.
@@L|Modèle Excel vide, testé, déposé à un emplacement partagé.
@@C|Le modèle accepte 5 lignes de test sans erreur et les listes déroulantes fonctionnent.

1. **Créer les feuilles** : Lisez-moi (mode d'emploi, versions), Taxonomie, Référentiels, Paramètres, Prix_EVP (puis une feuille Prix par famille), Listes (valeurs autorisées).
2. **Créer les colonnes** exactement comme prévu à la section 12.3 du noyau, dans le même ordre sur toutes les feuilles Prix.
3. **Ajouter les contrôles de saisie** : listes déroulantes pour les statuts (obligatoire, contractuel, volontaire, supplétif, abrogé ; vérifié, à vérifier, non vérifiable ; brouillon, vérifié, validé), codes famille et lot tirés de la taxonomie.
4. **Mettre en forme** : tableaux structurés Excel, en-têtes figés, filtres, en-têtes protégés.
5. **Fixer la règle de nommage et de version** du fichier et son emplacement partagé, avec des droits de modification limités.
6. **Tester** avec cinq lignes fictives, puis les supprimer.

## Action 0.6 — Feuille Référentiels de la famille EVP

@@O|Constituer la première base de références vérifiées pour la famille Espaces verts, afin que le pilote n'affirme aucune référence non vérifiée.
@@A|Porteur : ingénieur Espaces verts. Contributeur : juriste (statut juridique des textes).
@@D|1 à 2 semaines.
@@P|Classeur cible (action 0.5) ; liste B3 du paquet EVP ; sources du pilote (action 0.7) pour les références qu'elles citent.
@@L|Feuille Référentiels EVP renseignée (20 à 40 entrées).
@@C|Chaque référence de la liste B3 a un statut juridique et un statut de vérification ; les textes obligatoires sont tous « vérifiés ».

1. **Dresser la liste de départ** : références de la rubrique B3 du paquet EVP, complétées par celles citées dans les CPS sources du pilote.
2. **Rechercher la source officielle** de chaque référence : Bulletin officiel pour les lois, décrets et arrêtés ; catalogue IMANOR pour les normes marocaines (numéro et intitulé) ; édition en vigueur pour les fascicules et normes étrangères.
3. **Renseigner chaque ligne** : type, numéro, intitulé, édition, statut juridique, champ d'application, statut de vérification, source et date de vérification.
4. **Traiter les cas difficiles** : une norme payante dont seul l'intitulé est vérifié reçoit le statut « non vérifiable » ; une référence introuvable reste « à vérifier » avec l'action attendue.
5. **Faire relire** le statut juridique par le juriste et la pertinence technique par l'ingénieur.
6. **Passer les lignes relues** au statut « vérifié ».

## Action 0.7 — Rassembler les sources du pilote

@@O|Réunir les documents réels sur lesquels le pilote Espaces verts sera construit et testé.
@@A|Porteur : chef de projet. Contributeurs : chefs de projet opérationnels, service marchés.
@@D|2 à 3 semaines (à lancer dès le premier jour).
@@P|Aucun.
@@L|Dossier sources pilote, classé et documenté.
@@C|3 à 4 CPS et 3 à 4 BDDE adjugés disponibles, lisibles et décrits par une fiche d'identification.

1. **Fixer les critères de choix** : CPS récents (de préférence postérieurs à l'entrée en vigueur du décret n° 2-22-431), représentatifs des travaux d'ASMA (plantations, irrigation, entretien), dossiers complets (CPS et bordereau), tailles de marché variées.
2. **Chercher les documents** : archives des marchés d'ASMA, chefs de projet opérationnels, bureaux d'études partenaires ; à défaut, DCE publiés par des maîtres d'ouvrage comparables.
3. **Récupérer les BDDE réellement adjugés** : bordereau de l'entreprise attributaire, tel qu'il figure au marché signé, et non l'estimation initiale.
4. **Contrôler la lisibilité** : texte natif de préférence ; un document scanné est passé en reconnaissance de caractères (OCR) et vérifié.
5. **Classer et nommer les fichiers** selon une règle unique (par exemple EV_S01_CPS.pdf, EV_S01_BDDE.xlsx) dans un dossier à accès restreint : les BDDE adjugés sont confidentiels.
6. **Remplir une fiche d'identification par source** : année, maître d'ouvrage, objet, montant, lots couverts, format, qualité du texte.

## Action 0.8 — Désigner les responsables et la périodicité de revue

@@O|Nommer les personnes qui valident, relisent et tiennent à jour le standard, pour que chaque statut « validé » ait un auteur identifié.
@@A|Porteur : direction. Contributeur : chef de projet.
@@D|3 jours.
@@P|Section « Gouvernance » du plan d'action.
@@L|Note de désignation signée et tableau des responsabilités.
@@C|Chaque rôle a un titulaire et un suppléant ; la périodicité de revue est fixée.

1. **Lister les rôles** : sponsor, chef de projet, référent juridique, référent technique par famille (en priorité la famille EVP), BET testeur, responsable de la veille réglementaire.
2. **Établir le tableau des responsabilités** : qui rédige, qui vérifie, qui valide, qui est informé, pour chaque type de livrable (prompt, CPS type, prix, référentiel).
3. **Fixer la périodicité de revue** : revue complète annuelle, plus une réouverture à chaque publication ou abrogation d'un texte concerné.
4. **Désigner les titulaires et leurs suppléants** par une note de la direction.
5. **Communiquer la note** aux personnes concernées et aux bureaux d'études qui participeront aux tests.

# 3. Revue de sortie de la phase 0

La revue de sortie, présidée par le sponsor, autorise ou non le lancement du pilote.

| Critère | Action | Vérifié |
| Les 9 points de décision sont tranchés et le relevé est signé | 0.1 | ☐ |
| Le noyau est validé par le juriste | 0.2 | ☐ |
| La fiche du régime juridique d'ASMA est visée | 0.3 | ☐ |
| La taxonomie v3 est figée et les codes EVP sont définitifs | 0.4 | ☑ |
| Le classeur cible est en place et testé | 0.5 | ☐ |
| La feuille Référentiels EVP est au moins partiellement vérifiée | 0.6 | ☐ |
| Les sources du pilote sont rassemblées et documentées | 0.7 | ☐ |
| Les responsables sont désignés | 0.8 | ☐ |
