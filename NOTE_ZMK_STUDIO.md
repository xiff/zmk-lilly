# ⚠️ NOTE SUR ZMK STUDIO

### Option 1 : Mettre à jour ZMK (Recommandé)

Quand ZMK 3.6+ sera stable ou disponible dans votre build :

1. **Mettez à jour** votre repo ZMK
2. **Décommentez** dans `lily58.conf` :
   ```
   CONFIG_ZMK_STUDIO=y
   ```
3. **Ajoutez** dans `lily58.keymap` :
   ```c
   #include <dt-bindings/zmk/studio.h>
   ```
4. **Ajoutez** un combo de déverrouillage :
   ```c
   combo_studio_unlock {
       timeout-ms = <50>;
       key-positions = <39 40>; // LWR + SPACE
       bindings = <&studio_unlock>;
   };
   ```
5. **Recompilez**

### Option 2 : Utiliser une branche de développement

Si vous voulez ZMK Studio maintenant :
1. Modifiez votre workflow GitHub Actions pour utiliser la branche `main` ou une branche avec Studio
2. Référence : https://zmk.dev/docs/development/build-flash

# 🎨 Guide ZMK Studio

## Qu'est-ce que ZMK Studio ?

**ZMK Studio** est une interface graphique web qui vous permet de **modifier votre keymap en temps réel** sans recompiler le firmware ! C'est comme VIA/VIAL mais pour ZMK.

## ✅ Activé dans cette configuration

ZMK Studio est maintenant **activé** dans `lily58.conf` :
```
CONFIG_ZMK_STUDIO=y
CONFIG_ZMK_STUDIO_LOCKING=n
```

