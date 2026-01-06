# Configuration ZMK pour Silakka54 (basée sur Lily58) - QWERTZ Suisse 🇨🇭

## ✅ Ce qui a changé

Votre clavier Silakka54 fonctionne avec les pins du **Lily58**, donc cette configuration utilise :
- ✅ Le shield **Lily58** (pins compatibles avec votre Silakka54)
- ✅ Le keymap **QWERTZ Suisse** (adapté pour le layout suisse)
- ✅ Layout basé sur votre fichier JSON QMK

## 🎹 Layout configuré

### Layer 0 (Default) - QWERTZ Suisse
```
╭─────┬─────┬─────┬─────┬─────┬─────╮       ╭─────┬─────┬─────┬─────┬─────┬─────╮
│ ESC │  1  │  2  │  3  │  4  │  5  │       │  6  │  7  │  8  │  9  │  0  │  -  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB │  Q  │  W  │  E  │  R  │  T  │       │  Y  │  U  │  I  │  O  │  P  │  ü  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │  A  │  S  │  D  │  F  │  G  │       │  H  │  J  │  K  │  L  │  ö  │  ä  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHIFT│  Z  │  X  │  C  │  V  │  B  │       │  N  │  M  │  ,  │  .  │  /  │SHIFT│
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                   │ GUI │ LWR │ SPC │       │ ENT │CTRL │BSPC │
                   └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Note QWERTZ :** 
- Z et Y sont inversés par rapport à QWERTY
- Les caractères spéciaux suisses (ü, ö, ä) s'obtiennent via le système d'exploitation configuré en Suisse
- Le layout physique est adapté au QWERTZ

### Layer 1 (Lower) - Navigation & Fonctions
- Rangée 1 : ` F1 F2 F3 F4 F5 | F6 F7 F8 F9 F10 F11
- Rangée 2 : Navigation (PgUp, Up, PgDn, End, Del, F12)
- Rangée 3 : Flèches (Left, Down, Right, Home) + Crochets [ ]

### Layer 2 (Bluetooth)
- BT Clear + BT 1-5 (gestion des profils Bluetooth)

## 🚀 Comment utiliser

### Option 1 : Remplacer directement dans votre repo

1. Allez dans votre repo : https://github.com/xiff/zmk-lilly
2. Remplacez le contenu de `config/lily58.keymap` par le nouveau fichier
3. Attendez que GitHub Actions compile (5-10 min)
4. Téléchargez les nouveaux firmwares
5. Flashez les deux côtés

### Option 2 : Upload manuel

1. Clonez votre repo en local
2. Remplacez `config/lily58.keymap`
3. Commit et push
4. Attendez la compilation

## 📝 Notes importantes

- ✅ Les **pins sont corrects** (vous utilisez déjà le Lily58 qui fonctionne)
- ✅ Le **keymap correspond** à votre configuration QMK souhaitée
- ✅ **3 layers** : Default, Lower (navigation), Bluetooth

## 🎯 Accès aux layers

- **Layer 1 (Lower)** : Maintenez la touche du milieu (2ème pouce gauche)
- **Layer 2 (Bluetooth)** : Actuellement pas de combo définie
  - Option : Ajoutez une combo (ex: LWR + ESC)
  - Ou changez temporairement une touche pour accéder au layer 2

## 🔧 Personnalisation

Pour modifier le layout, éditez `config/lily58.keymap` :
- Changez les keycodes ZMK
- Ajoutez des combos
- Modifiez les layers

### Ajouter une combo pour le layer Bluetooth

Ajoutez ceci dans le keymap (après les behaviors) :

```c
combos {
    compatible = "zmk,combos";
    combo_bt {
        timeout-ms = <50>;
        key-positions = <38 39>; // LWR + SPC
        bindings = <&mo 2>;
    };
};
```

## 📖 Ressources

- [Documentation ZMK](https://zmk.dev/docs)
- [Keycodes ZMK](https://zmk.dev/docs/codes)
- [Votre repo actuel](https://github.com/xiff/zmk-lilly)

---

**Bonne continuation ! 🎮⌨️**
