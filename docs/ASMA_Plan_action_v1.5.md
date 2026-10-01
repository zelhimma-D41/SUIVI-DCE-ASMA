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

# 3. Objectif daté : le 31 décembre 2026

Avec l'équipe initiale et les familles traitées l'une après l'autre, le Bâtiment n'est validé qu'entre le 17 février et le 14 avril 2027. Le scénario retenu est celui de l'équipe renforcée : **au 31 décembre 2026, les quatre familles Espaces verts, VRD, Éclairage public et Bâtiment sont validées et la base de prix est lancée.** Les autres familles (OAH, AUS, EQS, PRE…) passent au premier trimestre 2027.

Trois leviers permettent de tenir cette date :

1. **La phase 2 se déroule en quatre flux simultanés** (VRD, ECL, Bâtiment gros œuvre et second œuvre, Bâtiment lots techniques) au lieu d'une famille après l'autre.
2. **Les durées sont prises au bas de la fourchette** : 3 semaines pour la phase 0, 6 semaines pour le pilote, 4 semaines par famille.
3. **Un jalon « noyau stabilisé » est placé à la quatrième semaine du pilote.** Il ne clôt pas le pilote : il autorise le lancement anticipé de la VRD sans attendre sa validation. Règle associée : toute correction du noyau issue de la fin du pilote est reportée sur la VRD en cours.

| Date | Jalon | Ce qui se passe |
| 14/10/2026 | Phase 0 close | Actions 0.1, 0.3, 0.7 et 0.8 menées en parallèle ; l'action 0.1 (arbitrage des 9 points) est le chemin critique |
| 11/11/2026 | Noyau stabilisé | Quatrième semaine du pilote EVP : le noyau ne bouge plus sauf correction majeure ; la VRD est lancée |
| mi-novembre 2026 | Renfort en place | Chef de projet adjoint et rédacteurs-analystes recrutés ou affectés, et formés au noyau |
| 25/11/2026 | Pilote EVP validé | CPS type et bibliothèque EVP en V1.0 ; l'Éclairage public et le Bâtiment sont lancés |
| 09/12/2026 | VRD validée | CPS type et bibliothèque VRD en V1.0 |
| mi-décembre 2026 | Base de prix lancée | La phase 3 démarre avec les deux familles validées (EVP et VRD) |
| 23/12/2026 | ECL et Bâtiment validés | Les quatre familles sont en V1.0 |
| 31/12/2026 | Objectif tenu | Une semaine de marge sépare le 23/12 de l'objectif |

La marge est d'une seule semaine : tout glissement de l'action 0.1 ou de l'arrivée du renfort se répercute directement sur la date de fin.

# 4. Phase 0 — Préparer le pilote (3 semaines, close le 14/10/2026)

La phase 0 fige les règles du jeu : on ne lance aucune génération tant que les décisions, la taxonomie et les sources ne sont pas prêtes. Pour tenir le 14 octobre, les actions 0.1, 0.3, 0.7 et 0.8 sont menées en parallèle : l'action 0.1 est le chemin critique, les autres n'attendent pas son résultat.

@@FLOW@@

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

# 5. Phase 1 — Pilote Espaces verts, de bout en bout (6 semaines, validé le 25/11/2026)

Le pilote EVP teste toute la chaîne sur de vrais documents ; c'est lui qui dit si le noyau et la taxonomie tiennent, avant toute réplication.

À la quatrième semaine (11/11/2026), le pilote passe le jalon **noyau stabilisé** : les corrections de fond du noyau sont faites, seuls des ajustements de détail restent possibles. La VRD est lancée à cette date, sans attendre la validation finale du pilote. Si une correction majeure du noyau apparaît ensuite, elle est reportée sur la VRD en cours et le chef de projet mesure l'impact sur le 09/12.

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

# 6. Phase 2 — Réplication en quatre flux parallèles (4 semaines par famille)

Chaque famille rejoue le protocole du pilote avec le noyau stabilisé. Pour tenir le 31 décembre, les familles ne sont plus traitées l'une après l'autre : quatre flux avancent en parallèle, chacun conduit par un rédacteur-analyste et suivi par le chef de projet adjoint.

