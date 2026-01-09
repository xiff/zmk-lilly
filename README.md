# Configuration ZMK finale pour Silakka54 - QWERTZ Suisse 🇨🇭

## ✅ Configuration personnalisée validée

Cette configuration a été ajustée manuellement et correspond parfaitement à votre clavier Silakka54 avec SuperMini nRF52840.

## 🎹 Layout final - Lily58 (58 touches)

### Layer 0 (Default) - QWERTZ Suisse

**Côté gauche :**
```
╭─────┬─────┬─────┬─────┬─────┬─────╮
│ ESC │  1  │  2  │  3  │  4  │  5  │
├─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB │  Q  │  W  │  E  │  R  │  T  │
├─────┼─────┼─────┼─────┼─────┼─────┤
│SHIFT│  A  │  S  │  D  │  F  │  G  │
├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │  Z  │  X  │  C  │  V  │  B  │
└─────┴─────┴─────┼─────┼─────┼─────┼─────┐
                   │ LWR │ GUI │RCTRL│  /  │
                   └─────┴─────┴─────┴─────┘
```

**Côté droit :**
```
       ╭─────┬─────┬─────┬─────┬─────┬─────╮
       │  6  │  7  │  8  │  9  │  0  │  -  │
       ├─────┼─────┼─────┼─────┼─────┼─────┤
       │  Y  │  U  │  I  │  O  │  P  │  ü  │
       ├─────┼─────┼─────┼─────┼─────┼─────┤
       │  H  │  J  │  K  │  L  │  ö  │  ä  │
       ├─────┼─────┼─────┼─────┼─────┼─────┤
       │  N  │  M  │  ,  │  .  │  /  │LGUI │
   ┌─────┼─────┼─────┼─────┼─────┴─────┴─────┘
   │RALT │SPACE│ENTER│RSHFT│
   └─────┴─────┴─────┴─────┘
```

### Layer 1 (Lower) - Pavé numérique + Navigation

**Côté gauche : Pavé numérique**
```
╭────────┬─────┬─────┬─────┬─────┬─────╮
│NUMLOCK │  7  │  8  │  9  │  /  │  *  │
├────────┼─────┼─────┼─────┼─────┼─────┤
│   `    │  4  │  5  │  6  │  -  │  +  │
├────────┼─────┼─────┼─────┼─────┼─────┤
│ TRANS  │  1  │  2  │  3  │ENTER│  =  │
├────────┼─────┼─────┼─────┼─────┼─────┤
│ TRANS  │  0  │  ,  │  .  │TRANS│TRANS│
└────────┴─────┴─────┴─────┴─────┴─────┘
```

**Côté droit : Navigation**
```
      ╭──────┬──────┬──────┬──────┬──────┬─────╮
      │  F6  │  F7  │  F8  │  F9  │ F10  │ F11 │
      ├──────┼──────┼──────┼──────┼──────┼─────┤
      │ PGUP │  UP  │ PGDN │ END  │ DEL  │ F12 │
      ├──────┼──────┼──────┼──────┼──────┼─────┤
      │ LEFT │ DOWN │RIGHT │ HOME │  [   │  ]  │
      ├──────┼──────┼──────┼──────┼──────┼─────┤
      │TRANS │TRANS │TRANS │TRANS │TRANS │TRANS│
      └──────┴──────┴──────┴──────┴──────┴─────┘
```

### Layer 2 (Bluetooth) - Gestion des profils

**Rangée du haut gauche :**
- BT CLR : Effacer tous les appairages
- BT 1-5 : Sélectionner profils Bluetooth 1 à 5

Toutes les autres touches sont transparentes (passthrough).

## 🎯 Accès aux layers

### Layer 1 (Pavé numérique + Navigation)
**Maintenez LWR** (1er pouce gauche)

### Layer 2 (Bluetooth)
**Combo : SPACE + ENTER ensemble** (pouces droits 2 et 3)

## 🔓 ZMK Studio

### ⚠️ Actuellement désactivé

ZMK Studio n'est **pas disponible** dans votre version actuelle de ZMK. Cette fonctionnalité sera activable quand vous mettrez à jour vers ZMK 3.6+.

**En attendant** : Modifiez le keymap dans votre repo GitHub, recompilez avec Actions, et flashez normalement.

Consultez `NOTE_ZMK_STUDIO.md` pour plus d'infos sur comment l'activer plus tard.

## 📝 Caractéristiques

- ✅ **Layout QWERTZ Suisse** (Z et Y inversés)
- ✅ **58 touches** (Lily58 complet avec 4 pouces par côté)
- ✅ **Pavé numérique** intégré sur Layer 1
- ✅ **5 profils Bluetooth** disponibles
- ✅ **SuperMini nRF52840** compatible Nice!Nano v2
- ⏳ **ZMK Studio** (désactivé, disponible avec ZMK 3.6+)

## 🚀 Installation

1. **Uploadez** `config/lily58.keymap` et `config/lily58.conf` dans votre repo GitHub
2. **GitHub Actions** compile automatiquement (5-10 min)
3. **Téléchargez** les firmwares :
   - `lily58_left-nice_nano_v2-zmk.uf2`
   - `lily58_right-nice_nano_v2-zmk.uf2`
4. **Flashez** les deux côtés en mode bootloader (double-clic RESET)

## ⚙️ Configuration système

Pour que les caractères spéciaux suisses (ü, ö, ä) s'affichent correctement :
- Configurez votre système d'exploitation en **Suisse (Français)** ou **Suisse (Allemand)**
- Layout clavier : **Swiss QWERTZ**

## 🔧 Personnalisation

Pour modifier le keymap :
1. Éditez `config/lily58.keymap` dans votre repo
2. Ou utilisez ZMK Studio en temps réel (modifications temporaires)
3. Recompilez avec GitHub Actions

### Keycodes utiles
- Documentation complète : https://zmk.dev/docs/codes
- Behaviors ZMK : https://zmk.dev/docs/behaviors

## 📚 Ressources

- **Votre repo GitHub** : https://github.com/xiff/zmk-lilly
- **ZMK Studio** : https://zmk.studio
- **Documentation ZMK** : https://zmk.dev/docs
- **Support ZMK** : https://zmk.dev/community/discord/invite

## 💡 Conseils

- **Bluetooth** : Vous pouvez connecter le clavier à 5 appareils différents
- **Économie d'énergie** : Le clavier se met en veille après 15 minutes
- **Batterie** : Les switches ON/OFF permettent de couper complètement l'alimentation
- **ZMK Studio** : Idéal pour tester des modifications sans recompiler

---

**Profitez de votre Silakka54 ! ⌨️🎮🇨🇭**
