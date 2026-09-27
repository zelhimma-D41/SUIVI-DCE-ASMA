# 1. Objectif final

Doter ASMA d'un référentiel DCE interne : pour chaque lot, un CPS type et un catalogue de prix paramétrés, que les bureaux d'études ne font que renseigner, puis une base de prix actualisée à partir des marchés adjugés.

À la fin du programme, ASMA dispose de :

1. **Un prompt standard v3** (noyau commun + paquet de variables par lot), versionné et figé.
2. **Un CPS type validé par famille**, anonyme, avec paramètres balisés {…}.
3. **Un classeur de référentiels et de prix** : une feuille de référentiels vérifiés, une feuille de prix par famille, sans montant dans la couche type.
4. **Une couche prix** alimentée par les BDDE adjugés, pour produire l'estimation confidentielle du maître d'ouvrage et contrôler les offres.
5. **Une gouvernance** : qui valide, à quel rythme, et comment on rouvre une entrée quand un texte change.

# 2. Point de départ (septembre 2026)

Les quatre prompts sont passés en v3 puis ont intégré la taxonomie v3 : un noyau commun identique (méthode, verrou juridique, phases, contrôles) et un paquet variable par famille. Ils restent au statut « projet » tant que la phase 0 n'est pas close.

| Élément | État | Ce qui manque |
| Prompts EVP v3.4, ECL v3.2, VRD v3.4, Bâtiment v3.2 | Rédigés, codes de la taxonomie v3 intégrés ; GMTR ajouté aux référentiels VRD et TER, transplantation intégrée au paquet EVP (24/09/2026) ; constats du CPS AOO 193/2025 intégrés aux paquets EVP et VRD (25/09/2026) | Validation par un juriste marchés et un ingénieur par famille |
| Taxonomie des corps d'état | v3 validée le 23/09/2026 : 107 lots, 13 familles, codes trigramme ; v3.1 du 24/09/2026 (transplantation dans EVP01, EVP03 et EVP04, codes inchangés) | Rien : codes reportés dans les paquets B2 |
| Référentiel juridique et normatif | Inexistant | Feuille Référentiels vérifiée (statut, source, date) |
| CPS sources et BDDE adjugés | Non rassemblés | 3 à 4 CPS et 3 à 4 BDDE par famille pilote |
| Décisions du guide (section 9) | 9 points ouverts | Arbitrage par la direction technique |

Le socle retenu est le prompt Espaces verts V2 corrigée, restructuré en noyau v3 commun et étendu aux trois autres familles.

# 3. Phase 0 — Préparer le pilote (environ 3 semaines)

La phase 0 fige les règles du jeu : on ne lance aucune génération tant que les décisions, la taxonomie et les sources ne sont pas prêtes.

```mermaid
flowchart LR
  P0[Phase 0] --> P1[Phase 1]
```

Le programme avance par portes : aucune phase ne démarre sans la validation de la précédente.

| N° | Action | Livrable | Porteur suggéré |
| 0.1 | Trancher les 9 points de décision du guide (défauts appliqués dans les paquets v3) | Note de décision signée | Direction technique |
| 0.2 | Faire relire le noyau v3 par un juriste marchés : régime propre d'ASMA, place du CCAG-T, variantes {REGIME_JURIDIQUE} | Noyau A-v3.0 validé | Service marchés |
| 0.3 | Obtenir le règlement des achats applicable à ASMA et le verser en donnée d'entrée | Document de référence | Service marchés |
| 0.4 | ✔ Fait le 23/09/2026 — taxonomie v3 validée (107 lots, 13 familles, codes trigramme) et codes reportés dans les paquets B2 | Taxonomie v3 validée, paquets à jour | Chef de projet |
| 0.5 | Créer le classeur cible : feuilles Référentiels, Paramètres, Prix par famille | Modèle Excel vide | Chef de projet |
| 0.6 | Constituer la feuille Référentiels de la famille EVP (B3) : vérifier chaque texte, statut et date | 20 à 40 entrées « vérifiées » | Ingénieur EV + juriste |
| 0.7 | Rassembler 3 à 4 CPS Espaces verts récents et 3 à 4 BDDE adjugés | Dossier sources pilote | Chef de projet |
| 0.8 | Désigner le validateur par famille et fixer la périodicité de revue | Liste nominative | Direction |