| Flux | Famille ou périmètre | Lancement et validation | Point d'attention |
| 1 | VRD — Voirie et réseaux divers | Lancée le 11/11/2026 (jalon noyau stabilisé), validée le 09/12/2026 | Interface eau d'irrigation avec EVP (point de livraison) et génie civil avec ECL ; reprise possible si le pilote corrige le noyau après le 11/11 |
| 2 | ECL — Éclairage public et vidéoprotection | Lancée le 25/11/2026, validée le 23/12/2026 | Texte électrique réellement applicable, loi 09-08 pour la vidéoprotection, interface génie civil avec la VRD |
| 3 | Bâtiment — gros œuvre et second œuvre (TER, GOS, ENV, SOF) | Lancé le 25/11/2026, validé le 23/12/2026 | Une feuille de prix par famille ; cohérence avec le flux 4 sur les interfaces |
| 4 | Bâtiment — lots techniques (FLU, ELB) | Lancé le 25/11/2026, validé le 23/12/2026 | Interfaces avec le flux 3 (réservations, attentes) et avec l'ECL pour les tableaux et comptages |
| — | Autres familles (PRE, OAH, AUS, EQS) | 1er trimestre 2027 | Nouveau paquet B à rédiger sur le modèle des quatre existants |

**Gel du noyau pendant la phase 2.** Tant que les quatre flux tournent, le noyau est figé : une seule personne est habilitée à le modifier, le chef de projet ou son adjoint. Toute demande de correction passe par le point hebdomadaire, est tranchée en séance et, si elle est retenue, appliquée à tous les flux en même temps, avec une nouvelle version numérotée. C'est la parade à la divergence du noyau entre flux.

Pour chaque famille :

- ☐ Paquet B mis à jour (codes lots, référentiels vérifiés, décisions)
- ☐ Sources et BDDE rassemblés
- ☐ Phases 0, 1 et 2 du prompt exécutées, fiches de décision signées
- ☐ Contrôles C1 à C12 et confrontation aux BDDE
- ☐ Test métier par un BET, réservé dès octobre
- ☐ Passage au statut « validé » (V1.0)

Dès qu'une interface change (par exemple la limite eau EVP/VRD), les paquets concernés sont mis à jour ensemble, dans tous les flux touchés.

# 7. Phase 3 — Base de prix et actualisation automatique

La phase 3 démarre dès que les Espaces verts et la VRD sont validés, soit la mi-décembre 2026, sans attendre l'Éclairage public ni le Bâtiment. Elle est conduite par le responsable base de prix et BDDE, qui rassemble les BDDE adjugés des trois familles dès octobre. Elle ajoute les montants dans une couche séparée, sans jamais toucher la bibliothèque type.

1. **Structurer la couche prix.** Une table « observations » : code prix unifié, valeurs des paramètres, prix unitaire adjugé, date d'adjudication, zone, taille du marché, rang de l'offre (attributaire ou non).
2. **Saisir l'historique.** Rattacher chaque ligne des BDDE adjugés d'ASMA à un code prix (le mapping est déjà amorcé par la confrontation des phases 1 et 2).
3. **Calculer les prix de référence.** Par code prix et combinaison de paramètres : médiane, fourchette basse et haute, nombre d'observations, ancienneté. Un prix fondé sur moins de 3 observations est signalé « peu fiable ».
4. **Actualiser.** À chaque nouvelle adjudication, ajouter les lignes ; appliquer si besoin un index de révision pour ramener les prix anciens à date.
5. **Exploiter.** Générer l'estimation confidentielle d'un nouveau DCE à partir des quantités et des paramètres choisis ; repérer les offres anormalement basses ou excessives.
6. **Outiller.** Commencer dans Excel ; passer à un outil (base de données, application interne) seulement quand le volume le justifie.

> Critère de réussite : sur un marché test, l'estimation générée reste dans un écart jugé acceptable par la direction par rapport à l'offre attributaire (seuil à fixer).

# 8. Gouvernance, rôles et indicateurs

Chaque entrée du standard suit le cycle brouillon → vérifié → validé, et seul un responsable désigné peut valider.

