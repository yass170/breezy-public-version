# Breezy — version publique

Projet web dont cette version publique présente la structure technique et l’architecture générale.

## Confidentialité et anonymisation

Ce dépôt est une présentation publique de la structure du projet. **Tous les contenus d’origine des fichiers conservés ont été supprimés pour des raisons de confidentialité.** Les fichiers de code, de configuration, de migration SQL, de tests, de gouvernance et les artefacts d’ingénierie conservés contiennent uniquement la phrase « Contenu anonymisé ». Cette règle s’applique aussi aux exemples et aux modèles.

Les données, secrets, fichiers binaires, dépendances embarquées, résultats générés, wireframes, journaux et dossiers de documentation de work ont été exclus. Les dossiers `.agent` et `.agents`, les fichiers `AGENTS.md` et les métadonnées Git d’origine sont absents. Les noms susceptibles de révéler une entreprise, une personne, un client ou un système interne ont été remplacés par des noms génériques.

Seuls ce README et les présentations d’architecture ont un contenu explicatif : ces textes ont été entièrement rédigés pour cette version publique, sans reprendre les détails internes. L’historique Git public commence avec cette version anonymisée.

## Fonctionnement général

Les dossiers conservés représentent les composants du projet web, leur configuration et leurs tests lorsqu’ils sont présents. Les fichiers de programmation et les paramètres ont été remplacés par un marqueur ; cette vue ne décrit aucun environnement interne.

Formats techniques représentés : TypeScript, JavaScript, SQL, CSS, scripts shell, configuration textuelle.

La copie permet de parcourir l’organisation technique et d’identifier les familles de composants. **Elle ne permet ni d’exécuter ni de reconstruire le projet.** Les configurations et les migrations sont volontairement incomplètes et ne doivent pas être lancées.

## Organisation

- `.dockerignore`
- `.github/`
- `.prettierrc`
- `apps/`
- `docker-compose.yml`
- `docs/`
- `eslint.config.mjs`
- `fichier-001.yml`
- `fichier-002.ts`
- `fichier-003.json`
- `module-009/`
- `module-012/`
- `module-014/`
- `package-lock.json`
- `package.json`
- `scripts/`

Les noms `module-…` et `fichier-…` désignent des éléments renommés. Les extensions des fichiers textuels conservés indiquent leur format d’origine.

Consulter [ARCHITECTURE.md](ARCHITECTURE.md) pour la présentation générale.
