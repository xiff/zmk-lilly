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
       │  N  │  M  │  ,  │  .  │  /  │  $  │
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

```
  ╭────────┬──────┬──────┬──────┬──────┬──────╮ 
  │BT CLR  │ BT 1 │ BT 2 │ BT 3 │ BT 4 │ BT 5 │ 
  ├────────┼──────┼──────┼──────┼──────┼──────┤ 
  │  TRANS │TRANS │TRANS │TRANS │TRANS │TRANS │ 
  ├────────┼──────┼──────┼──────┼──────┼──────┤ 
  │  TRANS │TRANS │TRANS │TRANS │TRANS │TRANS │
  ├────────┼──────┼──────┼──────┼──────┼──────┤
  │  TRANS │TRANS │TRANS │TRANS │TRANS │TRANS │ 
  └────────┴──────┴──────┴──────┴──────┴──────┘
```

**Légende :**
- **BT CLR** : Efface tous les appairages Bluetooth
- **BT 1-5** : Sélectionne le profil Bluetooth (1 à 5)
- **TRANS** : Touche transparente (passe au layer inférieur)

Toutes les autres touches sont transparentes.

## 🎯 Accès aux layers

### Layer 1 (Lower) - Pavé numérique + Navigation
**Maintenez la touche LWR** (1ère touche de pouce gauche)

### Layer 2 (Bluetooth)
**Combo : SPACE + ENTER** (touches de pouce droites : positions 40 + 41)
- Appuyez simultanément sur SPACE et ENTER pour accéder temporairement au layer Bluetooth

## 🔓 ZMK Studio

### Déverrouillage
**Combo Studio : LWR + SPACE** (positions 39 + 40)
- Appuyez simultanément sur LWR (gauche) et SPACE (droite) pour déverrouiller ZMK Studio

### Configuration ZMK Studio
- **Activé** dans `lily58.conf` avec `CONFIG_ZMK_STUDIO=y`
- **Locking désactivé** : `CONFIG_ZMK_STUDIO_LOCKING=n`
- **Support USB-UART** activé via `build.yaml` pour le côté gauche

**Note :** ZMK Studio nécessite une version récente de ZMK (3.6+). Consultez les fichiers `NOTE_ZMK_STUDIO.md` et `GUIDE_ZMK_STUDIO.md` pour plus de détails.

## 📝 Caractéristiques principales

- ✅ **Layout QWERTZ Suisse** avec caractères spéciaux (ü, ö, ä, $)
- ✅ **58 touches** (Lily58 complet : 4 touches de pouce par côté)
- ✅ **Pavé numérique** complet sur Layer 1 (gauche)
- ✅ **Navigation complète** sur Layer 1 (droite)
- ✅ **12 touches de fonction** (F1-F12) réparties sur Layer 1
- ✅ **5 profils Bluetooth** pour connexion multi-appareils
- ✅ **ZMK Studio** support activé
- ✅ **Combos** pour accès rapide aux layers
- ✅ **Nice!Nano v2** / SuperMini nRF52840 compatible
- ✅ **Mode veille** activé (`CONFIG_ZMK_SLEEP=y`)

## 🚀 Installation

### 1. Compilation automatique (GitHub Actions)

1. **Commit** vos modifications dans `config/lily58.keymap` ou `config/lily58.conf`
2. **Push** vers votre repo GitHub : https://github.com/xiff/zmk-lilly
3. **GitHub Actions** compile automatiquement (5-10 minutes)
4. **Téléchargez** les firmwares depuis l'onglet "Actions" :
   - `lily58_left-nice_nano_v2-zmk.uf2` (côté gauche avec ZMK Studio)
   - `lily58_right-nice_nano_v2-zmk.uf2` (côté droit)

### 2. Flash du firmware

1. **Débranchez** le clavier
2. **Côté gauche** :
   - Double-cliquez sur le bouton **RESET**
   - Le clavier apparaît comme lecteur USB
   - Copiez `lily58_left-nice_nano_v2-zmk.uf2` dans le lecteur
   - Le clavier redémarre automatiquement