| Rôle | Responsabilités |
| Sponsor (direction) | Tranche les points de décision, valide les portes de phase |
| Chef de projet standardisation | Pilote le planning, tient les versions du noyau, des paquets et du classeur |
| Référent juridique marchés | Verrou juridique, Chapitre 1, statut des textes du référentiel |
| Référent technique par famille | Fiches de décision techniques, relecture du Chapitre 3, validation des prix |
| Chef de projet adjoint | Coordonne les quatre flux de la phase 2, tient la cohérence du noyau entre flux, anime le point hebdomadaire |
| Rédacteur-analyste par famille | Conduit un flux de bout en bout : triage, diagnostic, production, contrôles C1 à C12 |
| Responsable base de prix et BDDE | Rassemble les BDDE adjugés, tient la couche prix, produit les estimations confidentielles |
| BET testeur (priorité A) | Test métier : produire un DCE en ne modifiant que les paramètres ; réservé dès octobre pour chaque famille |

Règles de version : noyau figé et numéroté (A-v3.0, A-v3.1…), modifié pour toutes les familles à la fois ; référentiel vivant, rouvert à chaque évolution d'un texte ; revue complète au moins une fois par an.

Le Bâtiment est scindé en deux binômes, gros œuvre et second œuvre d'une part, lots techniques d'autre part, chacun avec son rédacteur-analyste et son référent technique. Le juriste marchés est renforcé ou, à défaut, des créneaux de relecture lui sont réservés en décembre, au moment où les quatre familles arrivent ensemble à la validation.

Pendant les phases 1 et 2, un **point de suivi hebdomadaire** réunit le chef de projet, son adjoint et les rédacteurs-analystes : avancement de chaque flux, demandes de correction du noyau, entrées en attente de validation, marge restante avant le 31 décembre.

| Indicateur | Cible |
| Prix sources expliqués (C2) | 100 % |
| Couverture des BDDE adjugés | ≥ 90 % des lignes |
| Références « vérifiées » dans le CPS type | 100 % de celles affirmées |
| Textes réécrits par le BET lors du test métier | 0 |
| Familles validées | 2 avant la phase 3 (EVP et VRD, mi-décembre), 4 au 31/12/2026 |
| Avancement par flux | Chaque flux suivi séparément (et non plus la seule phase en cours) |
| Charge de validation | Entrées en attente par validateur ; alerte au-delà du volume traitable en une semaine |
| Marge restante avant le 31/12 | ≥ 1 semaine ; en deçà, arbitrage du sponsor sur le périmètre |

# 9. Risques et parades

| Risque | Parade |
| Références normatives inventées ou obsolètes produites par l'IA | Registre de vérification ; seules les entrées « vérifiées » sont affirmées ; revue juridique |
| Régime juridique d'ASMA mal qualifié (CCAG-T appliqué d'office) | Verrou juridique du noyau et règlement des achats d'ASMA en donnée d'entrée |
| Volume des CPS sources trop important pour une génération | Triage, seuils de volume utile, production lot par lot, mode incrémental |
| Arbitrages bloqués faute de décideur | Validateur nommé par famille ; décision par défaut = option recommandée, tracée et révisable |
| Recouvrements entre familles (eau EVP/VRD, génie civil ECL/VRD, VRD dans le Bâtiment) | Interfaces explicites dans chaque paquet ; mise à jour conjointe des paquets concernés |
| BET qui contournent le standard en réécrivant les textes | Test métier, clause d'usage obligatoire dans les contrats de BET, contrôle à la remise du DCE |
| Base de prix fondée sur trop peu d'observations | Seuil minimal de 3 observations et indicateur de fiabilité par prix |
| Validation en goulot en décembre : quatre familles arrivent ensemble chez les mêmes validateurs | Créneaux de relecture réservés dès novembre ; indicateur de charge de validation ; validation par lots plutôt qu'en un bloc |
| Divergence du noyau entre les quatre flux parallèles | Gel du noyau en phase 2 : une seule personne habilitée à le modifier, corrections appliquées à tous les flux en même temps, version numérotée |
| Renfort arrivé en retard : 1 à 2 semaines avant d'être productif | Recrutement ou affectation engagés dès octobre ; formation au noyau pendant le pilote ; à défaut, report d'un flux Bâtiment au 1er trimestre 2027 |
| Fin d'année : jours fériés et clôture budgétaire réduisent la disponibilité | Validations calées avant le 23/12 ; marge d'une semaine réservée ; aucune porte de phase planifiée entre le 24/12 et le 31/12 |
| Le pilote remet le noyau en cause après le lancement de la VRD | Jalon « noyau stabilisé » exigeant ; toute correction ultérieure est reportée sur la VRD en cours et son impact sur le 09/12 est mesuré au point hebdomadaire |
