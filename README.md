# Balagh – application Android

## 1. Créer le dépôt GitHub
1. Sur github.com : **New repository** → nom `balagh-android` → Create.
2. Téléverser tout le contenu de ce dossier (glisser-déposer dans la page du dépôt), y compris `.github/` et `www/`.

## 2. Compiler l'APK automatiquement
1. Onglet **Actions** → le workflow « Build Android APK » se lance à chaque `push`.
2. Attendre la fin (environ 5 à 10 minutes).
3. Ouvrir l'exécution → section **Artifacts** → télécharger `balagh-debug-apk`.
4. Dézipper : vous obtenez `app-debug.apk`.

## 3. Installer sur un téléphone Android
1. Copier `app-debug.apk` sur le téléphone.
2. Ouvrir le fichier et autoriser l'installation depuis cette source.
3. Au premier lancement, accepter l'accès à la **localisation** et à la **caméra**.

## 4. Mettre à jour l'application
Remplacer `www/index.html` par une nouvelle version, puis faire un `git commit` et `git push`. Un nouvel APK est généré.

## 5. Publier sur le Play Store (plus tard)
Il faut un APK signé (AAB) avec une clé de signature et un compte Google Play Console (frais unique d'environ 25 USD).

## Icône de l'application
- L'icône vient de `resources/icon.png` (1024×1024, fond transparent).
- Pour la changer, remplacez ce fichier par une image carrée de 1024×1024, puis refaites un `git push`.
- Les couleurs de fond de l'icône sont #F6F0E6 (clair) et #13251C (sombre), de la charte Balagh.
