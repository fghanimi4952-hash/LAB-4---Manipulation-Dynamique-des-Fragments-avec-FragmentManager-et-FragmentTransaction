# LAB 4 - Manipulation Dynamique des Fragments

Ce projet Android démontre l'utilisation des fragments dynamiques avec `FragmentManager` et `FragmentTransaction`.

## Structure du projet

<img width="639" height="764" alt="Capture d’écran 2025-11-17 à 11 46 52" src="https://github.com/user-attachments/assets/e83f5f5e-e395-4f73-bef9-7c2069206f7b" />

## Fonctionnalités

### Fragment 1
- Affiche le texte "Fragment One"
- Bouton "Dire bonjour" qui change le texte en "Bonjour depuis Fragment 1 !"
- Logs du cycle de vie dans Logcat (onResume, onPause)

### Fragment 2
- Affiche une SeekBar (0-100)
- Le TextView affiche la valeur actuelle : "Valeur : n"
- Sauvegarde l'état lors de la rotation de l'écran

### Navigation
- Deux boutons en haut pour naviguer entre les fragments
- Le bouton "Back" permet de revenir au fragment précédent grâce à `addToBackStack()`

## Résultat :


https://github.com/user-attachments/assets/4dc76f46-c805-4a97-80c6-6c77bb3cb486



