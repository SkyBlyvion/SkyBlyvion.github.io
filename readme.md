# SkyBlyvion.github.io-main

## Présentation
Générateur de mots de passe sécurisé et convertisseur décimal/ASCII/hexadécimal/binaire, 100% local, sans tracking ni serveur.

## Fonctionnalités principales
- Générateur de mots de passe personnalisable (longueur, types de caractères, minimums par type, anti-doublons consécutifs)
- Évaluation de la robustesse du mot de passe
- Historique local des mots de passe générés
- Convertisseur décimal : affiche la valeur ASCII, hexadécimale et binaire pour toute valeur entre 0 et 255
- Calculateur d'adresse IP (CIDR, masque, plage, etc.)
- Interface moderne, responsive, mode sombre

## Sécurité
- Toutes les opérations sont réalisées localement dans le navigateur
- Aucune donnée n'est envoyée à un serveur
- Génération aléatoire via `crypto.getRandomValues`

## Utilisation
1. Ouvrez simplement `index.html` dans votre navigateur
2. Utilisez les onglets pour accéder au générateur, convertisseur ou calculateur IP
3. Aucun prérequis, aucune installation

## Conventions et bonnes pratiques
- Respect strict de la plage 0-255 pour le convertisseur décimal
- Affichage ASCII uniquement pour les caractères imprimables (32-126), sinon le code décimal est grisé
- Code commenté et lisible, tout dans `index.html`

## Développement
- Modifiez directement `index.html` pour toute évolution
- Utilisez les outils de développement du navigateur pour déboguer

## Licence
MIT