3. **Répétez** pour le côté droit avec `lily58_right-nice_nano_v2-zmk.uf2`

### 3. Appairage Bluetooth

1. **Activez** le Bluetooth sur votre appareil
2. **Recherchez** "Lily58" dans les périphériques disponibles
3. **Connectez-vous** (le côté gauche gère la connexion)
4. **Profils** : Utilisez Layer 2 pour basculer entre 5 appareils

## ⚙️ Configuration système

Pour un affichage correct des caractères suisses (ü, ö, ä, $) :

- **Windows** : Paramètres → Heure et langue → Langue → Français (Suisse) ou Allemand (Suisse)
- **macOS** : Préférences Système → Clavier → Sources d'entrée → Suisse (Français/Allemand)
- **Linux** : `setxkbmap ch` ou configuration dans les paramètres système

**Important** : Le keymap ZMK envoie des scancodes US, qui sont ensuite interprétés par votre OS configuré en Swiss QWERTZ.

## 🔧 Personnalisation

### Modifier le keymap

1. **Éditez** `config/lily58.keymap` dans votre repo
2. **Consultez** la documentation ZMK : https://zmk.dev/docs/codes
3. **Testez** avec ZMK Studio (modifications temporaires en temps réel)
4. **Recompilez** via GitHub Actions

### Keycodes utiles

| Type | Exemples |
|------|----------|
| **Lettres** | `&kp A` ... `&kp Z` |
| **Chiffres** | `&kp N1` ... `&kp N0` |
| **Modificateurs** | `&kp LSHIFT`, `&kp LCTRL`, `&kp LGUI`, `&kp LALT` |
| **Navigation** | `&kp UP`, `&kp DOWN`, `&kp LEFT`, `&kp RIGHT` |
| **Page** | `&kp PG_UP`, `&kp PG_DN`, `&kp HOME`, `&kp END` |
| **Fonction** | `&kp F1` ... `&kp F12` |
| **Pavé num.** | `&kp KP_N0` ... `&kp KP_N9`, `&kp KP_PLUS`, etc. |
| **Layers** | `&mo 1` (momentary), `&to 1` (toggle) |
| **Bluetooth** | `&bt BT_CLR`, `&bt BT_SEL 0` |

Documentation complète : https://zmk.dev/docs/codes

## 📚 Ressources

- **Repo GitHub** : https://github.com/xiff/zmk-lilly
- **ZMK Studio** : https://zmk.studio
- **Documentation ZMK** : https://zmk.dev/docs
- **Behaviors ZMK** : https://zmk.dev/docs/behaviors
- **Keycodes ZMK** : https://zmk.dev/docs/codes
- **Discord ZMK** : https://zmk.dev/community/discord/invite

## 💡 Conseils d'utilisation

### Bluetooth
- **5 profils** disponibles : connectez jusqu'à 5 appareils différents
- **Basculement** : Utilisez le combo SPACE+ENTER pour accéder au Layer 2, puis BT 1-5
- **Reset** : BT CLR efface tous les appairages (utile en cas de problème)

### Économie d'énergie
- **Veille automatique** : Activé après inactivité (`CONFIG_ZMK_SLEEP=y`)
- **Switches ON/OFF** : Coupez complètement l'alimentation quand non utilisé
- **Batterie** : Autonomie de plusieurs semaines selon utilisation

### ZMK Studio
- **Configuration en temps réel** : Modifiez le keymap sans recompiler
- **Déverrouillage** : Combo LWR + SPACE
- **Modifications temporaires** : Les changements ne persistent pas après redémarrage (sauvegardez dans le repo pour les garder)

### Pavé numérique
- **Accès** : Maintenez LWR (1ère touche de pouce gauche)
- **NumLock** : Active/désactive le pavé numérique
- **Layout** : Disposition classique 4×3 avec 0 en bas à gauche

---

**Profitez de votre Lily58 ! ⌨️🇨🇭**
