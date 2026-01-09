# Configuration ZMK pour Silakka54 - QWERTZ Suisse personnalisé 🇨🇭

Shield ZMK pour le clavier split **Silakka54** (54 touches).

Basé sur la configuration QMK officielle du Silakka54 par Squalius-cephalus.

## 📋 Spécifications

- **Touches** : 54 (27 par côté)
- **Matrice** : 5 rangées × 6 colonnes par côté
- **Contrôleur compatible** : RP2040 (Seeeduino XIAO RP2040, SuperMini, etc.)
- **Communication** : Serial UART (GP0/GP1)
- **Diodes** : COL2ROW

## 🎹 Layout

```
╭─────┬─────┬─────┬─────┬─────┬─────╮       ╭─────┬─────┬─────┬─────┬─────┬─────╮
│ ESC │  1  │  2  │  3  │  4  │  5  │       │  6  │  7  │  8  │  9  │  0  │  -  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB │  Q  │  W  │  E  │  R  │  T  │       │  Z  │  U  │  I  │  O  │  P  │BSPC │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │  A  │  S  │  D  │  F  │  G  │       │  H  │  J  │  K  │  L  │  ;  │  '  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHIFT│  Y  │  X  │  C  │  V  │  B  │       │  N  │  M  │  ,  │  .  │  /  │SHIFT│
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ALT │SPACE│ Mo1 │       │ RET │ Mo2 │ DEL │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

## 🎹 Vue d'ensemble

Configuration personnalisée pour Lily58 avec SuperMini nRF52840 (compatible Nice!Nano v2).
Layout optimisé QWERTZ Suisse avec pavé numérique intégré et contrôles multimédia.

---

## 📐 Layout complet

### Layer 0 : BASE (Default)

```
╭─────┬─────┬─────┬─────┬─────┬─────╮       ╭─────┬─────┬─────┬─────┬─────┬─────╮
│ ESC │  1  │  2  │  3  │  4  │  5  │       │  6  │  7  │  8  │  9  │  0  │  -  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB │  Q  │  W  │  E  │  R  │  T  │       │  Y  │  U  │  I  │  O  │  P  │BSPC │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│CTRL │  A  │  S  │  D  │  F  │  G  │       │  H  │  J  │  K  │  L  │  ;  │  '  │
├─────┼─────┼─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┼─────┼─────┤
│SHIFT│  Z  │  X  │  C  │  V  │  B  │       │  N  │  M  │  ,  │  .  │  /  │SHIFT│
└─────┴─────┴─────┼─────┼─────┼─────┤       ├─────┼─────┼─────┼─────┴─────┴─────┘
                  │ ALT │SPACE│ Mo1 │       │ RET │ Mo2 │ DEL │
                  └─────┴─────┴─────┘       └─────┴─────┴─────┘
```

**Notes importantes :**
- **NUHS** = Touche Non-US Hash (§/° sur clavier suisse)
- **ALT** = Alt gauche
- **GUI** = Touche Windows/Command (droite)
- Layout adapté au **QWERTZ Suisse**

---

### Layer 1 : NUM (Pavé numérique + Navigation)

**Côté gauche : Pavé numérique**
```
╭────────┬─────┬─────┬─────┬─────┬─────╮
│ NUMLOCK│ F1  │ F2  │ F3  │ F4  │ F5  │
├────────┼─────┼─────┼─────┼─────┼─────┤
│   `    │     │  -  │  7  │  8  │  9  │
│        │     │     │(HOME)│(UP)│(PGUP)│
├────────┼─────┼─────┼─────┼─────┼─────┤
│   /    │     │     │  4  │  5  │  6  │
│        │     │     │(LEFT)│(DN)│(RGHT)│
├────────┼─────┼─────┼─────┼─────┼─────┤
│  GUI   │     │  0  │  1  │  2  │  3  │
│        │     │(INS)│(END)│(DN)│(PGDN)│
└────────┴─────┴─────┼─────┼─────┼─────┤
                     │TRANS│TRANS│ENTER│
                     └─────┴─────┴─────┘
```

