# Classeur des référentiels et de la bibliothèque de prix type — modèle v0.10

Action 0.5 de la phase 0 — version 0.10 du 27/09/2026. Fichier : ASMA_Classeur_Referentiels_Prix_v0.10_20260927.xlsx.

Ce classeur est le fichier cible du standard : il reçoit, famille par famille, la feuille Référentiels, le dictionnaire des Paramètres et la bibliothèque de prix type produits par les prompts v3 (Fichier 3, section 12.3 du noyau). Sa structure est identique pour les 13 familles de la taxonomie v3. Il ne contient aucun montant, aucune quantité et aucune source nommée.

# Feuilles

| Feuille | Contenu | Qui saisit |
| Lisez-moi | Mode d’emploi, règles et historique des versions | Chef de projet |
| Tableau de bord | Contrôles automatiques par famille : lots couverts, lignes par statut, codes non conformes, doublons ; état des référentiels | Formules, aucune saisie |
| Taxonomie | Les 107 lots de la taxonomie v3.1 (validée le 23/09/2026, contenus EVP précisés le 24/09/2026) | Verrouillée |
| Listes | Valeurs autorisées des listes déroulantes | Chef de projet |
| Référentiels | Une ligne par texte ou norme cité, toutes familles | Référent juridique et référents techniques |
| Paramètres | Dictionnaire des paramètres {…}, toutes familles | Référents techniques |
| Prix_EVP à Prix_EQS | 13 feuilles de prix type, colonnes identiques ; EVP (pilote), VRD et ECL en tête | Référent technique de la famille |

# Colonnes

**Référentiels** : Famille ; Code référence (REF-nnn) ; Type ; Numéro ; Intitulé ; Édition ; Statut juridique ; Champ d’application ; Statut de vérification ; Source de vérification ; Date de dernière vérification ; Emplacement du fichier.

**Paramètres** : Famille ; Nom du paramètre ({NOM}) ; Grandeur ; Unité ; Valeurs admissibles ; Prix qui l’utilisent.

**Prix** : Code famille ; Code lot ; Code prix unifié ; Désignation unifiée ; Descriptif unifié paramétré ; Paramètres admissibles ; Unité ; Règle de mesurage ; Prestations comprises ; Référence de l’article du CPS type ; Référentiels liés ; Statut de validation ; Observations.

La colonne « Famille » des feuilles Référentiels et Paramètres est le seul ajout à la section 12.3 : un classeur unique sert les 13 familles (« COMMUN » pour un élément partagé).

# Contrôles de saisie

- Listes déroulantes : famille, type de texte, statut juridique, champ d’application, statut de vérification, statut de validation (brouillon, vérifié, validé, retiré), unité, grandeur ; code lot limité aux lots de la famille de la feuille.
- Cellule rouge : code prix hors format [code lot].[nnn] ou ne commençant pas par le code lot, code en double, code référence hors format REF-nnn, paramètre mal écrit, référence « vérifiée » sans source ni date.
- En-têtes et taxonomie protégés (sans mot de passe) ; 500 lignes de saisie préparées par feuille, filtres et tri autorisés.

# Test (étape 6)

Cinq lignes fictives saisies dans Prix_VRD dont un code non conforme et un doublon : le tableau de bord a compté 5 lignes (3 brouillons, 1 vérifiée, 1 validée), 2 lots couverts, 1 code non conforme et 2 codes en double, et affiché « À corriger ». Les listes nommées renvoient 13 unités, 19 lots VRD et 14 familles. Lignes supprimées ensuite ; aucune erreur de formule.

# Version 0.2

Première entrée de la feuille Référentiels : REF-001 (famille VRD), cahier des prix assainissement 2026 de la SRM Souss-Massa, type « prescription d’opérateur », statut juridique « contractuel » (si le marché le cite), statut de vérification « à vérifier » tant que la version officielle des prescriptions de l’opérateur n’est pas obtenue.

# Version 0.3

REF-002 (COMMUN, familles VRD et TER) : Guide marocain pour les terrassements routiers (GMTR), fascicules I et II, édition 2001, type « guide technique », statut « supplétif » (contractuel si le marché le cite), « à vérifier » jusqu’à l’obtention d’une copie officielle et la confirmation de l’édition en vigueur.

# Version 0.4

Colonne « Emplacement du fichier » dans la feuille Référentiels et règle de nommage du dossier REFERENTIEL_TECHNIQUE_VRD : [code référence]_[sigle]_[partie]_[édition]_[officiel ou copie], par exemple REF-003_CPC_F01_1983_copie.doc. Les CPS et bordereaux sources restent hors de ce dossier (dossier restreint des sources).

| Code | Référence | Statut juridique | Remarque |
| REF-003 | CPC routier, fascicule 1 (1983) | Contractuel si cité | Arrêté n° 451-83 |
| REF-004 | CPC routier, fascicule 2 (1983) | Supplétif | Non repris : clauses financières ASMA, CPS, CCAG-T |
| REF-005 | CPC routier, fascicule 3 (1983) | Contractuel si cité | Classification des sols remplacée par le GMTR |
| REF-006 | CPC routier, fascicule 4 (1983) | Contractuel si cité | Assainissement routier, pas les réseaux urbains |
| REF-007 à REF-010 | CPC routier, fascicule 5, cahiers 1 à 4 (1983) | Contractuel si cité | Cahier 4 : désignations anciennes (GBB, EB) |
| REF-011 | CPC routier, fascicule 5, cahier 5 (1983) | Contractuel si cité | Texte d’approbation à identifier |
| REF-012 | CPC routier, fascicule 6 (1990) | Contractuel si cité | Arrêté n° 732-89 ; milieu désertique |

