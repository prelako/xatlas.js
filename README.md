# xatlas.js 

Forked from https://github.com/repalash/xatlas.js

## Install

```
npm i
npm run build:emcc
```

Check out the ./dist folder
```
xatlas.js
xatlas.wasm
```

Copy to your external project dir.

And include
```
import XAtlas from './xatlas.js';
const xatlas = await XAtlas()

const unwrapper = new BaseUVUnwrapper(
  { BufferAttribute: BufferAttribute },
  xatlas
);

```

Usage: geometry is THREE BufferGeometry instance
```
await unwrapper.unwrapGeometry(geometry);
```