**Côté droit : Navigation + Fonctions**
```
       ╭──────┬──────┬──────┬──────┬──────┬──────╮
       │  F6  │  F7  │  F8  │  F9  │ F10  │ F11  │
       ├──────┼──────┼──────┼──────┼──────┼──────┤
       │ PGUP │ HOME │  UP  │ END  │ END  │ F12  │
       ├──────┼──────┼──────┼──────┼──────┼──────┤
       │ PGDN │ LEFT │ DOWN │RIGHT │ HOME │VOL UP│
       ├──────┼──────┼──────┼──────┼──────┼──────┤
       │  4   │  {   │  }   │ LEFT │RIGHT │VOL DN│
       ├──────┼──────┼──────┼──────┴──────┴──────┘
       │TRANS │TRANS │ DEL  │
       └──────┴──────┴──────┘
```

**Notes :**
- Les chiffres du pavé ont des **fonctions secondaires** entre parenthèses
- **F1-F12** : Touches fonction complètes
- **Contrôle du volume** : VOL UP / VOL DN

---

### Layer 2 : THIRD (Bluetooth + Multimédia)

**Côté gauche : Bluetooth**
```
╭────────┬──────┬──────┬──────┬──────┬──────╮
│ BT CLR │ BT 1 │ BT 2 │ BT 3 │ BT 4 │ BT 5 │
├────────┼──────┼──────┼──────┼──────┼──────┤
│        │      │      │      │      │      │
├────────┼──────┼──────┼──────┼──────┼──────┤
│        │      │      │      │      │      │
├────────┼──────┼──────┼──────┼──────┼──────┤
│        │      │      │      │      │      │
└────────┴──────┴──────┼──────┼──────┼──────┤
                       │TRANS │TRANS │TRANS │    
                       └──────┴──────┴──────┘
```

**Côté droit : Multimédia + Symboles**
```
       ╭──────┬──────┬──────┬──────┬──────┬─────╮
       │ PREV │ NEXT │ PLAY │VOL DN│VOL UP│     │
       ├──────┼──────┼──────┼──────┼──────┼─────┤
       │      │      │      │      │      │     │
       ├──────┼──────┼──────┼──────┼──────┼─────┤
       │      │      │  {   │  }   │  '   │     │
       ├──────┼──────┼──────┼──────┼──────┼─────┤
       │      │      │ NUHS │ NUBS │      │     │
       ├──────┼──────┴──────┴──────┴──────┴─────┘
       │TRANS │TRANS │ DEL  │
       └──────┴──────┴──────┘
```

**Légende Bluetooth :**
- **BT CLR** : Effacer TOUS les appairages
- **BT 1-5** : Sélectionner profils Bluetooth 1 à 5

**Contrôles multimédia :**
- **PREV** : Piste précédente
- **NEXT** : Piste suivante
- **PLAY** : Play/Pause
- **VOL DN/UP** : Volume -/+

**Symboles spéciaux :**
- **NUHS** : Non-US Hash (§/°)
- **NUBS** : Non-US Backslash (</>)

---

## 📝 Caractéristiques techniques

### Configuration matérielle
- **Clavier** : Lily58 (58 touches)
- **Contrôleur** : SuperMini nRF52840 (compatible Nice!Nano v2)
- **Connectivité** : Bluetooth 5.0
- **Profils BT** : 5 profils mémorisables
- **Mode veille** : Activé (CONFIG_ZMK_SLEEP=y)

### Layout et bindings
- **Layout principal** : QWERTZ Suisse
- **Layers** : 3 (BASE, NUM, THIRD)
- **Combos** : 2 (Layer BT, Studio unlock)
- **Touches encodeur** : Compatibles (si encodeur présent)

### Keycodes spéciaux utilisés
- **NUHS** : Non-US Hash - Touche §/° (clavier suisse)
- **NUBS** : Non-US Backslash - Touche </>
- **KP_Nx** : Pavé numérique 0-9
- **C_PREV/NEXT/PP** : Contrôles multimédia
- **C_VOL_DN/UP** : Volume
- **K_VOL_UP/DN** : Volume (variante keyboard)

---

## 📂 Structure des fichiers

```
config/
├── boards/shields/silakka54/
│   ├── Kconfig.shield              # Configuration du shield
│   ├── Kconfig.defconfig           # Configuration par défaut
│   ├── silakka54.dtsi              # Définition commune (matrice)
│   ├── silakka54_left.overlay      # Overlay côté gauche
│   └── silakka54_right.overlay     # Overlay côté droit
├── silakka54.keymap                # Keymap par défaut
└── silakka54.conf                  # Configuration matérielle
build.yaml                          # Configuration GitHub Actions
```

