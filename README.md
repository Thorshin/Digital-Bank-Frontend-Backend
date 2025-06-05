# Banque Digitale - Frontend et Backend

Ce dépôt contient une application complète de banque digitale réalisée avec Angular pour la partie frontend et Spring Boot pour la partie backend.

## Présentation

L'application permet de gérer des comptes bancaires, d'effectuer des opérations de crédit et de débit et d'afficher les historiques des opérations. Le frontend communique avec l'API REST exposée par le backend.

## Prérequis

- **Node.js** et **npm** pour exécuter l'interface Angular.
- **Java 21** ainsi que **Maven** (via le wrapper fourni) pour le backend Spring Boot.

## Installation

1. Cloner le dépôt.
2. Installer les dépendances du frontend :
   ```bash
   cd digital-banking-angular-front
   npm install
   ```
3. Lancer le backend :
   ```bash
   cd ../digital-banking-spring-backend
   ./mvnw spring-boot:run
   ```
4. Dans un autre terminal, démarrer l'application Angular :
   ```bash
   cd ../digital-banking-angular-front
   npm start
   ```

## Captures d'écran

Quelques exemples de l'interface utilisateur sont disponibles dans le dossier `screenshots` :

![Liste des comptes](screenshots/screenshot1.png)

![Détail d'un compte](screenshots/screenshot2.png)

## Tests

Des tests unitaires sont fournis pour le frontend et le backend. Ils peuvent être lancés avec :

```bash
cd digital-banking-spring-backend
./mvnw test

cd ../digital-banking-angular-front
npm test -- --watch=false
```

