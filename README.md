# Algolia

[![License](https://img.shields.io/badge/license-MIT-10b981.svg)](https://github.com/enso-ui/algolia/blob/master/LICENSE)
[![Stable](https://img.shields.io/badge/stable-2.0.1-2563eb.svg)](https://www.npmjs.com/package/@enso-ui/algolia)
[![Downloads](https://img.shields.io/npm/dm/@enso-ui/algolia.svg)](https://www.npmjs.com/package/@enso-ui/algolia)
[![Vue](https://img.shields.io/badge/vue-2.x-42b883.svg)](https://vuejs.org/)
[![JavaScript](https://img.shields.io/badge/javascript-ES2020-f7df1e.svg)](https://developer.mozilla.org/docs/Web/JavaScript)
[![npm](https://img.shields.io/badge/npm-package-cb3837.svg)](https://www.npmjs.com/package/@enso-ui/algolia)
[![Issues](https://img.shields.io/github/issues/enso-ui/algolia.svg)](https://github.com/enso-ui/algolia/issues)
[![Merge Requests](https://img.shields.io/github/issues-pr/enso-ui/algolia.svg)](https://github.com/enso-ui/algolia/pulls)

## Description

Algolia integration settings page for Enso UI.

## Installation

Install the package:

```bash
yarn add @enso-ui/algolia
```

This package is also available through the full `enso-ui` workspace bundle.

## Features

- exports the settings page used to manage Algolia integration credentials
- wraps the backend-driven Enso form contract exposed by the Laravel package
- refreshes the page-scoped form instance after the initial create flow so subsequent updates stay bound to the created settings record

## Usage

```vue
<script>
import AlgoliaSettings from '@enso-ui/algolia';

export default {
    components: { AlgoliaSettings },
};
</script>
```

## API

### `Index`

Default export for the Algolia settings page.

Import: `@enso-ui/algolia`

Props:
- No public props. The page is driven by the backend form payload.

Events:
- No public emits.

Methods:
- Internally bumps the local key after the first submit when no `settings` route param exists.

## Depends On

- [`@enso-ui/forms`](https://docs.laravel-enso.com/frontend/forms.html) [↗](https://github.com/enso-ui/forms)
- [`Vue`](https://v2.vuejs.org/)
- [`Vuex`](https://vuex.vuejs.org/)

## Contributions

are welcome. Pull requests are great, but issues are good too.

Thank you to all the people who already contributed to Enso!

## License

[MIT](https://github.com/enso-ui/algolia/blob/master/LICENSE)
