# Politique de confidentialité — Offline Mini Games

**Date d'entrée en vigueur :** 20 février 2026  
**Dernière mise à jour :** 20 février 2026

---

## 1. Introduction

Offline Mini Games (ci-après « l'Application ») est une application mobile de mini-jeux conçue pour fonctionner **entièrement hors-ligne**. Cette politique de confidentialité explique quelles données sont utilisées, comment elles sont traitées et quels droits vous avez.

Nous prenons votre vie privée au sérieux. Notre principe de base : **nous ne collectons pas vos données personnelles et nous ne les transmettons à personne**.

---

## 2. Données collectées

### 2.1 Données collectées par l'Application

L'Application **ne collecte aucune donnée personnelle**. Les seules informations stockées sont :

| Type de donnée | Localisation | Finalité |
|---|---|---|
| Scores et meilleurs scores | Appareil local uniquement | Affichage de la progression |
| Préférences utilisateur (son, vibration, langue) | Appareil local uniquement | Personnalisation de l'expérience |
| État d'avancement dans les niveaux | Appareil local uniquement | Continuité du jeu |

Ces données sont stockées exclusivement sur votre appareil via le mécanisme de stockage local (`shared_preferences`) et **ne quittent jamais votre appareil**.

### 2.2 Données non collectées

L'Application **ne collecte pas** :

- Nom, prénom ou identité
- Adresse e-mail ou tout autre coordonnée
- Numéro de téléphone
- Localisation géographique
- Identifiant publicitaire
- Données biométriques
- Historique de navigation ou d'utilisation transmis à un serveur
- Toute autre donnée à caractère personnel

---

## 3. Connectivité réseau

L'Application **ne requiert aucune connexion Internet** et **n'effectue aucune communication réseau externe**. Aucune donnée n'est envoyée vers nos serveurs ou vers des serveurs tiers.

---

## 4. Fonctionnalité Bluetooth (multijoueur local)

Certains mini-jeux proposent un mode multijoueur en local via **Bluetooth/Wi-Fi Direct**, permettant à deux appareils proches de jouer ensemble sans Internet.

### 4.1 Utilisation du Bluetooth

- La connexion Bluetooth est **strictement locale** entre les appareils participants.
- Seules les **données de jeu en cours** (événements de partie, scores de session) transitent via cette connexion.
- Ces données sont éphémères : elles ne sont **ni stockées**, ni transmises à un tiers.
- La connexion Bluetooth est **exclusive aux jeux compatibles** et n'est jamais activée en arrière-plan.

### 4.2 Permissions requises

Sur Android, le système impose les permissions suivantes pour utiliser le Bluetooth et la découverte de proximité :

| Permission | Raison |
|---|---|
| `BLUETOOTH` / `BLUETOOTH_CONNECT` | Connexion entre deux appareils pour le jeu local |
| `BLUETOOTH_SCAN` / `BLUETOOTH_ADVERTISE` | Découverte et appairage des appareils proches |
| `ACCESS_FINE_LOCATION` *(Android ≤ 11)* | Requise par Android pour le scan Bluetooth. **La position GPS n'est pas lue ni stockée.** |
| `NEARBY_WIFI_DEVICES` *(Android 13+)* | Découverte d'appareils locaux via Wi-Fi Direct |

> **Important :** La permission de localisation est exigée par le système Android pour des raisons techniques liées au scan Bluetooth. L'Application **ne lit, ne collecte ni ne traite aucune donnée de localisation géographique**.

Ces permissions sont demandées **uniquement au moment où vous accédez à un mini-jeu Bluetooth** et vous pouvez refuser sans impact sur les jeux en mode solo.

---

## 5. Services tiers

L'Application **n'intègre aucun service tiers** tel que :

- Outils d'analyse (Google Analytics, Firebase, etc.)
- Réseaux publicitaires
- SDK de collecte de données
- Services de crash reporting externes

---

## 6. Mineurs

L'Application est accessible à tous les publics, y compris aux personnes de moins de 18 ans. Dans la mesure où **aucune donnée personnelle n'est collectée**, aucun régime de protection spécifique aux mineurs n'est applicable.

---

## 7. Sécurité des données

Les données stockées localement (scores, préférences) sont protégées par le mécanisme de sécurité standard du système d'exploitation de votre appareil. Elles ne quittant jamais l'appareil, elles ne sont exposées à aucun risque de transmission ou de piratage réseau.

---

## 8. Suppression des données

Vous pouvez supprimer l'intégralité des données locales à tout moment en désinstallant l'Application. La réinitialisation peut également être effectuée depuis les paramètres de l'Application.

---

## 9. Modifications de cette politique

Toute mise à jour de cette politique de confidentialité sera publiée sur cette page avec une nouvelle date de mise à jour. En cas de changement significatif, une notification sera affichée dans l'Application.

---

## 10. Contact

Pour toute question relative à cette politique de confidentialité, vous pouvez nous contacter à :

**E-mail :** *contact@sanotema.com*  
**Développeur :** *Damien Bertrand*  
**Pays :** *France*

---

## 11. Droit applicable

Cette politique est rédigée conformément au **Règlement Général sur la Protection des Données (RGPD)** de l'Union Européenne et aux lois applicables dans le pays du développeur.

Dans la mesure où l'Application ne collecte aucune donnée personnelle, elle n'est pas soumise aux obligations de désignation d'un DPO ni de tenue de registre de traitement au sens du RGPD.

---

*Cette politique de confidentialité a été rédigée spécifiquement pour l'Application Offline Mini Games et reflète fidèlement son fonctionnement technique.*
