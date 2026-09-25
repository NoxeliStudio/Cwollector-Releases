# Patchnotes Cwollector

## 0.3.84-beta — 25/09/2026

Bêta 0.3.84 — correctif critique de l’updater Android.

• Correction du crash au démarrage introduit en 0.3.83.
• Suppression complète des appels Java/JNI réseau automatiques au lancement du jeu.
• Vérification des mises à jour via HTTPRequest avec l’API GitHub officielle en endpoint principal et raw.githubusercontent.com en secours.
• Retries par endpoint conservés pour fiabiliser la détection des nouvelles versions.
• DownloadManager Android conservé uniquement au moment où l’utilisateur appuie sur « METTRE À JOUR ».
• Contrôle des exceptions Java ajouté autour du DownloadManager afin d’éviter un crash si Android refuse une opération native.
• Bouton de secours vers la page officielle des versions conservé.
• Aucun changement d’équilibrage ou de contenu gameplay dans cette hotfix.

Cette correction a été validée sur téléphone avec une build de test : démarrage OK et vérification de version OK.

- Android : APK Release signé officiel Noxeli Studio.
- versionCode : 11.
- Statut pré-release : true.
- Mise à jour obligatoire : false.

Téléchargement officiel : [Cwollector 0.3.84 Beta](https://github.com/NoxeliStudio/Cwollector-Releases/releases/tag/v0.3.84-beta)


## 0.3.83-beta — 24/09/2026

Bêta 0.3.83 — refonte de l’updater Android.

• Vérification des mises à jour via les API Android natives en priorité, au lieu de dépendre uniquement de HTTPRequest Godot.
• Utilisation de java.net.HttpURLConnection sur Android avec l’API GitHub comme endpoint principal et raw.githubusercontent.com en secours.
• HTTPRequest Godot conservé uniquement comme dernier fallback.
• Téléchargement des APK confié au DownloadManager Android : téléchargement en arrière-plan, reprise réseau et notification système à la fin.
• Nouveau champ download_url dans latest.json réservé au téléchargement natif Android ; les anciennes builds continuent d’ouvrir la page officielle de release.
• Bouton de secours « OUVRIR LA PAGE DES VERSIONS » disponible si les vérifications intégrées échouent.
• Aucun changement d’équilibrage ou de contenu gameplay dans cette hotfix.

L’installation finale reste confirmée par Android.

- Android : APK Release signé officiel Noxeli Studio.
- versionCode : 9.
- Statut pré-release : true.
- Mise à jour obligatoire : false.

Téléchargement officiel : [Cwollector 0.3.83 Beta](https://github.com/NoxeliStudio/Cwollector-Releases/releases/tag/v0.3.83-beta)


## 0.3.82-beta — 24/09/2026

Bêta 0.3.82 — hotfix du système de mise à jour Android.

• Vérification des mises à jour rendue plus fiable avec jusqu’à 3 tentatives automatiques.
• Nouvelle vérification lorsque Cwollector revient au premier plan après un passage en arrière-plan.
• Nouveau bouton « RECHERCHER UNE MISE À JOUR » dans les Réglages avec état visible.
• Le bouton de mise à jour ouvre désormais la page officielle de la release GitHub plutôt que le téléchargement direct de l’APK, afin d’éviter les téléchargements bloqués à 100 % sur certains appareils Android.
• Synchronisation automatique du versionCode interne de l’updater avec le versionCode Android pendant les futures releases.
• Le saut de version reste supporté : une ancienne bêta peut passer directement à la dernière version disponible sans installer toutes les versions intermédiaires.

Aucun changement d’équilibrage ou de contenu gameplay dans cette hotfix.

- Android : APK Release signé officiel Noxeli Studio.
- versionCode : 8.
- Statut pré-release : true.
- Mise à jour obligatoire : false.

Téléchargement officiel : [Cwollector 0.3.82 Beta](https://github.com/NoxeliStudio/Cwollector-Releases/releases/tag/v0.3.82-beta)


## 0.3.81-beta — 24/09/2026

Bêta 0.3.81 — grosse passe de stabilisation et de finition avant ouverture plus large.

• Interface mobile revue et homogénéisée : Accueil/HUD, Collection, Boutique, Missions, Événements/Roulette, Succès et fiches de cartes.
• 89 cartes actives et 14 familles progressives complètes.
• Succès recalibrés : 50 paliers atteignables avec le contenu actuel, migration des anciennes sauvegardes sans double récompense.
• Missions fiabilisées : plus d'objectif de découverte impossible et meilleure gestion des 5 missions Club Cwok.
• Pass bêta utilisables dans les builds Release : Cwollector Auto, Pack XXL, Joker Doublon, Club Cwok et Héritage Astral.
• Pack XXL sécurisé : activer/désactiver le pass ne reroll plus le pack préchargé et ne modifie jamais le jet Secrète.
• Joker Doublon fiabilisé pour chercher un remplacement réellement disponible.
• Récompenses de familles complètes sécurisées et désormais signalées en jeu.
• Prestige/Héritage Astral et familles préparés pour le futur contenu sans casser les progressions 6/6 existantes.
• Roulette renforcée contre les tirages sauvegardés invalides, tout en conservant Cwok Roulette à 0,5 % par lancer.
• Codes Event renforcés et maintenant conservés dans la sauvegarde principale lors des transferts.
• Sauvegarde passée en version 21 avec migrations et réparations automatiques.
• Nombreux correctifs Android, navigation, pagination Collection et protections anti-duplication/anti-reroll.

Équilibrage important inchangé :
• Carte Secrète des packs : exactement 1/1000 par pack, même avec Pack XXL.
• Cwok Roulette : 0,5 % par lancer.

Merci pour les tests de la bêta ❤️

- Android : APK Release signé officiel Noxeli Studio.
- versionCode : 7.
- Statut pré-release : true.
- Mise à jour obligatoire : false.

Téléchargement officiel : [Cwollector 0.3.81 Beta](https://github.com/NoxeliStudio/Cwollector-Releases/releases/tag/v0.3.81-beta)


Les notes des versions publiques de Cwollector sont archivées ici en complément des GitHub Releases.

## 0.3.80-beta — 22 septembre 2026

Mise à jour bêta officielle de **Cwollector**.

- Android : APK Release signé officiel Noxeli Studio.
- `versionCode` : 6.
- Système de mise à jour intégré via GitHub.
- Ajout du transfert de sauvegarde.
- Distribution : GitHub Releases.
- Statut : pré-release bêta.
- Mise à jour obligatoire : non.

Téléchargement officiel : [Cwollector 0.3.80 Beta](https://github.com/NoxeliStudio/Cwollector-Releases/releases/tag/v0.3.80-beta)

## 0.3.79-beta — 22 septembre 2026

Première version bêta officielle distribuée par **Noxeli Studio**.

- Android : APK Release signé officiel.
- `versionCode` : 5.
- Distribution : GitHub Releases.
- Statut : pré-release bêta.
- Mise à jour obligatoire : non.

Téléchargement officiel : [Cwollector 0.3.79 Beta](https://github.com/NoxeliStudio/Cwollector-Releases/releases/tag/v0.3.79-beta)
