# astro-merge-assets

The integration will bundle all CSS and JS files into a single file after Astro's static build.

The output after the integration runs will look like this:

```
dist
  _astro
    script.js
    style.css
  ...
```

## Setup

astro.config.ts

```ts
import { defineConfig } from 'astro/config'
import { astroMergeAssets } from 'astro-merge-assets'

export default defineConfig({
  output: 'static',

  integrations: [astroMergeAssets()],
})
```
