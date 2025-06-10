
# Cahier des charges

## Projet : Générateur de mot de passe sécurisé

### Spécifications initiales

- Génération de mot de passe
- Longueurs possibles : 8, 12, 16, 20 caractères
- Chiffres : 0 - 9
- Lettres minuscules et majuscules : a - Z
- Caractères spéciaux : %$

---

## Objectif

Créer une application simple, rapide et sécurisée permettant de générer des mots de passe aléatoires répondant à des critères personnalisables de sécurité.

---

## Fonctionnalités attendues

- Génération de plusieurs mots de passe à la demande
- Longueurs disponibles : **8**, **12**, **16**, **20** caractères
- Types de caractères pris en charge :
  - Lettres minuscules : `a-z`
  - Lettres majuscules : `A-Z`
  - Chiffres : `0-9`
  - Caractères spéciaux : `%$` (extensible à d’autres comme `!@#^&*`)
- Personnalisation :
  - Sélection des types de caractères à inclure (via interface ou paramètres)
- Affichage du ou des mots de passe générés
- Bouton pour copier le mot de passe dans le presse-papiers
- Fonction de régénération
- Mode sombre / clair
- Évaluation de la solidité du mot de passe généré

---

## Interface utilisateur

- Sélecteur pour la longueur du mot de passe (menu déroulant ou boutons radio)
- Cases à cocher pour activer/désactiver :
  - Lettres majuscules
  - Lettres minuscules
  - Chiffres
  - Caractères spéciaux
- Bouton **Générer**
- Champ en lecture seule pour afficher le mot de passe
- Bouton **Copier**

---

## Contraintes techniques

- Application web légère (HTML / CSS / JavaScript pur)
- Code lisible et commenté
- Fonctionnement 100 % local (aucune dépendance serveur)

---

## Sécurité

- Génération de mot de passe à partir d’une source de hasard cryptographique (`crypto.getRandomValues` en JavaScript)
- Aucune information n’est envoyée à un serveur externe