# Étape 3 — Tirage au sort

## Objectif

Constituer le MiniPublic par un tirage au sort structuré, transparent et documenté — sur la base des candidatures reçues lors de la mobilisation et des critères de stratification définis lors du cadrage. Le tirage au sort est un moment fondateur : il ancre la légitimité du MiniPublic et marque publiquement le début du processus.

## Principes directeurs

**Le tirage au sort est un acte politique autant que technique.** Sa crédibilité repose sur la transparence du protocole, l'indépendance de l'opérateur et la traçabilité de chaque étape. Un tirage réalisé en public ou filmé vaut mieux qu'un tirage opaque, même techniquement parfait.

**La diversité ne s'obtient pas spontanément.** Un tirage purement aléatoire sur une liste de candidat·es volontaires ne produira pas automatiquement un MiniPublic représentatif : les candidat·es sont déjà un sous-ensemble biaisé. Le tirage structuré (stratifié) compense ce biais en garantissant la présence de profils sous-représentés.

**L'anonymisation est une condition de confiance.** Les membres du MiniPublic ne se connaissent pas avant les ateliers. L'anonymisation des données lors du tirage protège les candidat·es non sélectionné·es et renforce l'intégrité du processus.

**Le rapport de composition est un livrable jalon.** Il documente publiquement la composition du MiniPublic, les chiffres de candidatures, le protocole de garantie et les acteurs impliqués. Sa publication ancre la légitimité du processus auprès du grand public, des médias et des partenaires institutionnels.

---

## Outils

Le tirage au sort structuré utilise **Panelot**, un outil conçu pour les MiniPublics et les panels délibératifs. Il permet de :

- importer les données des candidat·es
- configurer les catégories de stratification et leurs quotas
- générer plusieurs distributions valides répondant à toutes les contraintes
- documenter le protocole et exporter les résultats

---

## Processus en cinq phases

### Phase 1 — Extraction et préparation des données

Les candidatures ont été collectées via le formulaire de mobilisation (ClickUp ou autre outil). Avant le tirage, les données doivent être extraites et nettoyées.

**Extraction depuis ClickUp :**
1. Exporter les réponses au formulaire en CSV depuis ClickUp (vue Tableur → Export)
2. Vérifier que toutes les candidatures attendues sont présentes
3. Identifier et traiter les doublons ou inscriptions invalides

**Nettoyage des données :**
- Uniformiser les valeurs dans chaque colonne de catégorie (ex. : « F », « Femme », « femme » → une seule valeur)
- Vérifier la cohérence des tranches d'âge (calculer à partir de la date de naissance si disponible)
- Compléter ou écarter les candidatures incomplètes selon le protocole défini lors du cadrage
- Documenter le nombre de candidatures valides retenues

### Phase 2 — Anonymisation

Avant l'import dans Panelot, anonymiser les données personnelles :

1. Remplacer les noms et prénoms par un identifiant numérique (ex. : `C001`, `C002`...)
2. Supprimer ou pseudonymiser les adresses email et numéros de téléphone
3. Conserver uniquement les variables de stratification (âge ou tranche d'âge, genre, niveau de formation, engagement, proximité, sous-catégories spécifiques)
4. Conserver la table de correspondance `identifiant ↔ données personnelles` dans un fichier séparé, sécurisé, accessible uniquement à l'AMU

Cette table de correspondance sera utilisée après le tirage pour identifier les personnes sélectionnées et les contacter.

### Phase 3 — Configuration dans Panelot et génération des distributions

**Import des données :**
1. Créer un nouveau projet dans Panelot
2. Importer le fichier CSV anonymisé
3. Définir les colonnes correspondant à chaque variable de stratification

**Configuration des catégories et quotas :**

Pour chaque variable, définir les modalités et les quotas cibles. Exemple tiré du projet Prairie-Nord (Morges) :

| Variable | Modalités | Quota MiniPublic (n=20) |
|---|---|---|
| Genre | Hommes / Femmes | 10 / 10 |
| Tranche d'âge | 08–15 / 16–25 / 26–35 / 36–45 / 46–55 / 56–65 / 66–75 / 76–85 | à définir selon candidatures |
| Niveau de formation | École obligatoire / Formation prof. / Études sup. / Autre | à définir selon candidatures |
| Engagement citoyen | Oui / Non | à définir selon candidatures |
| Proximité site | Quartier / Commune | à définir selon candidatures |
| Sous-catégories | Club Natation / Club Gym / Besoin particulier | 1 / 1 / 1 |

Les quotas sont définis en concertation avec la maîtrise d'ouvrage lors du cadrage. Certains quotas peuvent être des minimums (« au moins 1 personne de 8–15 ans ») plutôt que des cibles exactes.

**Génération des distributions :**

Lancer Panelot pour générer les distributions valides. Paramétrer le nombre de distributions à générer : **6 distributions** est la pratique recommandée, ce qui permet un tirage par dé à 6 faces.

Vérifier que chaque distribution respecte tous les quotas définis. Si aucune distribution valide ne peut être générée, revoir les quotas ou la taille du MiniPublic.

### Phase 4 — Tirage public

Le tirage désigne l'une des 6 distributions générées par Panelot. Ce moment est l'acte de légitimation du MiniPublic — il doit être réalisé de manière transparente.

**Deux modalités :**

**Tirage en public** (recommandé si le calendrier le permet) : organiser un événement court, ouvert à la presse et aux habitant·es. Un dé à 6 faces est lancé devant les personnes présentes. Le chiffre obtenu désigne la distribution retenue.

**Tirage filmé** : si aucune présence publique n'est possible, filmer le lancer de dé en incluant un témoin indépendant (représentant·e de la maîtrise d'ouvrage, journaliste, ou autre). Publier la vidéo sur la page web du processus.

