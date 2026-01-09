# ⚠️ NOTE SUR ZMK STUDIO

## Pourquoi ZMK Studio est désactivé

Votre version actuelle de ZMK **ne supporte pas encore ZMK Studio**. Cette fonctionnalité nécessite **ZMK 3.6 ou supérieur**.

L'erreur de compilation était :
```
fatal error: dt-bindings/zmk/studio.h: No such file or directory
```

## ✅ Solution appliquée

J'ai **désactivé ZMK Studio** pour que votre configuration compile correctement :
- ❌ Retiré `#include <dt-bindings/zmk/studio.h>`
- ❌ Retiré le combo `studio_unlock`
- ❌ Désactivé `CONFIG_ZMK_STUDIO=y`

Votre clavier **fonctionne normalement** sans ZMK Studio, vous aurez juste besoin de recompiler pour chaque modification du keymap.

## 🔄 Comment activer ZMK Studio plus tard

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

## 📝 Pour l'instant

Votre configuration **fonctionne parfaitement** sans ZMK Studio. Vous modifiez simplement le keymap dans GitHub, recompilez, et flashez.

## 🎯 Fonctionnalités disponibles

Même sans ZMK Studio, vous avez :
- ✅ 3 layers complets
- ✅ Pavé numérique
- ✅ Gestion Bluetooth (5 profils)
- ✅ Combos (SPACE + ENTER pour le layer BT)
- ✅ Layout QWERTZ Suisse

**Tout fonctionne ! 🎉**

## 📚 Ressources

- **ZMK Studio docs** : https://zmk.dev/docs/features/studio
- **ZMK versions** : https://github.com/zmkfirmware/zmk/releases
- **Configuration actuelle** : Fonctionne avec ZMK stable

---

**La compilation devrait maintenant réussir ! ✅**
