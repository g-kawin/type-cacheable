# @type-cacheable/node-cache-adapter

TypeScript-based caching decorators to assist with caching (and clearing cache for) async methods. This package supports the `node-cache` client.

[View full documentation](https://github.com/joshuaslate/type-cacheable)

## Usage

### Installation

```bash
npm install --save @type-cacheable/core @type-cacheable/node-cache-adapter
```

or

```bash
yarn add @type-cacheable/core @type-cacheable/node-cache-adapter
```

### Using adapter

```ts
import * as NodeCache from 'node-cache';
import { useAdapter } from '@type-cacheable/node-cache-adapter';

const client = new NodeCache();
useAdapter(client);
```

Then you can rely on the `@Cacheable` and `@CacheClear` decorators from `@type-cacheable/core`. [See core documentation](https://github.com/joshuaslate/type-cacheable/tree/master/packages/core)