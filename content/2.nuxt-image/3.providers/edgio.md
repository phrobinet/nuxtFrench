---
title: Edgio
description: Optimize images with Edgio (formerly Layer0)'s optimization service.
links:
  - label: Source
    icon: i-simple-icons-github
    to: https://github.com/nuxt/image/blob/main/src/runtime/providers/edgio.ts
    size: xs
---

Edgio fournit un service HTTP simple pour optimiser les images.

::callout
#summary
L'optimiseur d'images ne renverra qu'une image optimisée aux navigateurs mobiles. Les navigateurs de bureau reçoivent l'image d'origine.
::

Cette intégration fonctionne directement sans avoir besoin de configuration ! Consultez la [Documentation](https://docs.edg.io/guides/image_optimization) pour plus d'informations.

**Exemple :**

```vue
<NuxtImg provider="edgio" src="https://i.imgur.com/LFtQeX2.jpeg" width="200" height="200" quality="80" />
```

## Modificateurs

Edgio prend en charge les modificateurs suivants : `height`, `width` et `quality`

## Options

### `baseURL`

- Par défaut : `https://opt.moovweb.net`
