# 🔓 DÉVERROUILLAGE ZMK STUDIO - AIDE RAPIDE

## ⚠️ Problème : "Unlock To Continue"

Si vous voyez ce message dans ZMK Studio, c'est normal ! C'est une sécurité.

## ✅ Solution : Combo de déverrouillage

**Appuyez SIMULTANÉMENT sur ces deux touches :**

```
┌─────────────────────────────────────┐
│  CLAVIER GAUCHE    CLAVIER DROIT    │
│                                     │
│  Pouces:           Pouces:          │
│  [LWR] GUI RCTRL   SPACE ENTER [RSHFT]│
│   ↑↑↑                          ↑↑↑↑↑ │
│  Appuyez ici                Appuyez ici│
└─────────────────────────────────────┘
```

**LWR (gauche externe) + RSHFT (droite externe) = Déverrouillage !**

## 📝 Procédure complète :

1. **Connectez le clavier** à ZMK Studio (USB ou Bluetooth)
2. Vous voyez "Unlock To Continue"
3. **Appuyez simultanément** sur **LWR + RSHFT** (les deux pouces externes)
4. **Maintenez** environ 1 seconde
5. ✅ **Déverrouillé !** Vous pouvez maintenant configurer

## 🔒 Pourquoi ce verrouillage ?

C'est une protection de sécurité pour empêcher quelqu'un de modifier votre keymap à distance en Bluetooth. Vous devez avoir un accès physique au clavier pour le déverrouiller.

## 🔄 À chaque connexion

Vous devrez déverrouiller **à chaque fois** que vous connectez le clavier à ZMK Studio. C'est normal et volontaire pour la sécurité.

## 💡 Astuce

Si vous voulez changer la combo de déverrouillage (par exemple utiliser d'autres touches), modifiez cette section dans `lily58.keymap` :

```c
combo_studio_unlock {
    timeout-ms = <50>;
    key-positions = <39 44>; // Changez ces numéros
    bindings = <&studio_unlock>;
};
```

Les numéros correspondent aux positions des touches dans la matrice (0-53 pour le Lily58).

---

**Maintenant, essayez de déverrouiller ! 🔓**