## 🔌 Pin Mapping (basé sur QMK)

### Matrice

**Rangées (Rows)** : GP2, GP3, GP4, GP5, GP6  
**Colonnes (Cols)** : GP7, GP8, GP9, GP10, GP11, GP12

### Communication split

**TX** : GP0  
**RX** : GP1

### Bootloader

- **LED** : GP17 (pour double-tap reset)
- **Double-tap** : Activé

## 🚀 Installation

### Option 1 : GitHub Actions (Recommandé)

1. **Forkez** le template : https://github.com/zmkfirmware/unified-zmk-config-template
2. **Copiez** tout le contenu de `config/` dans votre repo
3. **Modifiez** `build.yaml` avec le board correct :
   ```yaml
   include:
     - board: seeeduino_xiao_rp2040  # ou votre board
       shield: silakka54_left
     - board: seeeduino_xiao_rp2040
       shield: silakka54_right
   ```
4. **Commit & Push** → GitHub Actions compile automatiquement
5. **Téléchargez** les firmwares dans l'onglet Actions

### Option 2 : Compilation locale

```bash
# Cloner ZMK
git clone https://github.com/zmkfirmware/zmk.git
cd zmk/app

# Compiler pour le côté gauche
west build -p -b seeeduino_xiao_rp2040 -- \
  -DSHIELD=silakka54_left \
  -DZMK_CONFIG="/chemin/vers/config"

# Compiler pour le côté droit
west build -p -b seeeduino_xiao_rp2040 -- \
  -DSHIELD=silakka54_right \
  -DZMK_CONFIG="/chemin/vers/config"
```

## 🔧 Flash du firmware

### Avec SuperMini nRF52840

⚠️ **ATTENTION** : Le SuperMini utilise un **nRF52840** (Bluetooth natif), pas un RP2040 !

Si vous avez un **SuperMini nRF52840**, changez le board dans `build.yaml` :

```yaml
include:
  - board: nice_nano_v2  # Compatible SuperMini nRF52840
    shield: silakka54_left
  - board: nice_nano_v2
    shield: silakka54_right
```

### Procédure de flash

1. **Double-cliquez** sur le bouton RESET du contrôleur
2. Le drive **bootloader** apparaît (RPI-RP2, NICENANO, ou SUPERMINI)
3. **Copiez** le fichier `.uf2` correspondant
4. Le drive **disparaît automatiquement** = flash réussi ✅

### Erreur Windows 0x800701B1

C'est **normal** ! Cela signifie que le flash a réussi et le contrôleur a redémarré.

## ⚙️ Personnalisation

### Modifier le keymap

Éditez `config/silakka54.keymap` :

```c
&kp ESC   &kp N1 &kp N2 ...  // Changez les keycodes
```

### Ajouter un layer

```c
my_layer {
    bindings = <
        // Votre layout ici
    >;
};
```

## ⚙️ Configuration système (OS)

Pour que tous les caractères s'affichent correctement :

### Windows
```
Paramètres → Heure et langue → Langue et région
→ Ajouter une langue → Français (Suisse) ou Allemand (Suisse)
→ Options → Ajouter un clavier → Suisse (QWERTZ)
```

### macOS
```
Préférences Système → Clavier → Méthodes de saisie
→ + → Français/Allemand → Suisse
```

### Linux
```
Settings → Region & Language → Input Sources
→ + → French (Switzerland) ou German (Switzerland)
```

---

## 🔧 Personnalisation

### Modifier le keymap
1. Éditez `config/lily58.keymap` dans GitHub
2. Commit les changements
3. Attendez la recompilation (Actions)
4. Téléchargez et flashez

### Keycodes ZMK
Référence complète : https://zmk.dev/docs/codes

**Exemples utiles :**
- `&kp KEY` : Keypress simple
- `&mo N` : Momentary layer (maintenir)
- `&lt N KEY` : Layer-tap (maintenir = layer, tap = touche)
- `&mt MOD KEY` : Mod-tap (maintenir = modificateur, tap = touche)
- `&trans` : Transparent (passe au layer du dessous)
- `&none` : Aucune action

### Ajouter des combos
Exemple pour accéder au layer NUM :
```c
combo_num_layer {
    timeout-ms = <50>;
    key-positions = <38 39>; // ALT + DOT (pouces gauche)
    bindings = <&mo 1>;
};
```

