# Classeur des référentiels et de la bibliothèque de prix type — modèle v0.19

Action 0.5 de la phase 0 — version 0.15 du 27/09/2026. Fichier : ASMA_Classeur_Referentiels_Prix_v0.15_20260927.xlsx.

Ce classeur est le fichier cible du standard : il reçoit, famille par famille, la feuille Référentiels, le dictionnaire des Paramètres et la bibliothèque de prix type produits par les prompts v3 (Fichier 3, section 12.3 du noyau). Sa structure est identique pour les 13 familles de la taxonomie v3. Il ne contient aucun montant, aucune quantité et aucune source nommée.

# Feuilles

| Feuille | Contenu | Qui saisit |
| Lisez-moi | Mode d’emploi, règles et historique des versions | Chef de projet |
| Tableau de bord | Contrôles automatiques par famille : lots couverts, lignes par statut, codes non conformes, doublons ; état des référentiels | Formules, aucune saisie |
| Taxonomie | Les 106 lots de la taxonomie v3.2 (validée le 23/09/2026, contenus EVP précisés le 24/09/2026, lot VRD13 fusionné dans VRD02 le 27/09/2026) | Verrouillée |
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

# Version 0.11

Feuille Taxonomie en v3.2 : le lot VRD13 « Couche de forme et traitement des sols » est fusionné dans VRD02, renommé « Remblais, plateformes de voirie et couche de forme » (décision I-8 du 27/09/2026). Le code VRD13 reste vacant ; les codes VRD14 à VRD19 sont inchangés. Total : 106 lots, dont 18 en VRD.

# Version 0.12

REF-022 (VRD) : arrêté conjoint n° 3106-19 du 10 octobre 2019 (BO n° 6832 du 21/11/2019) modifiant l’arrêté n° 2805-14 du 1er août 2014 relatif à la signalisation routière et promulguant l’instruction générale de la signalisation routière. Obligatoire sur toute voie ouverte à la circulation publique ; signaux non conformes tolérés au plus dix ans. Arrêté de base n° 2805-14 à obtenir. Emplacement : 09_TEXTES_REGLEMENTAIRES (BO et note de la DGRTT).

| Code | Partie de l’instruction générale sur la signalisation routière (2019) | Lots |
| REF-023 | 1 — Généralités : homologation, gammes de panneaux, supports, implantation, rétroréflexion | VRD08, VRD09, VRD15 |
| REF-024 | 2 — Signalisation de danger | VRD09 |
| REF-025 | 3 — Intersections et régimes de priorité | VRD08, VRD09 |
| REF-026 | 4 — Signalisation de prescription | VRD09 |
| REF-027 | 5 — Signalisation d’indication, des services et de repérage | VRD09 |
| REF-028 | 6 — Signalisation lumineuse (famille ECL) | ECL11 |
| REF-029 | 7 — Marques sur chaussées : largeurs, modulations, rétroréflexion, produits homologués | VRD08, VRD15 |
| REF-030 | 8 — Signalisation temporaire (chantiers) | VRD09, chapitre 2 du CPS type |

Type « Instruction », obligatoire, « à vérifier » (origine des fichiers à confirmer). Emplacement : 07_SIGNALISATION_ACCESSIBILITE.

REF-031 (VRD) : NM 13.1.214 (2008), bétons bitumineux semi-grenus (BBSG 0/10 et 0/14, classes 1 à 3, épaisseurs 5 à 7 cm et 6 à 9 cm). Probablement remplacée : le catalogue 2023 donne ce numéro à une édition 2019 sur les enrobés à froid ; les enrobés à chaud relèvent de la NM 13.1.213 (2019) et de la série NM EN 13108 (2018). Ne pas citer au CPS type avant confirmation. Emplacement : 05_NORMES.

REF-032 (COMMUN) : liste des réglementations techniques et des normes marocaines d’application obligatoire, mise à jour du 08/04/2024. Utile à la VRD : armatures, ciments, bétons, bitumes routiers, canalisations PVC et PE ; à l’éclairage : candélabres, luminaires, câbles. Emplacement : 05_NORMES.