Toutes ces références sont « à vérifier » : les fichiers reçus sont des copies Word ressaisies.

# Version 0.5

REF-013 (VRD) : Catalogue marocain des structures types de chaussées neuves, édition 1995 — classes de trafic TPL1 à TPL6, portance P1 à P4, structures, entretien, profils en travers. Guide technique, supplétif, « à vérifier » (copie non officielle, édition en vigueur à confirmer). Emplacement : 04_CATALOGUES.

# Version 0.6

Feuille Taxonomie mise à jour en v3.1 : EVP03 devient « Plantation et transplantation d’arbres et de palmiers » ; EVP04 couvre la transplantation des arbustes ; EVP01 couvre l’abattage, le dessouchage et la protection des arbres conservés. Codes inchangés.

# Version 0.7

REF-014 (VRD) : cahier des prix eau potable 2026 de la SRM Souss-Massa — bordereau et définitions des prix (conduites PVC et PEHD, fonte, robinetterie, poteaux d’incendie, branchements, rinçage et stérilisation). Prescription d’opérateur, « à vérifier » : HT ou TTC non précisé, mentions RAMSA à actualiser. Emplacement : 06_OPERATEURS.

REF-015 (ECL) : cahier des prix électricité 2026 de la SRM Souss-Massa — bordereau seul, prix HT, avec la consistance de chaque prix (pose, fourniture, fourniture et pose) : supports, armements, appareils de coupure, câbles BT et MT, postes et transformateurs. Prescription d’opérateur, « à vérifier ». Emplacement : 06_OPERATEURS.

# Version 0.8

REF-016 (VRD, avec des parties bâtiment pour la famille ELB) : cahier des charges fixant les spécifications techniques minimales des infrastructures de télécommunications des nouveaux lotissements et constructions, approuvé par l’arrêté conjoint n° 1114-25 du 29 avril 2025 (BO n° 7454 du 06/11/2025, version française). Texte obligatoire pour le lotisseur ; « à vérifier » tant que la copie reçue (version site web) n’est pas rapprochée du BO. Emplacement : 09_TEXTES_REGLEMENTAIRES (dossier ajouté en v0.9).

# Version 0.9

REF-017 (COMMUN) : règlement de construction parasismique RPS 2000, version 2011, approuvé par le décret n° 2-12-682 du 28 mai 2013 (BO n° 6206 du 21/11/2013). Obligatoire pour les bâtiments ; ne couvre ni les ouvrages enterrés ni les ouvrages d’art. Zonage de 21 communes de la province de Taroudant révisé en 2024 (décret n° 2-24-766, à obtenir). « À vérifier ». Emplacement : 09_TEXTES_REGLEMENTAIRES (édition du ministère et BO).

REF-018 (VRD) : PNM 13.1.220 (2018), tranchées : ouverture, remblayage, réfection — objectifs de densification q2 à q5 par zone de tranchée. Projet de norme IMANOR, remplace la NM 13.1.220 de 2008 : homologation à vérifier. Fichier en accès restreint (document IMANOR à usage du client). Emplacement : 05_NORMES.

REF-019 (COMMUN) : PNM EN 206 (IC 10.1.008, 2022), béton — spécification, performances, production et conformité. Projet de norme IMANOR, remplace la NM 10.1.008 de 2009 : homologation à vérifier. Fichier en accès restreint. Emplacement : 05_NORMES.

REF-020 (COMMUN) : règles de certification NM Ciments RCNM014, version 03 du 31/07/2020 (IMANOR). Permet d’exiger dans les CPS des ciments titulaires de la marque NM. Emplacement : 05_NORMES.

Le dossier 09_TEXTES_REGLEMENTAIRES est ajouté à l’arborescence du référentiel pour les lois, décrets et arrêtés ; REF-016 y est déplacé.

# Version 0.10

REF-021 (COMMUN) : règlement de passation des marchés de la SDL Agadir Souss Massa Aménagement, modifié par décision du conseil d’administration du 08/03/2024 (120 articles). Obligatoire pour ASMA ; « à vérifier » tant que la décision d’entrée en vigueur du président du CA (article 120) et les annexes 1 à 4 ne sont pas obtenues. Dispositions utiles au standard : mentions obligatoires du CPS (article 15), estimation du maître d’ouvrage, qui peut s’appuyer sur des référentiels de prix (article 5), prix révisables au-delà de 8 mois de délai (article 14), contrôle des offres et des prix unitaires principaux à ± 20 % de l’estimation (article 43), sous-traitance limitée à 50 % et hors corps d’état principal (article 106). Emplacement : 09_TEXTES_REGLEMENTAIRES.

# Reste à faire

- Désigner l’emplacement partagé et les droits de modification (étape 5), puis renommer le fichier selon la règle ASMA_Classeur_Referentiels_Prix_v[X.Y]_[AAAAMMJJ].xlsx.
- Faire valider le modèle par le chef de projet ; le statut « validé » des lignes reste réservé aux responsables désignés (action 0.8).
