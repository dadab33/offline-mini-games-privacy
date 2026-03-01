# Politique de confidentialité — Offline Mini Games

**Date d'entrée en vigueur :** 20 février 2026  
**Dernière mise à jour :** 28 février 2026

---

## 1. Introduction

Offline Mini Games (ci-après « l'Application ») est une application mobile de mini-jeux conçue pour fonctionner **entièrement hors-ligne**. Cette politique de confidentialité explique quelles données sont utilisées, comment elles sont traitées et quels droits vous avez.

L'Application intègre des services tiers (Google AdMob pour les publicités, Google Play Games Services pour les classements et succès) qui peuvent collecter certaines données conformément aux politiques de Google. Nous vous informons de manière transparente de ces collectes ci-dessous.

---

## 2. Données collectées

### 2.1 Données collectées directement par l'Application

L'Application **ne collecte aucune donnée personnelle directement**. Les seules informations stockées localement sont :

| Type de donnée | Localisation | Finalité |
|---|---|---|
| Scores et meilleurs scores | Appareil local uniquement | Affichage de la progression |
| Préférences utilisateur (son, vibration, langue) | Appareil local uniquement | Personnalisation de l'expérience |
| État d'avancement dans les niveaux | Appareil local uniquement | Continuité du jeu |
| Statut premium (achat sans pub) | Appareil local uniquement | Désactivation des publicités |

Ces données sont stockées exclusivement sur votre appareil via `shared_preferences` et **ne quittent jamais votre appareil**.

### 2.2 Données collectées indirectement via les services tiers

L'Application intègre des services tiers susceptibles de collecter des données :

| Service | Données collectées | Finalité |
|---|---|---|
| **Google AdMob** | Identifiant publicitaire (IDFA/GAID), données comportementales anonymisées | Affichage de publicités ciblées |
| **Google Play Games Services** | Identifiant de compte Google, scores soumis aux classements, succès débloqués | Classements et succès publics |
| **Google Play Billing** | Données de transaction gérées par Google Play | Achat in-app « Supprimer les publicités » |

Ces données sont collectées et traitées par Google selon sa [Politique de confidentialité](https://policies.google.com/privacy).

### 2.3 Consentement publicitaire (RGPD / CCPA)

Conformément au Règlement Général sur la Protection des Données (RGPD) et aux exigences de Google AdMob, l'Application affiche un **formulaire de consentement** aux utilisateurs situés dans l'Espace Économique Européen (EEE) lors du premier lancement :

- **Consentement accordé** → publicités personnalisées (AdMob utilise votre identifiant publicitaire).
- **Consentement refusé** → publicités non personnalisées (aucun ciblage basé sur votre profil).
- **Utilisateur premium** → aucune publicité, aucun consentement demandé.

Vous pouvez modifier votre choix à tout moment depuis les paramètres de l'Application.

---

## 3. Connectivité réseau

L'Application fonctionne **sans connexion Internet** pour les jeux en solo. Les fonctionnalités suivantes nécessitent ponctuellement une connexion réseau :

| Fonctionnalité | Réseau requis |
|---|---|
| Affichage des publicités AdMob | Oui (HTTPS vers serveurs Google) |
| Synchronisation des classements Play Games | Oui (HTTPS vers serveurs Google) |
| Achat in-app (suppression des pubs) | Oui (Google Play) |

En l'absence de connexion, ces fonctionnalités sont silencieusement ignorées : les jeux restent pleinement jouables.

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

L'Application intègre les services tiers suivants :

| Service | Éditeur | Utilisation | Politique de confidentialité |
|---|---|---|---|
| **Google AdMob** | Google LLC | Affichage de publicités (utilisateurs non premium) | [policies.google.com/privacy](https://policies.google.com/privacy) |
| **Google Play Games Services** | Google LLC | Classements, succès, connexion compte Google | [policies.google.com/privacy](https://policies.google.com/privacy) |
| **Google Play Billing** | Google LLC | Achat in-app « Supprimer les publicités » | [play.google.com/about/play-terms](https://play.google.com/about/play-terms) |

> **Note :** Si vous n'êtes pas connecté à Google Play Games et que vous n'avez pas accordé de consentement publicitaire, aucune donnée n'est transmise à des tiers.

---

## 6. Mineurs

L'Application est accessible à tous les publics, y compris aux personnes de moins de 18 ans. Concernant la publicité :

- AdMob est configuré avec `tagForChildDirectedTreatment: false` (public général).
- Si votre application cible principalement des enfants de moins de 13 ans, ce paramètre doit être mis à `true` (conformité COPPA).
- Les utilisateurs mineurs sont encouragés à utiliser la version premium (sans publicité).

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
**Développeur :** *Damien.bertrand33@gmail.com*  
**Pays :** *France*

---

## 11. Droit applicable

Cette politique est rédigée conformément au **Règlement Général sur la Protection des Données (RGPD)** de l'Union Européenne et aux lois applicables dans le pays du développeur.

Dans la mesure où l'Application ne collecte aucune donnée personnelle, elle n'est pas soumise aux obligations de désignation d'un DPO ni de tenue de registre de traitement au sens du RGPD.

---

*Cette politique de confidentialité a été rédigée spécifiquement pour l'Application Offline Mini Games et reflète fidèlement son fonctionnement technique.*