REF-033 (COMMUN) : catalogue des normes marocaines 2023 de l’IMANOR (16 526 normes), converti en PDF. Sert à vérifier le numéro, l’intitulé et l’édition de chaque NM. Emplacement : 05_NORMES.

Feuille Listes : types « Instruction » et « Catalogue ou liste » ajoutés.

# Version 0.13

REF-034 (VRD) : PNM 13.1.230 (2019), installations de fabrication d’enrobés bitumineux à chaud en mode discontinu (équipements, réglages initiaux). Projet de norme IMANOR ; une NM 13.1.230 homologuée en 2020 figure au catalogue : édition définitive à obtenir. Fichier en accès restreint (document IMANOR à usage du client). Emplacement : 05_NORMES.

REF-035 (ECL) : cahier des prescriptions spéciales SRM-SM des travaux d’électrification des lotissements et ensembles immobiliers (SRM SM-CPS-S08-01, version 01 du 10/06/2026). Prescriptions de l’opérateur pour les câbles HTA et BT, les tranchées et traversées, les postes HTA/BT, les coffrets, la mise à la terre et les dossiers à fournir. Fichier en accès restreint (document marqué « accessibilité restreinte », avec noms et signatures). Emplacement : 06_OPERATEURS.

REF-031 : le catalogue IMANOR du secteur BTP confirme que la NM 13.1.214 : 2019 porte sur les enrobés à froid ; la NM 13.1.214 : 2008 (BBSG) ne doit pas être citée au CPS type.

# Version 0.14

REF-036 (COMMUN) : guide promoteurs de la SRM-SM, édition 2026 (eau potable, assainissement, électricité) : instruction des projets, devis d’équipement, réalisation des travaux, réception technique, provisoire et définitive (garantie d’un an). Guide indicatif, non contractuel ; renvoie au CPS et au CPC de l’opérateur. Emplacement : 06_OPERATEURS.

REF-037 (COMMUN) : règles de certification NM des éléments de regards de visite et boîtes de branchement en béton RCNM025, version 02 du 17/01/2024 (IMANOR), avec la liste des normes applicables (NM EN 1917 et normes des constituants). Emplacement : 05_NORMES.

# Version 0.15

REF-038 (VRD) : arrêté conjoint n° 2306-17 du 5 décembre 2017 (BO n° 6652 du 01/03/2018) fixant les spécificités techniques des accessibilités en matière d’urbanisme : cheminements de 1,50 m libres, dévers ≤ 2 %, ressauts ≤ 2 cm, bandes d’éveil de vigilance, bateaux de 1,50 m à pente < 5 %, places de stationnement réservées de 3,30 m. Obligatoire. Emplacement : 07_SIGNALISATION_ACCESSIBILITE.

REF-039 (COMMUN) : arrêté conjoint n° 3146-18 du 28 février 2019 (BO n° 6820, édition arabe) fixant les spécificités techniques des accessibilités architecturales. Obligatoire ; familles du bâtiment surtout. Emplacement : 07_SIGNALISATION_ACCESSIBILITE.

REF-040 (VRD) : PNM 13.1.213 (2019), exécution des enrobés hydrocarbonés à chaud (assises, liaison, roulement), remplaçant pour l’exécution la NM 13.1.214 : 2008. Accès restreint. Emplacement : 05_NORMES.

REF-041 (VRD) : NM 13.1.220 (2008), tranchées, édition homologuée en vigueur (le projet de 2018 reste REF-018). Exemplaire sous licence d’utilisateur unique : accès restreint, licence ASMA à acquérir. Emplacement : 05_NORMES.

# Version 0.16

REF-042 (COMMUN) : décret n° 2-11-246 du 30 septembre 2011 (BO n° 5988 du 20/10/2011) portant application de la loi n° 10-03 relative aux accessibilités : trottoirs de 1,50 m à 2,00 m, bateaux en plan incliné < 5 %, une place de stationnement réservée sur vingt, passages des bâtiments de 2,00 m à 12 % maximum, arrêts de transport accessibles ; base des arrêtés REF-038 et REF-039. Obligatoire. Emplacement : 09_TEXTES_REGLEMENTAIRES. Note de REF-038 mise à jour.

# Version 0.17

