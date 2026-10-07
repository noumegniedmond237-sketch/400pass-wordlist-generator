# 400PASS // 400WORDS

> Générateur de dictionnaire universel (wordlist) au thème « terminal hacker » — **100 % local, dans un seul fichier HTML**. Aucune installation, aucun serveur, aucune dépendance.

![stack](https://img.shields.io/badge/stack-HTML%20%2B%20CSS%20%2B%20JS-00ff41)
![licence d'usage](https://img.shields.io/badge/usage-tests%20autoris%C3%A9s%20uniquement-ff2d55)

## ✨ Fonctionnalités

- **Longueur minimale / maximale** de la partie variable (1 à 32 caractères)
- **Jeux de caractères** : lettres minuscules, majuscules, chiffres et **33 symboles spéciaux** (`& ! @ # $ % ^ * ( ) _ + - = < > , . / ? [ ] { } ~ : ; \` ' | " \` et Espace)
- **Grille de sélection symbole par symbole** dans la modale « Détails », synchronisée bidirectionnellement avec le champ d'édition libre
- **Préfixe et suffixe** personnalisés (non comptés dans la longueur)
- **Aperçu animé** des 500 premières combinaisons (effet de décodage) + compteur total en **BigInt** — gère les centaines de milliards de combinaisons
- **Export `.txt`** par flux incrémental (aucune saturation mémoire) avec barre de progression, vitesse, annulation et confirmation au-delà de 10 millions de lignes
- **Thème hacker** : pluie Matrix, titre glitché, scanlines et flicker CRT, glow néon, police monospace
- **Interface responsive** (mobile → desktop) et clavier (Entrée = générer, Échap = fermer les modales)

## 🚀 Utilisation

1. Télécharger `index.html`
2. Double-cliquer dessus — l'application s'ouvre dans votre navigateur
3. Régler les paramètres, puis **GÉNÉRER** pour l'aperçu ou **EXPORT .TXT** pour la liste complète

## 🖥️ Aperçu

L'interface reprend la structure des boîtes de dialogue de récupération de mot de passe, habillée d'un terminal rétro-futuriste : masque de longueur, jeux de caractères avec boutons « Détails », préfixe/suffixe, et une fenêtre de sortie style console.

## ⚠️ Avertissement légal

Cet outil est destiné aux **tests de sécurité autorisés**, à la **récupération de vos propres mots de passe** et à l'apprentissage. L'utilisation des dictionnaires générés contre des systèmes sans autorisation explicite du propriétaire est illégale.

## 🛠️ Technique

- HTML + CSS + JavaScript vanilla, zéro dépendance de build
- Énumération incrémentale type compteur base-N (production à la volée par lots)
- Comptage et tailles de fichiers en `BigInt`
- Polices : [Share Tech Mono](https://fonts.google.com/specimen/Share+Tech+Mono) & [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (repli monospace hors-ligne)

---

**Développé par Edmond NOUMEGNI** `<< Hacker Éthique >>` — [Portfolio](https://portfolio-nine-jade-22.vercel.app/)
