# Gestion de projet — MedScope

## Méthodologie
Approche itérative de type Kanban, découpée par étapes alignées sur le référentiel CDA (Conception → Environnement → Développement par blocs → Tests & CI/CD).

## Outils collaboratifs
- **Gestion de versions :** Git & GitHub (`https://github.com/K-marcos01/MedScope`)
- **Suivi des tâches :** GitHub Projects (`MedScope - Suivi`) avec colonnes `Todo`, `In Progress`, `Done`

## Stratégie de branches (GitFlow)
- `main` : code stable, validé et prêt pour la production
- `develop` : branche d'intégration des fonctionnalités terminées
- `feature/*` : développement isolé d'une fonctionnalité ou d'un livrable (créée depuis `develop`, fusionnée via Pull Request)
- `release/*` : préparation et stabilisation d'une version avant mise en production sur `main`
- `hotfix/*` : correction urgente d'un bug critique en production (créée depuis `main`, réintégrée dans `main` et `develop`)

## Convention de commits
Format *Conventional Commits* :
- `docs:` documentation et conception
- `chore:` configuration, outillage, Docker
- `feat:` nouvelle fonctionnalité
- `fix:` correction de bug
- `test:` ajout ou modification de tests