REF-043 (COMMUN) : loi n° 10-03 relative aux accessibilités (dahir n° 1-03-58 du 12/05/2003, BO n° 5118 du 19/06/2003) : loi-cadre dont REF-042, REF-038 et REF-039 sont les textes d’application ; feux sonores aux traversées des artères principales (art. 20). Obligatoire. Emplacement : 09_TEXTES_REGLEMENTAIRES (extrait de 4 pages du BO).

REF-044 (COMMUN) : catalogue des normes marocaines du secteur BTP du ministère de l’Équipement (2022, 2 449 normes dont 41 d’application obligatoire). Confirme NM 13.1.213 : 2019, le remplacement de REF-031 et l’édition 2008 de la NM 13.1.220 ; REF-033 prime en cas d’écart. Emplacement : 05_NORMES.

# Version 0.18

REF-045 (VRD) : NM 10.9.001 (1990), dispositifs de couronnement et de fermeture des ouvrages d’assainissement et de distribution d’eau utilisés en voirie : classes A 15 à F 900 et choix selon le lieu (B 125 trottoir, C 250 caniveau, D 400 chaussée), matériaux, emboîtement, masse surfacique, essais et marquage. Homologuée par l’arrêté n° 353.90 (BO n° 4071 du 07/11/1990). Référence nationale à citer à la place de la NM EN 124. Emplacement : 05_NORMES.

REF-046 (VRD) : NM 10.1.027, projet de révision du 03/01/2021, canalisations en béton armé et non armé : séries 60 A, 90 A, 135 A, 60 B, 90 B, joints et abouts, armatures, essais. À rapprocher de l’édition homologuée 2021 avant citation. Emplacement : 05_NORMES.

REF-047 (VRD) : liste des méthodes appliquées à la Direction Contrôle qualité des eaux de l’ONEE (version 03 du 12/08/2024) : essais et normes d’analyse de l’eau, statut d’accréditation. Utile aux prescriptions d’essais de réception (V18). Emplacement : 06_OPERATEURS.

REF-048 (COMMUN) : politique qualité et engagement de la direction du Contrôle qualité des eaux de l’ONEE (version 04 du 30/03/2026). Noms et signatures : accès restreint. Emplacement : 06_OPERATEURS.

# Version 0.19

REF-049 (VRD) : CCTG des travaux d’assainissement liquide urbain de l’ONEE — Branche Eau, tome 2 « Terrassements », version 2 de février 2013 : déblais, matériaux de remblai classés selon le GMTR, remblais de tranchée à 95 % de l’OPM par couches de 20 cm, lit de pose en sable 0/10, enrobage, fouilles, étanchéité des bassins. Emplacement : 06_OPERATEURS.

REF-050 (VRD) : CCTG ONEE — Branche Eau, tome 3 « Canalisations et ouvrages annexes », version 2 de février 2013 : produits (béton, PVC-U, fonte ductile, PEHD et PP à parois structurées, PRV), regards, couronnement et fermeture, branchements, pose, contrôles et épreuves d’étanchéité selon l’EN 1610 avec valeurs d’eau d’appoint admissibles. Couvre la partie « essais » manquante de la ligne V18. Emplacement : 06_OPERATEURS.

REF-051 (VRD) : PNM 13.1.023 : 2019, essais Proctor normal et modifié (remplace la NM 13.1.119). Accès restreint. Emplacement : 05_NORMES.

REF-052 (VRD) : PNM 30.8.111 : 2020, gestion d’un réseau d’assainissement (lignes directrices de service). Accès restreint. Emplacement : 05_NORMES.

REF-053 et REF-054 (VRD) : PNM EN 13508-1 et EN 13508-2 : 2020, investigation et évaluation des réseaux — exigences générales et système de codage de l’inspection visuelle. Accès restreint (reproduction CEN). Emplacement : 05_NORMES.

Le fichier 13.1.220 reçu le même jour est identique à REF-018 : aucun nouveau code.

# Reste à faire

- Désigner l’emplacement partagé et les droits de modification (étape 5), puis renommer le fichier selon la règle ASMA_Classeur_Referentiels_Prix_v[X.Y]_[AAAAMMJJ].xlsx.
- Faire valider le modèle par le chef de projet ; le statut « validé » des lignes reste réservé aux responsables désignés (action 0.8).
