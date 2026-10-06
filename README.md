# Gym IA Pasteur 2026

Outil d'évaluation en gymnastique (EPS, collège) : saisie des évaluations au sol et aux agrès, puis impression de fiches élèves et de feuilles de jugement.

Tout tient dans un seul fichier, `index.html`. Il fonctionne hors ligne et ne se connecte à aucun serveur : les noms et les notes des élèves restent sur l'ordinateur de l'enseignant.

## Ouvrir l'outil

- **En ligne** : via le lien GitHub Pages du dépôt.
- **Hors ligne** : télécharger `index.html` et l'ouvrir par un double-clic dans Chrome ou Edge.

Les données saisies ne sont jamais envoyées sur GitHub ni ailleurs, même quand l'outil est ouvert depuis le lien en ligne.

## Les onglets

| Onglet | Rôle |
|---|---|
| 1 · Élèves | Importer une liste de classe (CSV, par exemple un export Pronote), choisir le programme de chaque classe et l'agrès de chaque élève, régler la sauvegarde. |
| 2 · Évaluer | Créer une évaluation (sol ou agrès), noter la présence, puis cliquer le niveau réalisé (A à D) et le statut de chaque figure. |
| 3 · Fiches | Imprimer une fiche par élève : ce qu'il a fait, ce qu'il doit travailler, et le code pour composer son enchaînement. |
| 4 · Jugement | Imprimer des feuilles de jugement entre partenaires (sol, barres, poutre), vierges ou au nom des élèves. |
| 5 · Récapitulatif | Voir le meilleur niveau réussi par élève et par figure, avec une synthèse par classe. |

## Barème

- Niveau A = 1 point, B = 2, C = 3, D = 4.
- Statut de la figure : réussi (tous les points), à améliorer (−0,5 point), raté (0 point).
- Au sol, les 2 sauts comptent pour une seule figure : la moyenne des deux.
- Fluidité, notée sur 4 selon la connaissance de l'enchaînement : par cœur (4), presque entièrement (3), il se perd (2), ne le connaît pas (1).
- Si l'élève présente plus de figures que demandé, seules celles qui rapportent le plus de points comptent.

## Programmes par niveau de classe

| Programme | Sol | Agrès | Fiches imprimées |
|---|---|---|---|
| 6ème | Capitalisation : valider le plus de figures possible, sans enchaînement | — | Recto seul |
| 4ème 2h | 4 figures | 1 agrès, 4 figures | Recto-verso (sol et agrès, puis les codes) |
| 4ème 1h | 4 figures | — | Recto-verso (fiche et code, puis feuille de jugement) |
| 3ème 2h | 5 figures | 1 agrès, 4 figures | Recto-verso |
| 3ème 1h | 5 figures | — | Recto-verso |

Avec 5 figures, la note est calculée sur 24 points puis ramenée sur 20.

Aux agrès, l'enchaînement commence par une entrée et finit par une sortie. Aux barres, les 4 familles sont obligatoires ; à la poutre, l'élève en choisit 4 sur 5.

## Figure à travailler

| Résultat à la dernière évaluation | Ce que la fiche propose |
|---|---|
| Raté ou à améliorer, niveau précédent déjà réussi | Retravailler le même niveau |
| Raté ou à améliorer, niveau précédent jamais réussi | Revenir au niveau précédent |
| Réussi | Viser le niveau suivant |

Une figure ratée à l'évaluation d'avant, et pas réussie depuis, reste dans les éléments à travailler. Quand l'élève a présenté moins de figures que demandé, la fiche complète avec des propositions de niveau A.

## Sauvegarde

- **Sauvegarde automatique** (Chrome, Edge) : choisir une fois un fichier CSV sur l'ordinateur ou sur un dossier réseau de l'établissement. Chaque modification y est ensuite enregistrée automatiquement. À la prochaine ouverture, le bouton « Reprendre » recharge ce fichier.
- **Télécharger une copie** : crée un CSV daté, à garder comme sauvegarde.
- Le fichier de sauvegarde est un CSV ordinaire (séparateur point-virgule), lisible dans Excel.

## Impression

- Format A4 paysage, marges « aucune ».
- Cocher « graphiques d'arrière-plan ».
- Recto-verso sur le bord long.
- Imprimer une classe à la fois, en la choisissant dans le menu en haut de l'outil.
- Les fiches sont conçues pour une impression en noir et blanc.

## Données personnelles

L'outil ne transmet aucune donnée. Les fichiers CSV contenant les noms des élèves doivent rester sur un poste ou un espace de stockage professionnel. **Ne jamais les déposer dans ce dépôt GitHub.**
