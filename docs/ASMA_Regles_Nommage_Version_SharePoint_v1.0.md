# 1. Objet

Cette fiche fixe la règle de nommage, la règle de version, l'emplacement SharePoint et les droits du classeur des référentiels et des prix, ainsi que des autres livrables du standard DCE (étape 5 de l'action 0.5). Elle est proposée par le chef de projet et validée par la direction. Les noms des personnes qui reçoivent des droits sont ceux de la fiche de l'action 0.8.

# 2. Emplacement SharePoint

Un site SharePoint dédié, « Standardisation DCE ASMA » (site d'équipe, éventuellement relié à une équipe Teams), contient une bibliothèque de documents « Standard DCE » organisée ainsi :

| Dossier | Contenu | Remarque |
| 01_CLASSEUR | Classeur des référentiels et des prix, version en vigueur seule | Extraction obligatoire |
| 02_PROMPTS | Noyau et paquets par famille, version en vigueur | Un fichier par famille |
| 03_REFERENTIEL_TECHNIQUE | Fichiers de référence REF-nnn, dossiers 00_INDEX à 09_TEXTES_REGLEMENTAIRES | Chemin repris dans la colonne « Emplacement du fichier » |
| 04_SOURCES_RESTREINT | CPS nominatifs, BDDE adjugés, classeur confidentiel des BDDE, normes IMANOR à usage du client | Héritage des autorisations rompu |
| 05_PILOTAGE | Fiches d'actions, relevés de décisions, listes de collecte, procès-verbaux | Modifiable par les référents |
| _ARCHIVE | Versions remplacées, rangées par type de document | Lecture seule pour tous |

Le lien vers la bibliothèque est noté dans la note de l'action 0.5 de l'outil de suivi. Le partage avec des personnes extérieures à ASMA est désactivé sur le site ; un bureau d'études testeur reçoit un fichier précis, jamais l'accès à la bibliothèque.

# 3. Droits d'accès

Les droits sont donnés par groupe SharePoint, jamais par personne isolée.

| Groupe SharePoint | Membres | Droits |
| Propriétaires | Chef de projet (titulaire et suppléant) | Contrôle total ; seuls à déposer une nouvelle version dans 01_CLASSEUR et 02_PROMPTS |
| Membres | Référents techniques et juridique désignés à l'action 0.8 | Modification dans 05_PILOTAGE ; lecture et commentaires ailleurs |
| Visiteurs | Services techniques et marchés, direction | Lecture seule |
| Accès restreint | Direction, chef de projet, référent juridique | Seuls à voir 04_SOURCES_RESTREINT |

Les référents proposent leurs corrections du classeur par commentaire dans le fichier ou sur une copie de travail déposée dans 05_PILOTAGE ; le chef de projet les intègre dans une nouvelle version.

# 4. Règle de nommage

- Classeur : ASMA_Classeur_Referentiels_Prix_vX.Y_AAAAMMJJ.xlsx (exemple : ASMA_Classeur_Referentiels_Prix_v0.11_20260927.xlsx).
- Autres livrables : ASMA_[Objet]_[Famille]_vX.Y_AAAAMMJJ.ext (exemple : ASMA_Prompt_CPS_Type_VRD_v3.5_20260927.docx).
- Fichiers de référence : REF-nnn_[sigle]_[partie]_[édition]_[officiel ou copie].pdf (exemple : REF-017_RPS2000_Reglement_v2011_copie.pdf).
- Ni accents, ni espaces, ni caractères spéciaux ; la date est celle de la version, pas celle du dépôt.

# 5. Règle de version

- **Versions 0.x** jusqu'à la validation du pilote Espaces verts ; **1.0** est la première version validée, à la sortie de la phase 1.
- **Y augmente** (0.10 → 0.11) à chaque ajout ou modification de contenu : lignes Référentiels, Paramètres ou Prix.
- **X augmente** (0.x → 1.0, 1.x → 2.0) à chaque changement de structure (colonnes, feuilles, refonte de la taxonomie) ou à chaque validation formelle.
- Chaque version reçoit une ligne dans le tableau des versions de la feuille Lisez-moi : numéro, date, auteur, changements.
- Une seule version en vigueur dans 01_CLASSEUR : à chaque nouvelle version, l'ancienne est déplacée dans _ARCHIVE. Aucun fichier n'est écrasé.
- L'historique des versions de SharePoint reste activé : il conserve les enregistrements intermédiaires entre deux versions numérotées, mais il ne remplace pas le numéro de version.
- Chaque ligne du classeur suit le cycle brouillon → vérifié → validé ; seuls les responsables désignés à l'action 0.8 passent une ligne à « validé ».

# 6. Paramétrage SharePoint à faire

1. Créer le site « Standardisation DCE ASMA » et la bibliothèque « Standard DCE » avec les six dossiers.
2. Activer l'historique des versions principales (50 versions au moins) sur la bibliothèque.
3. Exiger l'extraction des fichiers dans 01_CLASSEUR, pour éviter deux modifications simultanées du classeur.
4. Créer les groupes Propriétaires, Membres, Visiteurs et Accès restreint, et y placer les personnes de la fiche 0.8.
5. Rompre l'héritage des autorisations sur 04_SOURCES_RESTREINT (groupe Accès restreint seulement) et sur _ARCHIVE (lecture seule pour tous).
6. Désactiver le partage externe du site.
7. Déposer le classeur v0.11 dans 01_CLASSEUR et les fichiers REF-nnn dans 03_REFERENTIEL_TECHNIQUE.
8. Noter le lien de la bibliothèque dans l'action 0.5 de l'outil de suivi, puis cocher l'étape 5.

# 7. Validation

| Rubrique | Valeur |
| Proposé par | Chef de projet standardisation — date et visa : ………… |
| Validé par | Direction — date, nom et visa : ………… |
| Paramétrage réalisé par | Administrateur SharePoint — date : ………… |