Dans les deux cas : documenter la date, le lieu, les témoins présents, le résultat du tirage et la distribution retenue.

### Phase 5 — Identification et contact des personnes sélectionnées

1. Utiliser la table de correspondance pour identifier les personnes sélectionnées à partir de leurs identifiants
2. Les contacter par email ou téléphone selon la procédure définie dans `02-mobilisation.md`
3. Constituer la liste de suppléant·es à partir des distributions non retenues (prioriser les profils les plus proches des quotas de la distribution retenue)
4. Documenter les confirmations et refus dans le tableau de suivi (voir `outils/fr/gestion-emails-minipublic.md`)

---

## Livrable jalon — Rapport de composition du MiniPublic

À l'issue du tirage, l'AMU produit un **rapport de composition du MiniPublic**. Ce document est rendu public et constitue un livrable jalon du processus.

**Contenu du rapport :**

- Présentation du processus de tirage (pourquoi un MiniPublic, comment le tirage a eu lieu)
- Chiffres des candidatures reçues et validées
- Comparaison graphique candidatures / MiniPublic sélectionné pour chaque variable de stratification (genre, âge, formation, engagement, proximité)
- Description des sous-catégories spécifiques retenues
- Protocole de garantie : méthode, acteurs, transparence, protection des données
- Carte de localisation des candidat·es (anonymisée — niveau commune/quartier uniquement)
- Étapes suivantes du processus

**Destinataires et diffusion :**
- Publication sur la page web du projet (voir `06-transmission.md`)
- Transmission à la maîtrise d'ouvrage et à l'AMO
- Mise à disposition pour les médias sur demande

Ce rapport s'adresse à toutes les personnes concernées — il doit être rédigé dans un langage clair et accessible, sans jargon technique.

---

## Livrables de l'étape

- Fichier CSV anonymisé des candidatures valides
- Table de correspondance identifiants ↔ données personnelles (fichier sécurisé, usage AMU uniquement)
- Fichier projet Panelot avec les 6 distributions générées
- Documentation du tirage (procès-verbal, vidéo ou attestation de témoin)
- Liste des 20 membres du MiniPublic confirmés + liste de suppléant·es
- **Rapport de composition du MiniPublic** (document public)

---

## Points de vigilance

- **Conserver la table de correspondance en sécurité** : c'est la seule pièce qui relie les identifiants anonymes aux personnes réelles. Sa perte rend le tirage inutilisable.
- **Ne pas modifier les quotas après génération** : toute modification des critères après la génération des distributions invalide le protocole. Si des ajustements sont nécessaires, les faire avant de lancer Panelot et les documenter.
- **Anticiper les refus** : prévoir une liste de suppléant·es d'au moins 30% de la taille du MiniPublic. Les suppléant·es sont tirés des distributions non retenues.
- **Documenter chaque étape** : la légitimité du tirage repose sur sa traçabilité. Conserver les fichiers intermédiaires (données brutes, données nettoyées, données anonymisées, configurations Panelot, résultat du tirage).
- **Respecter la protection des données** : les données personnelles des candidat·es non sélectionné·es doivent être supprimées à l'issue du processus selon les modalités définies lors du cadrage (LPD, Suisse).
- **Rédiger le rapport de composition pour un public large** : éviter les graphiques trop techniques, soigner la lisibilité, utiliser des visuels accessibles. Ce document sera la première image publique du MiniPublic.