> Critère de sortie : noyau validé, codes lots EVP définitifs, sources rassemblées, référentiel EVP au moins partiellement vérifié.

# 4. Phase 1 — Pilote Espaces verts, de bout en bout (environ 6 à 8 semaines)

Le pilote EVP teste toute la chaîne sur de vrais documents ; c'est lui qui dit si le noyau et la taxonomie tiennent, avant toute réplication.

1. **Triage (phase 0 du prompt).** Lancer le prompt EVP-v3.4 avec les sources brutes. Valider le découpage proposé et le volume utile (seuils 100 / 250 pages).
2. **Diagnostic (phase 1 du prompt).** Recevoir l'inventaire, la matrice de couverture, le registre des contradictions et les fiches de décision FD-nn.
3. **Arbitrage.** Réunion de décision : chaque fiche reçoit une décision datée et signée. Valider aussi la liste des paramètres {…} et leurs valeurs admissibles.
4. **Production (phase 2 du prompt).** Générer le CPS type EVP, la bibliothèque de prix EVP et la note de synthèse, lot par lot si nécessaire.
5. **Contrôle.** Appliquer la grille C1 à C12 ; relecture technique par l'ingénieur EV, relecture juridique du Chapitre 1.
6. **Confrontation aux BDDE adjugés.** Pour chaque BDDE : taux de lignes retrouvées dans la bibliothèque, lignes manquantes, lignes jamais utilisées.
7. **Test métier.** Demander à un BET de produire un DCE fictif en ne modifiant que les paramètres. Noter chaque endroit où il a dû réécrire un texte.
8. **Corrections à la racine.** Tout défaut récurrent est corrigé dans le noyau, le paquet ou la taxonomie (nouvelle version), pas seulement dans le livrable.

Critères de validation du pilote :

- 100 % des prix sources expliqués (contrôle C2) ;
- au moins 90 % des lignes des BDDE adjugés retrouvées dans la bibliothèque ;
- aucune référence « à vérifier » affirmée dans le CPS type ;
- test métier réussi : le BET n'a réécrit aucun descriptif ;
- CPS type et bibliothèque EVP passés au statut « validé », version V1.0.

# 5. Phase 2 — Réplication aux autres familles (4 à 6 semaines par famille)

Chaque famille rejoue exactement le protocole du pilote, avec le noyau tel que corrigé par le pilote. On n'avance qu'une ou deux familles à la fois.

| Ordre | Famille | Prompt | Point d'attention |
| 1 | VRD — Voirie et réseaux divers | Prompt_CPS_Type_VRD_v3.4 | Interface eau d'irrigation avec EVP (point de livraison) et génie civil avec ECL |
| 2 | ECL — Éclairage public et vidéoprotection | Prompt_CPS_Type_Eclairage_Public_v3.2 | Vérifier le texte réellement applicable (« RGIE » douteux), loi 09-08 pour la vidéo |
| 3 | TER à ELB — Bâtiment | Prompt_CPS_Type_Batiment_v3.2 | Exécuter famille par famille ({FAMILLES_TRAITEES}), une feuille de prix par famille |
| 4 | Autres familles (PRE, OAH, AUS, EQS) | Nouveau paquet B à rédiger sur le modèle des quatre existants | Ordre fixé selon les besoins réels des projets ASMA |

L'ordre proposé est à ajuster selon la priorité opérationnelle d'ASMA. Pour chaque famille :

- ☐ Paquet B mis à jour (codes lots, référentiels vérifiés, décisions)
- ☐ Sources et BDDE rassemblés
- ☐ Phases 0, 1 et 2 du prompt exécutées, fiches de décision signées
- ☐ Contrôles C1 à C12 et confrontation aux BDDE
- ☐ Test métier par un BET
- ☐ Passage au statut « validé » (V1.0)

