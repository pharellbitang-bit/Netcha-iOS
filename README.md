# Netcha for iOS

Version iOS de **Netcha**, indépendante de Netcha+.

Ce dépôt prépare une application iPhone basée sur Capacitor 8.6.0 et connectée au service Netcha existant par HTTPS. Il ne contient ni copie de la base de données ni modification du backend.

## État

- Structure iOS en préparation.
- Application web Netcha chargée depuis le service de production existant.
- Accès caméra, microphone et photothèque déclarés pour les fonctions compatibles.
- La compilation Simulator sert aux tests et n'est pas installable directement sur un iPhone physique.

## Prérequis

- Node.js 22+
- Xcode 26+ sur macOS
- Capacitor 7

## Développement

```bash
npm install
npx cap add ios
npx cap sync ios
npx cap open ios
```

## Compilation iPhone et App Store

Une archive destinée à un iPhone physique ou à l'App Store doit être signée avec une identité Apple et un provisioning profile valides. La préparation du code et une compilation pour simulateur peuvent être réalisées sans abonnement Apple Developer ; la distribution signée nécessite les accès Apple appropriés.

## Protection du projet

Le dépôt cible uniquement Netcha. Ne pas importer Netcha+, ne pas modifier le backend ni les données de production dans le cadre de cette préparation.
