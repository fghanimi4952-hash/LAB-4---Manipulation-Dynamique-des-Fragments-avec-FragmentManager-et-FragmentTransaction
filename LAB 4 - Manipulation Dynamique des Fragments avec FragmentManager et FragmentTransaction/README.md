# LAB 4 - Manipulation Dynamique des Fragments

Ce projet Android démontre l'utilisation des fragments dynamiques avec `FragmentManager` et `FragmentTransaction`.

## Structure du projet

```
app/
├── src/main/
│   ├── java/com/example/fragmentslab/
│   │   ├── MainActivity.java          # Contrôleur principal
│   │   ├── FragmentOne.java           # Premier fragment
│   │   └── FragmentTwo.java           # Deuxième fragment
│   ├── res/
│   │   ├── layout/
│   │   │   ├── activity_main.xml      # Layout principal
│   │   │   ├── fragment_one.xml       # Layout Fragment 1
│   │   │   └── fragment_two.xml       # Layout Fragment 2
│   │   └── values/
│   │       └── strings.xml            # Ressources string
│   └── AndroidManifest.xml
└── build.gradle
```

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

## Configuration requise

- **Min SDK**: 24 (Android 7.0)
- **Target SDK**: 34
- **Langage**: Java
- **Template**: Empty Views Activity

## Installation

1. Ouvrir le projet dans Android Studio
2. Synchroniser Gradle
3. Exécuter sur un émulateur ou un appareil Android

## Concepts appris

- **Fragment**: Partie réutilisable d'une interface avec son propre cycle de vie
- **FragmentManager**: Contrôle l'ajout, le remplacement ou la suppression de fragments
- **FragmentTransaction**: Représente une action sur les fragments (add, replace, remove)
- **addToBackStack()**: Permet de revenir au fragment précédent avec le bouton "Back"
- **onSaveInstanceState()**: Sauvegarde l'état avant destruction temporaire (rotation)
- **onViewCreated()**: Idéal pour initialiser les composants de la vue

## Debug

Pour observer le cycle de vie des fragments, ouvrez Logcat dans Android Studio et filtrez par "FragmentOne" pour voir les logs onResume() et onPause().

