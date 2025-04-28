# Guide de contribution

Merci de l'intérêt que vous portez aux projets de Cérebrum. Nous sommes ravis de votre volonté de contribuer ! Ce document vous guidera à travers notre processus de contribution.

## Table des matières

- [Code de conduite](#code-de-conduite)
- [Comment contribuer](#comment-contribuer)
- [Signaler des bugs](#signaler-des-bugs)
- [Soumettre des demandes de fonctionnalités](#soumettre-des-demandes-de-fonctionnalités)
- [Environnement de développement](#environnement-de-développement)
- [Style et standards de code](#style-et-standards-de-code)
- [Processus de Pull Request](#processus-de-pull-request)
- [Tests](#tests)
- [Documentation](#documentation)

## Code de conduite

Nous attendons de tous les participants qu'ils respectent notre [Code de conduite](CODE_OF_CONDUCT.md). Veuillez le lire avant de contribuer.

## Comment contribuer

### Signaler des bugs

Si vous trouvez un bug, veuillez le signaler en créant une issue en utilisant le [template de rapport de bug](.github/ISSUE_TEMPLATE/bug_report.md). Avant de créer une nouvelle issue, veuillez vérifier si le bug n'a pas déjà été signalé. 

Pour un rapport de bug efficace :
- Utilisez un titre clair et descriptif
- Décrivez les étapes précises pour reproduire le problème
- Décrivez le comportement attendu et le comportement observé
- Incluez des captures d'écran si possible
- Mentionnez votre environnement (navigateur, système d'exploitation, etc.)

### Soumettre des demandes de fonctionnalités

Si vous souhaitez proposer une nouvelle fonctionnalité, utilisez le [template de demande de fonctionnalité](.github/ISSUE_TEMPLATE/feature_request.md). Décrivez clairement la fonctionnalité et expliquez pourquoi elle serait utile pour le projet.

## Environnement de développement

Pour configurer votre environnement de développement :

1. Clonez le dépôt :
```bash
git clone https://github.com/cerebrumwebsite/[nom-du-dépôt].git
cd [nom-du-dépôt]
```

2. Installez les dépendances :
```bash
npm install
# ou
yarn install
```

3. Configurez les variables d'environnement en copiant le fichier .env.example :
```bash
cp .env.example .env.local
```

4. Lancez le serveur de développement :
```bash
npm run dev
# ou
yarn dev
```

## Style et standards de code

Nous utilisons les conventions suivantes :

- **JavaScript/TypeScript** : Nous suivons les règles ESLint définies dans notre configuration
- **CSS/SCSS** : Nous utilisons Tailwind CSS
- **Markdown** : Indentation à 2 espaces, lignes maximales de 80 caractères
- **Commits** : Suivez le format [Conventional Commits](https://www.conventionalcommits.org/)
  - `feat: ajouter nouvelle fonctionnalité`
  - `fix: corriger un bug`
  - `docs: mettre à jour la documentation`
  - `style: changements de formatage`
  - `refactor: refactorisation du code`
  - `test: ajouter/modifier des tests`
  - `chore: tâches de maintenance`

## Processus de Pull Request

1. Créez une branche à partir de `main` (ou `develop` selon le projet) :
```bash
git checkout -b type/nom-court-descriptif
# Exemple : feat/ajouter-auth ou fix/corriger-navbar
```

2. Apportez vos modifications et commitez-les selon les conventions ci-dessus

3. Assurez-vous que les tests sont réussis :
```bash
npm run test
```

4. Poussez vos modifications et créez une Pull Request en utilisant le template fourni

5. Un membre de l'équipe Cérebrum examinera votre PR et pourra demander des modifications

## Tests

Tous les nouveaux codes doivent être accompagnés de tests. Nous utilisons Jest comme framework de test. Pour exécuter les tests :

```bash
npm run test
# ou pour un test spécifique
npm run test -- -t "nom du test"
```

## Documentation

Pour toute nouvelle fonctionnalité ou modification, assurez-vous de :
- Mettre à jour les commentaires dans le code
- Mettre à jour ou créer des fichiers de documentation si nécessaire
- Inclure des exemples d'utilisation si pertinent

---

Merci encore pour votre contribution ! Si vous avez des questions, n'hésitez pas à nous contacter.
