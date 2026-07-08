# Coffre 🔐

Coffre-fort de mots de passe personnel — application web installable sur iPhone (PWA), **chiffrée** et **100 % locale**.

- **Chiffrement AES‑256‑GCM** : mots de passe et identifiants sont chiffrés par une clé maître, elle-même protégée par un code à 6 chiffres (PBKDF2‑SHA256, 310 000 itérations). Rien n'est stocké en clair.
- **Accès** : code à 6 chiffres + Face ID / Touch ID (optionnel).
- **Aucune donnée envoyée** : tout reste dans le navigateur de l'appareil. Aucun serveur, aucun compte.
- **Fonctionne hors-ligne** une fois installée.

## Installation sur iPhone

1. Ouvrir le site dans **Safari**.
2. **Partager → Sur l'écran d'accueil**.
3. Lancer *Coffre* depuis l'écran d'accueil et choisir son code.

> ⚠️ Installer l'app **avant** de saisir ses mots de passe : sur iOS, Safari et l'app installée ne partagent pas le même stockage.

## Structure

Application mono-fichier : [`index.html`](index.html) + annexes PWA (`sw.js`, `manifest.webmanifest`, icônes). Tous les chemins sont relatifs — fonctionne en sous-répertoire.
