# 🎨 Guide ZMK Studio

## Qu'est-ce que ZMK Studio ?

**ZMK Studio** est une interface graphique web qui vous permet de **modifier votre keymap en temps réel** sans recompiler le firmware ! C'est comme VIA/VIAL mais pour ZMK.

## ✅ Activé dans cette configuration

ZMK Studio est maintenant **activé** dans `lily58.conf` :
```
CONFIG_ZMK_STUDIO=y
```

## 🔓 Déverrouillage de ZMK Studio

Pour des raisons de sécurité, ZMK Studio nécessite un **déverrouillage** avant utilisation.

### Comment déverrouiller :

**Appuyez simultanément sur : LWR (pouce gauche externe) + RSHFT (pouce droit externe)**

```
Pouces gauches :  [LWR] | GUI | RCTRL
                   ^^^^
                  Appuyez ici

Pouces droits :   SPACE | ENTER | [RSHFT]
                                   ^^^^^^
                              Et appuyez ici
```

**En même temps pendant 1 seconde** → ZMK Studio sera déverrouillé ! ✅

## 🚀 Comment utiliser ZMK Studio

### Étape 1 : Compiler avec ZMK Studio activé
1. Uploadez cette nouvelle configuration dans votre repo GitHub
2. Attendez que GitHub Actions compile
3. Téléchargez et flashez les firmwares

### Étape 2 : Accéder à ZMK Studio
1. **Branchez votre clavier en USB**
2. Allez sur : **https://zmk.studio**
3. Cliquez sur **"Connect"**
4. Sélectionnez votre clavier dans la liste

### Étape 3 : Modifier votre keymap
- ✅ Changez n'importe quelle touche en temps réel
- ✅ Testez immédiatement les changements
- ✅ Ajustez les layers visuellement
- ✅ Configurez les combos
- ✅ **Pas besoin de recompiler !**

## 🎯 Utiliser ZMK Studio pour corriger les inversions

Avec ZMK Studio, vous pourrez :
1. Voir exactement quelle touche physique correspond à quel keycode
2. Réassigner facilement les touches inversées
3. Tester en temps réel

**C'est PARFAIT pour diagnostiquer et corriger les problèmes de pin mapping !**

## 📝 Notes importantes

### Compatibilité
- ✅ Fonctionne en **USB**
- ✅ Fonctionne avec **Chrome/Edge** (WebHID requis)
- ❌ Ne fonctionne pas en Bluetooth
- ❌ Ne fonctionne pas avec Firefox (pas de support WebHID)

### Sauvegarde
Les modifications faites dans ZMK Studio sont :
- ✅ Sauvegardées dans le clavier (EEPROM/flash)
- ✅ Persistantes après redémarrage
- ❌ **MAIS** si vous re-flashez le firmware, elles seront perdues

**Conseil :** Une fois que vous avez trouvé la bonne configuration dans ZMK Studio, notez les changements et mettez à jour votre `lily58.keymap` pour que les modifications soient permanentes.

## 🔧 Workflow recommandé

1. **Flashez** le firmware avec ZMK Studio activé
2. **Connectez** sur https://zmk.studio
3. **Testez et ajustez** toutes les touches
4. **Notez** les corrections nécessaires
5. **Mettez à jour** le keymap dans GitHub
6. **Recompilez** avec les bonnes valeurs
7. **Re-flashez** le firmware final

## 💡 Avantages de ZMK Studio pour votre cas

Étant donné que vous avez des **inversions de touches**, ZMK Studio est **PARFAIT** car :
- Vous pouvez **voir et corriger** chaque touche individuellement
- Vous **testez immédiatement** sans recompiler
- Vous **identifiez** précisément quel keycode va où

## 🌐 Liens utiles

- **ZMK Studio** : https://zmk.studio
- **Documentation** : https://zmk.dev/docs/features/studio
- **Navigateurs compatibles** : Chrome, Edge, Opera

---

**Bonne configuration ! 🎮**
