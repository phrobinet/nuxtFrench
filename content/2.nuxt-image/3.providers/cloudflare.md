---
title: Cloudflare
description: Nuxt Image dispose d'une intégration de premier ordre avec Cloudflare.
links:
  - label: Source
    icon: i-simple-icons-github
    to: https://github.com/nuxt/image/blob/main/src/runtime/providers/cloudflare.ts
    size: xs
---

Intégration entre [Cloudflare](https://developers.cloudflare.com/images/) et le module d'image.

Pour utiliser ce fournisseur, vous avez simplement besoin de spécifier l'URL de base (zone) de votre service :

```ts [nuxt.config.ts]
export default defineNuxtConfig({
  image: {
    cloudflare: {
      baseURL: 'https://that-test.site'
    }
  }
})
```

**Exemple :**

```vue
<NuxtImg provider="cloudflare" src="/burger.jpeg" height="300" :modifiers="{ fit: 'contain' }" />
```

## Options

### `baseURL`

Par défaut : `/`

Le domaine de votre déploiement (zone).

**Note :** `/cdn-cgi/image/` sera automatiquement ajouté pour générer les URLs.