---

## 📊 Mappage des positions des touches

Pour créer des combos, voici les **key-positions** :

```
Lily58 Key Positions:
 0  1  2  3  4  5                    6  7  8  9 10 11
12 13 14 15 16 17                   18 19 20 21 22 23
24 25 26 27 28 29                   30 31 32 33 34 35
36 37 38 39 40 41 42          43 44 45 46 47 48 49 50
            51 52 53 54    55 56 57 58
```

**Pouces gauches :** 51, 52, 53, 54  
**Pouces droits :** 55, 56, 57, 58

**⚠️ Note :** Le keymap utilise parfois des positions simplifiées. Les positions exactes peuvent varier selon le shield Lily58 spécifique.

---

## 🔋 Gestion de l'alimentation

### Bluetooth
- **5 profils** : Connectez jusqu'à 5 appareils différents
- **Changement de profil** : Layer 2 → BT 1-5
- **Effacer les profils** : Layer 2 → BT CLR

### Autonomie
- **Veille automatique** : Activée après inactivité
- **Switches ON/OFF** : Sur le SuperMini pour couper complètement
- **Batterie LiPo** : Typiquement plusieurs semaines d'autonomie

---

## 💡 Astuces et conseils

### Pavé numérique (Layer 1)
Les chiffres ont des **fonctions de navigation intégrées** :
- 7 (HOME), 8 (UP), 9 (PGUP)
- 4 (LEFT), 5 (DOWN), 6 (RIGHT)
- 1 (END), 2 (DOWN), 3 (PGDN)
- 0 (INSERT)

C'est pratique pour la navigation sans quitter le pavé numérique !

### Contrôles multimédia
Le layer THIRD (Bluetooth) inclut des **contrôles média** :
- Changement de piste : PREV/NEXT
- Lecture : PLAY (Play/Pause)
- Volume : VOL UP/DN

Parfait pour contrôler la musique sans quitter votre application !

### Symboles suisses
- **§/°** : NUHS (disponible en layer 0 et 2)
- **</>** : NUBS (layer 2)
- **ü, ö, ä** : Via le layout système QWERTZ Suisse

---

## 🐛 Dépannage

### Le clavier ne compile pas
- **Erreur `studio.h`** : Retirez les lignes ZMK Studio (voir section ZMK Studio)
- **Erreur de syntaxe** : Vérifiez les virgules, points-virgules, accolades
- **Keycode invalide** : Consultez https://zmk.dev/docs/codes

### Une touche ne fonctionne pas
1. Testez avec un **testeur de clavier** : https://www.keyboardtester.com
2. Vérifiez le **keycode** dans le .keymap
3. Vérifiez que le **layout système** est bien QWERTZ Suisse

### Le Bluetooth ne se connecte pas
1. **Effacez les profils** : Layer 2 → BT CLR
2. **Côté OS** : Oubliez l'appareil puis reconnectez
3. **Vérifiez la batterie** : Peut-être déchargée

### Layer inaccessible
- **Layer 1 (NUM)** : Ajoutez `&mo 1` sur une touche ou créez une combo
- **Layer 2 (THIRD)** : Utilisez la combo SPACE + ENTER

---

## 📚 Ressources

### Documentation officielle
- **ZMK Docs** : https://zmk.dev/docs
- **Keycodes** : https://zmk.dev/docs/codes
- **Behaviors** : https://zmk.dev/docs/behaviors
- **Combos** : https://zmk.dev/docs/features/combos

### Communauté
- **Discord ZMK** : https://zmk.dev/community/discord/invite
- **GitHub ZMK** : https://github.com/zmkfirmware/zmk

### Votre configuration
- **Repo GitHub** : https://github.com/xiff/zmk-lilly
- **Actions** : https://github.com/xiff/zmk-lilly/actions

---

## 📄 Changelog

### Version actuelle
- ✅ Layout BASE complet (QWERTZ Suisse)
- ✅ Layer NUM avec pavé numérique + navigation
- ✅ Layer THIRD avec Bluetooth + multimédia
- ✅ Combos : Layer BT, Studio unlock
- ✅ Configuration optimisée pour SuperMini nRF52840

---

**Bonne frappe ! ⌨️🇨🇭**
