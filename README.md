# Configuration ZMK pour Lily58 - QWERTZ Suisse personnalisé 🇨🇭

## 🎹 Vue d'ensemble

Configuration personnalisée pour Lily58 avec SuperMini nRF52840 (compatible Nice!Nano v2).
Layout optimisé QWERTZ Suisse avec pavé numérique intégré et contrôles multimédia.

---

## 📐 Layout complet

### Layer 0 : BASE (Default)

**Côté gauche :**
```
╭─────┬─────┬─────┬─────┬─────┬─────╮
│ ESC │  1  │  2  │  3  │  4  │  5  │
├─────┼─────┼─────┼─────┼─────┼─────┤
│ TAB │  Q  │  W  │  E  │  R  │  T  │
├─────┼─────┼─────┼─────┼─────┼─────┤
│SHIFT│  A  │  S  │  D  │  F  │  G  │
├─────┼─────┼─────┼─────┼─────┼─────┼─────┐
│CTRL │  Z  │  X  │  C  │  V  │  B  │  N  │
└─────┴─────┴─────┼─────┼─────┼─────┼─────┤
                   │ ALT │  .  │SPACE│BKSP │
                   └─────┴─────┴─────┴─────┘
```

**Côté droit :**
```
       ╭─────┬─────┬─────┬─────┬─────┬─────╮
       │  6  │  7  │  8  │  9  │  0  │ NUHS│
       ├─────┼─────┼─────┼─────┼─────┼─────┤
       │  Y  │  U  │  I  │  O  │  P  │  '  │
       ├─────┼─────┼─────┼─────┼─────┼─────┤
       │  H  │  J  │  K  │  L  │  ;  │  [  │
   ┌─────┼─────┼─────┼─────┼─────┼─────┼─────┤
   │  M  │  N  │  M  │  ,  │  .  │  /  │ GUI │
   ├─────┼─────┼─────┴─────┴─────┴─────┴─────┘
   │ RET │BKSP │
   └─────┴─────┘
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
└────────┴─────┴─────┼─────┼─────┼─────┼─────┤
                      │TRANS│TRANS│TRANS│ENTER│
                      └─────┴─────┴─────┴─────┘
```

**Côté droit : Navigation + Fonctions**
```
       ╭──────┬──────┬──────┬──────┬──────┬──────╮
       │  F6  │  F7  │  F8  │  F9  │ F10  │ F11  │
       ├──────┼──────┼──────┼──────┼──────┼──────┤
       │ PGUP │ HOME │  UP  │ END  │ END  │ F12  │
       ├──────┼──────┼──────┼──────┼──────┼──────┤
       │ PGDN │ LEFT │ DOWN │RIGHT │ HOME │VOL UP│
   ┌─────┼──────┼──────┼──────┼──────┼──────┼──────┤
   │     │  4   │  {   │  }   │ LEFT │RIGHT │VOL DN│
   ├─────┼──────┼──────┴──────┴──────┴──────┴──────┘
   │TRANS│TRANS │
   └─────┴──────┘
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
├────────┼──────┼──────┼──────┼──────┼──────┼─────┐
│        │      │      │      │      │      │     │
└────────┴──────┴──────┼──────┼──────┼──────┼─────┤
                        │TRANS │TRANS │TRANS │     │
                        └──────┴──────┴──────┴─────┘
```

**Côté droit : Multimédia + Symboles**
```
       ╭──────┬──────┬──────┬──────┬──────┬─────╮
       │ PREV │ NEXT │ PLAY │VOL DN│VOL UP│     │
       ├──────┼──────┼──────┼──────┼──────┼─────┤
       │      │      │      │      │      │     │
       ├──────┼──────┼──────┼──────┼──────┼─────┤
       │      │      │  {   │  }   │  '   │     │
   ┌─────┼──────┼──────┼──────┼──────┼──────┼─────┤
   │     │      │      │ NUHS │ NUBS │      │     │
   ├─────┼──────┼──────┴──────┴──────┴──────┴─────┘
   │     │      │
   └─────┴──────┘
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

## 🎯 Accès aux layers

### Layer 1 (NUM) - Pavé numérique
**Comment y accéder :** Actuellement, pas de touche définie dans le keymap.

**💡 Suggestion :** Ajoutez `&mo 1` sur une touche inutilisée ou créez une combo pour activer ce layer.

### Layer 2 (THIRD) - Bluetooth
**Combo : SPACE + ENTER** (pouces gauche 3 + droit 1)
- Maintenez **SPACE** (pouce gauche)
- Appuyez sur **ENTER** (pouce droit)
- Le layer Bluetooth s'active temporairement

---

## 🔓 ZMK Studio (si disponible)

### Déverrouillage
**Combo : LWR (pos 39) + SPACE (pos 40)**

**⚠️ Note :** ZMK Studio nécessite ZMK 3.6+ et doit être activé dans la config. Si vous voyez une erreur de compilation concernant `studio.h`, ZMK Studio n'est pas disponible dans votre version.

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

## 🚀 Installation

### 1. Upload des fichiers
Dans votre repo GitHub **xiff/zmk-lilly** :
```
config/
├── lily58.keymap    ← Votre configuration
└── lily58.conf      ← Configuration matérielle
```

### 2. Compilation automatique
- GitHub Actions compile automatiquement à chaque commit
- Durée : 5-10 minutes
- Allez dans l'onglet **Actions** pour suivre la progression

### 3. Téléchargement des firmwares
Une fois la compilation terminée :
```
firmware/
├── lily58_left-nice_nano_v2-zmk.uf2
└── lily58_right-nice_nano_v2-zmk.uf2
```

### 4. Flash des contrôleurs
Pour chaque côté (gauche puis droit) :
1. **Double-cliquez** sur le bouton RESET du SuperMini
2. Le drive **NICENANO** ou **SUPERMINI** apparaît
3. **Copiez** le fichier .uf2 correspondant
4. Le drive **disparaît automatiquement** = flash réussi ✅
5. Le clavier redémarre avec le nouveau firmware

**Erreur Windows 0x800701B1** : C'est normal ! Cela signifie que le flash a réussi.

---

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
