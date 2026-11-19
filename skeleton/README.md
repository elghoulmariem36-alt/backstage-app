
# ${{ values.name }}

${{ values.description }}

## Technologies utilisées

- Next.js
- React
- TypeScript
- Docker
- Docker Compose

## Installation

Installer les dépendances :

```bash
npm install
```

Lancer le projet en mode développement :

```bash
npm run dev
```

Ouvrir dans le navigateur :

http://localhost:3000

## Docker

Construire et lancer les conteneurs :

```bash
docker compose up -d --build
```

Arrêter les conteneurs :

```bash
docker compose down
```

## Build de production

```bash
npm run build
npm start
```

## Auteur

Généré automatiquement avec Backstage Scaffolder.