Dès qu'une interface change (par exemple la limite eau EVP/VRD), les deux paquets concernés sont mis à jour ensemble.

# 6. Phase 3 — Base de prix et actualisation automatique

La phase 3 ne démarre qu'avec au moins deux familles validées. Elle ajoute les montants dans une couche séparée, sans jamais toucher la bibliothèque type.

1. **Structurer la couche prix.** Une table « observations » : code prix unifié, valeurs des paramètres, prix unitaire adjugé, date d'adjudication, zone, taille du marché, rang de l'offre (attributaire ou non).
2. **Saisir l'historique.** Rattacher chaque ligne des BDDE adjugés d'ASMA à un code prix (le mapping est déjà amorcé par la confrontation des phases 1 et 2).
3. **Calculer les prix de référence.** Par code prix et combinaison de paramètres : médiane, fourchette basse et haute, nombre d'observations, ancienneté. Un prix fondé sur moins de 3 observations est signalé « peu fiable ».
4. **Actualiser.** À chaque nouvelle adjudication, ajouter les lignes ; appliquer si besoin un index de révision pour ramener les prix anciens à date.
5. **Exploiter.** Générer l'estimation confidentielle d'un nouveau DCE à partir des quantités et des paramètres choisis ; repérer les offres anormalement basses ou excessives.
6. **Outiller.** Commencer dans Excel ; passer à un outil (base de données, application interne) seulement quand le volume le justifie.

> Critère de réussite : sur un marché test, l'estimation générée reste dans un écart jugé acceptable par la direction par rapport à l'offre attributaire (seuil à fixer).

# 7. Gouvernance, rôles et indicateurs

Chaque entrée du standard suit le cycle brouillon → vérifié → validé, et seul un responsable désigné peut valider.

| Rôle | Responsabilités |
| Sponsor (direction) | Tranche les points de décision, valide les portes de phase |
| Chef de projet standardisation | Pilote le planning, tient les versions du noyau, des paquets et du classeur |
| Référent juridique marchés | Verrou juridique, Chapitre 1, statut des textes du référentiel |
| Référent technique par famille | Fiches de décision techniques, relecture du Chapitre 3, validation des prix |
| BET testeur | Test métier : produire un DCE en ne modifiant que les paramètres |

Règles de version : noyau figé et numéroté (A-v3.0, A-v3.1…), modifié pour toutes les familles à la fois ; référentiel vivant, rouvert à chaque évolution d'un texte ; revue complète au moins une fois par an.

| Indicateur | Cible |
| Prix sources expliqués (C2) | 100 % |
| Couverture des BDDE adjugés | ≥ 90 % des lignes |
| Références « vérifiées » dans le CPS type | 100 % de celles affirmées |
| Textes réécrits par le BET lors du test métier | 0 |
| Familles validées | 2 avant la phase 3, puis selon le plan |

# 8. Risques et parades

| Risque | Parade |
| Références normatives inventées ou obsolètes produites par l'IA | Registre de vérification ; seules les entrées « vérifiées » sont affirmées ; revue juridique |
| Régime juridique d'ASMA mal qualifié (CCAG-T appliqué d'office) | Verrou juridique du noyau et règlement des achats d'ASMA en donnée d'entrée |
| Volume des CPS sources trop important pour une génération | Triage, seuils de volume utile, production lot par lot, mode incrémental |
| Arbitrages bloqués faute de décideur | Validateur nommé par famille ; décision par défaut = option recommandée, tracée et révisable |
| Recouvrements entre familles (eau EVP/VRD, génie civil ECL/VRD, VRD dans le Bâtiment) | Interfaces explicites dans chaque paquet ; mise à jour conjointe des paquets concernés |
| BET qui contournent le standard en réécrivant les textes | Test métier, clause d'usage obligatoire dans les contrats de BET, contrôle à la remise du DCE |
| Base de prix fondée sur trop peu d'observations | Seuil minimal de 3 observations et indicateur de fiabilité par prix |
